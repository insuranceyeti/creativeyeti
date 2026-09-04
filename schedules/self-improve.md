# Schedule — self-improve

- **Task:** The weekly governance pass. Curate captured reasoning traces and promote (provenance-tied) into `applied-changes.md`; dispose of `dreaming/proposals/pending/` with the human in the loop; advance weighted open loops into hypotheses via the roll-up (kill list → re-formulate → score /20 → promote); run any re-validations that have come due.
- **Cadence:** Weekly (continuous capture happens during everyday work; this is the weekly curation that promotes carefully).
- **Sources:** `self-improvement/reasoning-traces/`, `dreaming/proposals/pending/`, `schedules/proposed/`, every context doc's open-loops + `open-loops/`, `hypotheses/`, `validations/`, `re-validations/scheduled/`.
- **Skill:** `.claude/skills/self-improve/` (`/self-improve`). Scaffolds `self-improvement/` on first run if absent.
- **Deliverable:** Promotions logged with cited trace IDs; proposals moved to applied/dismissed with reasoning; Tier-1 loops promoted into `hypotheses/`; due re-validations filed under `re-validations/results/`; a report of what was promoted, what awaits the user, and what was killed (and why).
- **Origin:** Seeded 2026-06-18 from the factory's `self-improvement/self-improvement-system.md` + `parker-system/system/open-loops-system.md`.
- **Status:** **Active.** Registered 2026-09-04 by the onboarding build (build mode, `/setup-routines`) on mike@americafirstleads.com's account as routine `trig_017qzoFfMN32isDeUoMkpMLG`, named "Health For Moms: self-improvement". Fires Fridays 16:12 America/New_York (`12 20 * * 5` UTC); next run 2026-09-11 20:12 UTC. Each firing starts a fresh cloud session in this repo's environment.
  - **Known limitation, recorded 2026-09-04:** the routine was created without MCP connectors attached, so its fired sessions run with **no Parker MCP tools**. This one curates files already in the repo, so it works without connectors. Fix: recreate or edit the routine from the claude.ai Routines UI with the Parker connector attached, or from a session that holds it. Until then, run this routine by hand with its slash command, where the connectors are live.

## Schedule recipe (register once via `/schedule`)

> **Cadence:** weekly, Friday 16:00 (user's timezone) — end-of-week, so it disposes of the week's dreaming proposals and freshly captured traces.
> **Prompt:** "Run the /self-improve routine for the brand brain in this repo. Follow the skill exactly: curate reasoning traces, dispose of dreaming proposals (human in the loop — surface decisions, don't silently promote), advance open loops into hypotheses via the roll-up, run due re-validations. Report what was promoted, what awaits me, and what was killed."

> **This is the disposing half: dreaming proposes, self-improve disposes. Nothing canonical changes without going through this pass and the human.**
