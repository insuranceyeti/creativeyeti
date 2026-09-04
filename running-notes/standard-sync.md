# Standard sync — the update ledger

This is the one file that says how this brain relates to the `parker-brain` factory: which
release it runs, what posture it holds toward updates, and every offer the team has answered.
`/disconnect-factory` flips the posture; nothing else edits the header block.

## Where this brain stands

- **Factory remote:** https://github.com/real-simple-labs/parker-brain
- **Posture:** `follow`
- **Pinned release:** `v15` (matches `parker_config.json` → `parker_brain_version`)
- **Migrations applied through:** `v15`
- **Last compared:** 2026-09-03 against `v15` (newest published tag; `v16` exists in the
  factory's `main` but has no release tag yet)
- **Verified 2026-09-04:** the mount is initialized and clean at commit `b55c441`. **Note for
  whoever reads `git submodule status` next: it prints `(v14)`, not `(v15)`, and that is not
  drift.** The factory has `v14` and `v15` pointing at the *same commit* — `git tag --points-at
  HEAD` returns both — and `git describe` just picks one of them. The pin is `v15`, as recorded
  here and in `parker_config.json`. Do not "correct" either file to v14 and do not re-pin on
  this basis.

## Repo posture — self-managed

**This brain is self-managed, not Parker Desktop managed.** Read this before applying any
Parker Desktop guidance in the method docs, because that guidance does not apply here.

Parker provisioned a managed repo for this brand at `parker-brain/insuranceyeti-health-for-moms`,
but it could not be reached from the build session: that session's egress proxy injects git
credentials only for repositories in its authorized set, and the managed repo is under a
different GitHub owner than the session was scoped to. `add_repo` refused it as a cross-tier
add. So the brain lives in the team's own repository instead.

- **This repo:** https://github.com/insuranceyeti/creativeyeti
- **Managed repo, provisioned but empty:** https://github.com/parker-brain/insuranceyeti-health-for-moms
- **Sync:** ordinary git with the team's own credentials. `save-brain`'s managed-credential
  procedure (the `setup_parker_brain` token and `.git/parker-credentials`) does **not** apply —
  that skill's "self-hosted (the rare exception)" branch is the one that governs here.
- **Parker Desktop does not watch this folder.** Nothing syncs automatically; work is saved by
  committing and pushing.

### The session-start pull fails, and it is benign — recorded 2026-09-04

The session-start hook runs `git pull --rebase origin main` and reports
`fatal: couldn't find remote ref main`. **That is not auth, not drift, and not a broken remote.
This repository has no `main` branch at all.** `git ls-remote --heads origin` returns exactly two
refs, both feature branches: `claude/parker-brain-health-for-moms-x0vbs5` (where the build lives)
and `claude/parker-mcp-http-349ri1` (the earlier session's branch).

So the `save-brain` rule that "everything lands on `main`, no feature branches" cannot be followed
literally here — there is no `main` to land on. Until the team creates one or promotes a branch,
the working rule for this brain is: **pull and push the current working branch by name.** The build
has been pushed to `claude/parker-brain-health-for-moms-x0vbs5` throughout, and GitHub pull request
[#1](https://github.com/insuranceyeti/creativeyeti/pull/1) tracks it.

**What to do about it is the team's call, not Parker's.** Merging that pull request would create the
`main` this brain's own procedure assumes, after which the hook stops failing and the standard save
path works as written. Until then, ignore the pull error rather than "fixing" it by creating a
branch nobody asked for.

To move this brain into the managed repo later, run a session rooted on
`parker-brain/insuranceyeti-health-for-moms` and copy this tree across, then flip this section.

## Offer history

Append one line per offer, newest first: date — item — taken / declined (why, if given) / deferred.

- 2026-09-03 — initial mount at `v15` — taken (build time, not an offer)
