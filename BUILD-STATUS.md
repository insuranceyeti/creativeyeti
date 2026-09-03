# Build status — Health For Moms brand brain

**Brand:** Health For Moms (`aed0ff06-555d-4f4f-9bf8-31178e2fb977`)
**Build started:** 2026-09-03
**Method version:** parker-brain `v15`
**Run id:** `e5c1cbe7-0bba-4a1e-8b7e-9bdc075777e1`
**Current phase:** Phase 0 — Repo & Scaffold

**Saved to:** https://github.com/insuranceyeti/creativeyeti (branch `claude/parker-mcp-http-349ri1`)
**Repo posture:** self-managed — see `running-notes/standard-sync.md`

## What is happening right now

Phase 0 is complete and saved. The flat layout is scaffolded, the factory method is mounted
read-only at `parker-system/` pinned to v15, the executable layer is shipped, and every data
surface has been tested. Phase 1 is next.

## Scoreboard

| Phase | Status | Done / Total |
|---|---|---|
| Phase 0 — Repo & Scaffold | **done** | 7 of 7 |
| Phase 1A — Brand foundation | pending | 0 of 14 |
| Phase 1B — Competitor profiles | **deferred** | 0 of 0 |
| Phase 1C — Persona source pulls | pending | 0 of 12 |
| Phase 1D — Voice of customer | pending | 0 of 12 |
| Phase 1E — Audit baseline (internal) | pending | 0 of 11 |
| Phase 1E — Audit baseline (external) | **deferred** | 0 of 6 |
| Phase 1 — Synthesis | pending | 0 of 2 |
| Phase 2 — Strategy | pending | 0 of 5 |
| Phase 3 — Ideation | pending | 0 of 4 |
| Stamp / verify / hand off | pending | 0 of 4 |

## Data surfaces — tested 2026-09-03

| Surface | State | Note |
|---|---|---|
| Brand context document | live | ~50KB, detailed |
| Meta ads (`HealthForMoms`, act 484897827497337) | live | 136 ads, $98,277 / 90d, 4,336 leads, $22.67 CPL |
| Facebook ad comments | live | current through today |
| TikTok mining library | live | 23 relevancy-scored videos |
| Parker chat history | live | 4 threads (1 web, 3 Slack) |
| Customer reviews | **dark** | zero rows; team confirmed none exist |
| Post-purchase surveys | **dark** | zero rows |
| Competitor ad library | **dark** | no brands tracked; branch deferred by user |
| Northbeam | not connected | read performance on Meta numbers |

**Account shape:** this is lead generation, not ecommerce. Zero purchases, 4,336 leads.
Every performance read runs on CPL and lead volume, never ROAS.

## Prompt ledger

### Phase 0 — Repo & Scaffold
- [x] Resolve brand and lock brand_id — done
- [x] Test every data surface — done
- [x] Scaffold flat layout — done
- [x] Mount factory method at `parker-system/` (pinned v15) — done
- [x] Write `parker_config.json` — done
- [x] Ship executable layer into `.claude/` — done (26 skills, 2 agents, 2 scripts, voice layer)
- [x] Establish save path — done (self-managed in `insuranceyeti/creativeyeti`)

### Phase 1A — Brand foundation (14)
- [ ] brand-identity-analysis
- [ ] category-and-market-research
- [ ] community-and-forums
- [ ] competitive-landscape
- [ ] customer-journey-and-persona-discovery
- [ ] marketing-calendar-and-campaigns
- [ ] operations-and-team
- [ ] reputation-analysis
- [ ] visual-vocabulary
- [ ] website-and-product-audit
- [ ] ad-account-evaluation (blocked on 1E)
- [ ] performance-targets-and-metrics (blocked on 1E)
- [ ] organic-channels-inventory (blocked on 1E)
- [ ] brand-profile-narrative (synthesis of all A)

### Phase 1B — Competitor profiles
- DEFERRED at user's request. No competitors tracked in the Parker app.
  Add rivals there and this branch backfills without redoing anything.

### Phase 1C — Persona source pulls (12)
- [ ] source: ad-account
- [ ] source: ad-comments
- [ ] source: customer-reviews (will run data-limited — surface is dark)
- [ ] source: other-reviews
- [ ] source: post-purchase-surveys (will run data-limited — surface is dark)
- [ ] source: reddit
- [ ] source: brand-reputation
- [ ] source: brand-self-echo-detection
- [ ] personas-profile (synthesis)
- [ ] persona-voice-library
- [ ] lifecycle-journey-maps
- [ ] cross-persona-bias-notes

### Phase 1D — Voice of customer (12)
- [ ] voc-corpus-profile
- [ ] voc-pain-phrase
- [ ] voc-outcome-phrase
- [ ] voc-objection
- [ ] voc-trigger-moment
- [ ] voc-metaphor
- [ ] voc-aspirational
- [ ] voc-anti-language
- [ ] voc-category-jargon
- [ ] voc-surprise-delight
- [ ] voc-corpus (assembly inputs)
- [ ] voice-of-customer-assembly

### Phase 1E — Audit baseline, internal (11)
- [ ] 90-day-creative-strategy-audit (anchor)
- [ ] 90-day-performance-audit
- [ ] 90-day-diversity-audit
- [ ] customer-review-audit (will run data-limited)
- [ ] quarterly-whitespace-analysis
- [ ] monthly-hook-audit
- [ ] monthly-performance-report
- [ ] monthly-organic-tiktok-audit
- [ ] monthly-tiktok-mining
- [ ] biweekly-iterations-report
- [ ] weekly-performance-snapshot

### Phase 1E — Audit baseline, external (6)
- DEFERRED with the competitor branch.

### Phase 1 — Synthesis (2)
- [ ] gaps-opportunities-inspo
- [ ] open-loops-roll-up

### Phase 2 — Strategy (5)
- [ ] persona-strategy-input
- [ ] product-priority
- [ ] messaging-strategy-input
- [ ] creator-talent-strategy-input
- [ ] strategic-roadmap

### Phase 3 — Ideation (4)
- [ ] brand-idea-bank
- [ ] idea-evaluation
- [ ] sprint-plan
- [ ] brief-creation

### Finish (4)
- [ ] Stamp operating contract (CLAUDE.md, README.md, brand-lens, refresh-schedule)
- [ ] Verify build
- [ ] Confirm save
- [ ] Hand off to /get-started

## Needs attention

1. **Managed Parker storage was unreachable** from the build session, so this brain is
   self-managed. `parker-brain/insuranceyeti-health-for-moms` was provisioned but is empty.
   Details and the migration path are in `running-notes/standard-sync.md`.
2. **Reviews and surveys are dark.** Voice-of-customer will lean on ad comments, Reddit,
   and competitor reviews instead, per the team's own guidance in Slack. Every VoC claim
   sourced that way is labelled accordingly.
3. **Competitors deferred.** External audit cuts skipped with them.

## What happens next

Run Phase 1: the internal audit baseline first, then the brand foundation slices, persona
source pulls, and voice of customer.
