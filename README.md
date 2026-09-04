# Health For Moms — the brand brain

This repository is everything Parker knows about Health For Moms: the brand, the customer, the account, the creative read on top of it, and the method that produced all of it. It is not a folder of reports. It is a thing you talk to.

**Built 2026-09-03 and 2026-09-04.** 56 standing documents, roughly 300,000 words, plus the strategy set and the Phase-3 creative work.

## Start here

**Open this repo in Claude Code and run `/get-started`.** That is the one move that needs no map. It reads the brain as it stands today, works out how familiar you are with this kind of system, and walks you through what is here and what to do first — one thing at a time, grounded in this brand's own numbers, ending on a single first move. It is re-runnable by anyone, any time, including a teammate who clones this repo next month.

If you would rather read than be walked through it, in this order:

1. **`sub-context-docs/brand-profile-narrative.md`** — the one-pager. Everything else hangs off it.
2. **`strategy/strategic-roadmap.md`** — the diagnosis and the three priorities. **Drafted, not approved.** It is waiting on the team.
3. **`CLAUDE.md`** — the operating contract. The hard rules sit first, and they outrank everything else in the repo.
4. **`brand-lens.md`** — this brand's own tribal knowledge, the overlay every creative output loads on top of the general method.
5. **`open-loops/open-loops-roll-up.md`** — the 57 graded questions this brain is still carrying, cut down from 212.

## What is in here

| Folder | What it holds |
|---|---|
| `sub-context-docs/` | The foundation reads — brand, category, competitors, journey, website, account, targets, organic, reputation, visual vocabulary, operations, calendar. 14 docs. |
| `personas/` | The personas profile, the voice library, the lifecycle maps, the bias notes, and `voice-of-customer/` with 11 extracted language slices. |
| `source-pulls/` | The raw source reads the personas and voice-of-customer work were built from. 8 files, including the honest named blanks. |
| `audits/` | The account cadence layer, date-bucketed. 12 cuts baselined at build. See `audits/INDEX.md`. |
| `strategy/` | The four Phase-2 inputs and the roadmap they converged into. |
| `idea-bank/`, `sprints/` | The Phase-3 creative memory and the round of work that came out of it. |
| `open-loops/`, `hypotheses/`, `validations/`, `re-validations/` | The research pipeline — the questions, the tests, and the honest resolutions. |
| `running-notes/` | The brand rules, the success definition, the missing-context list, the freshness schedule, the routine log, and the update ledger. |
| `competitors/` | Empty on purpose. `competitors/INDEX.md` says why and what it costs. |
| `.claude/skills/` | The skills. What makes this brain executable rather than readable. |
| `parker-system/` | The method, mounted read-only and pinned to a release. |

## What Parker could see, and what stayed dark

Tested 2026-09-03, re-verified through the build.

**Live:** the brand context document; the Meta ad account (`HealthForMoms`, act 484897827497337 — 136 ads, $98,277 across 90 days, 4,336 leads, $22.67 cost per lead); Facebook ad comments (1,342 rows, 2025-01-08 to 2026-09-03); a 23-video TikTok mining library; and the Parker chat history.

**Dark, and every doc in here says so rather than filling the gap:**

- **Customer reviews — zero rows.** The team confirmed none exist.
- **Post-purchase surveys — zero rows.**
- **Competitor ad library — no brands tracked.** One external brand is configured, Ethos, and it sells term life. The competitor branch and all six external audit cuts are deferred at the team's request.
- **Northbeam — not connected.** Every figure here is Meta-reported on the org default attribution window. Nothing is multi-touch.
- **Gate two — lead quality.** It lives with the partner insurance agencies and nothing in this brain reaches it. The account fired 44 `Call` events against 4,421 leads in the trailing 90 days.
- **Reddit — unreachable** at build time.

**Two things this shape means, and they govern every read in here.** First, this is lead generation with zero purchase events, so ROAS, AOV and purchase value are meaningless and never appear. Second, the only first-party language surface is comments under the brand's own paid ads, so every persona is capped at mixed confidence and the honest sentence is always "commenters under the brand's paid ads said," never "customers said."

## The method travels with the repo

This brain can refresh, rebuild and execute itself, because both halves of the method ship inside it.

**The skills**, in `.claude/skills/`, load automatically when you open this repo in Claude Code, after a one-time trust prompt. Two kinds live there together. The **craft** skills do the work — `/scriptwriting`, `/hooks`, `/headlines`, `/iterations`, `/ad-account-analysis`, `/ai-ad-generation`, the open-loops pipeline. The **routine** skills keep the brain alive — `/refresh-context`, `/research-loops`, `/dream`, `/harvest-ideas`, `/evaluate-ideas`, `/self-improve`, `/update-brain`, plus `/setup-routines` and `/get-started`.

**The method**, at `parker-system/`, is the factory's own prompts, craft knowledge and system docs, mounted **read-only and pinned to release `v15`**. Read-only matters: the brain reasons with it but never edits it. Pinned matters too — a refresh re-runs a document's *own* generating prompt at the exact version it was built with, rather than improvising a new one.

It is a git submodule, so a fresh clone needs `git clone --recurse-submodules`. If you forget, the brain notices on the next session and tells you to run `git submodule update --init parker-system`.

**Updates are opt-in.** `/update-brain` compares the pinned release against the newest factory release once a week and offers the bump as one short question. What the team declines stays declined; what the team changed stays theirs. The full record is `running-notes/standard-sync.md`.

## What this brain does on its own

Six routines run on a schedule without being asked: the freshness sweep, the research cycle, the nightly dreaming pass, the weekly idea hunt and its grading, the self-improvement curation, and the update check. The recipes live in `schedules/` and travel with the repo. **The schedules themselves are per-account and cannot be committed**, so a brain cloned onto a new machine arrives un-armed — run `/setup-routines` there once to start the clock. The same command changes any cadence or turns a routine off.

`running-notes/routine-log.md` is the record of what actually fired and when. `running-notes/refresh-schedule.md` is the live view of what is due.

## Where this brain is saved

**https://github.com/insuranceyeti/creativeyeti** — the team's own repository, synced with ordinary git. Parker Desktop does not watch this folder; work is saved by committing and pushing. The full posture, and the path to move this into Parker-managed storage later, is in `running-notes/standard-sync.md`.

## One caveat that sits on the whole repo

**The strategic roadmap is drafted and unapproved.** It carries `status: drafted, awaiting review` and `approved_by: null`. Its three priorities are the best-evidenced direction in this brain — four independent strategy inputs converged on them without seeing each other — and they are still provisional until the team signs off. Everything downstream of it, including the Phase-3 idea grading and the briefs, is labeled accordingly. Approving or reordering that roadmap is the highest-value thing anyone can do with this brain today.
