# Brand rules — the standing constraints

> Source: brand intake, 2026-09-03, plus the Phase 0 surface test. Everything marked `stated`
> is brand input, not verified fact.

## How performance is judged

- **North star:** CPL first, then lead quality before real scale. Two gates, not one.
  Full definition in `success-definition.md`. (`stated`)
- **Objective:** efficiency before volume. (`stated`)
- **Reporting surface:** Meta Ads Manager, in-platform. No third-party attribution. (`stated`)
- **Never report ROAS, AOV, purchase value or add-to-cart** for this brand. The account has
  zero purchase events by design; it is lead generation. ROAS reads 0 everywhere and reporting
  it as a performance figure is a fabrication. (`verified` — Phase 0 pull, 2026-09-03.)

## Open — not answered at intake

- **Spend-versus-efficiency tiebreak.** Asked at intake; the team expressed no preference.
  Until they do, when two ads in one ad set diverge on spend, **report both readings**: what
  the spend split implies about Meta's delivery, and what the CPL comparison implies about
  efficiency. Do not silently pick one. Re-ask when there is a real decision riding on it.
- **Ad naming convention** — not yet captured.
- **Brief template** — not yet captured. Until it is, briefs follow the factory format in
  `parker-system/prompts/ideas-and-briefs/brief-creation.md`.
- **Unit economics** — customer value, gross margin, LTV or payback window, max tolerable CPA.
  Not captured. Without a max CPA there is no ceiling to hold reads against, so "efficient"
  is currently relative to the account's own trailing CPL, not to a business threshold.

All of the above are logged in `missing-context.md` as open questions, never blockers.

## Campaign structure — observed, not stated

From the Phase 0 pull: campaigns run under a `USHA - ABO - {SCALE|TEST} - MOMS` shape, with
ad sets named by audience cohort and iteration (e.g. `Moms43 - 4 (State Moment)`) and ads
suffixed by version (`- V1`, `- V3`). This is an inference from names, not a stated convention.
Treat it as a working read until the team confirms it. (`inferred` — Phase 0 pull, 2026-09-03.)
