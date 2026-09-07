# Routine log — Health For Moms

The append-only record of everything the brain did on its own. Each standing routine (`/refresh-context`, `/research-loops`, `/dream`, `/harvest-ideas` + `/evaluate-ideas`, `/self-improve`, `/update-brain`) writes one entry here every time it runs, scheduled or manual, newest at the top.

This is the history — what fired, when, what it changed, what it left, and why. It is distinct from `refresh-schedule.md`, which tracks only current due dates. This file is never overwritten, only appended.

Read it to answer "what has the brain been doing," to see whether a scheduled routine actually fired, and to trace when a doc last changed and which run changed it.

## Entry shape

Each entry is one dated block. Keep it short — the routine's own deliverable holds the detail; this is the ledger line.

```
### YYYY-MM-DD HH:MM · [routine] · [scheduled | manual]
- **Checked:** what the run examined.
- **Did:** what it changed, named — or "nothing due."
- **Left:** what it deliberately did not do, and why (fresh, awaiting user, gated).
- **Surfaced:** any open loop, idea, conflict, or proposal raised for a downstream routine or the user.
```

## Log

<!-- newest entries at the top; routines prepend here -->

### 2026-09-05 · setup · manual

- **Checked:** the build's own finish checklist against what is actually on disk, plus the live
  routine list for this account.
- **Did:** stamped the four missing contract files (`CLAUDE.md`, `README.md`, `brand-lens.md`,
  `running-notes/refresh-schedule.md`), created this log, scaffolded `expert-insights/`, and
  corrected `BUILD-STATUS.md`, which still reported Phase 2 and Phase 3 as blocked when both had
  completed on 2026-09-04.
- **Routines — corrected a wrong record.** All six `schedules/*.md` status lines claimed the
  schedules were "not yet registered." The live routine list says otherwise: **the build armed all
  six on 2026-09-04 at 21:14**, and dreaming has already fired once successfully (2026-09-05 08:57
  UTC). Acting on the stale stamps, this run created five duplicate routines and then deleted all
  five once the live list was read. Net change to what runs: none, except dreaming. Every status
  line now reflects live state with its trigger id.
- **Dreaming disabled** at the user's request (`trig_01VTKecvDtKudiMygVoshuBk`, was daily 08:57
  UTC). Disabled rather than deleted, so re-arming is one step. Reason: the team is just starting,
  dreaming needs daily conversations to read, and it is the heaviest of the six on usage.
- **Left:** the sprint plan and the creative briefs, both unbuilt — they wait on roadmap approval.
  The competitor branch and all six external audit cuts stay deferred at the team's request.
- **Surfaced:** three things. The roadmap is still `drafted, awaiting review` with `approved_by:
  null`, which caps the whole Phase-3 layer as provisional and is the brand's next real decision.
  Scheduled runs fire **without the Parker MCP connector** — the org does not permit attaching
  connectors to routines — so every scheduled routine is data-limited on live account reads until
  that changes; a routine's findings should be read with that in mind, and the skills' own
  honest-blank discipline is what keeps it from fabricating. And a live pull today confirmed the
  two non-compliant claims still run on all five top-spending active ads.
