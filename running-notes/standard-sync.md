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

To move this brain into the managed repo later, run a session rooted on
`parker-brain/insuranceyeti-health-for-moms` and copy this tree across, then flip this section.

## Offer history

Append one line per offer, newest first: date — item — taken / declined (why, if given) / deferred.

- 2026-09-03 — initial mount at `v15` — taken (build time, not an offer)
