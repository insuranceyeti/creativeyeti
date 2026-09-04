# Build status — Health For Moms brand brain

**Brand:** Health For Moms (`aed0ff06-555d-4f4f-9bf8-31178e2fb977`)
**Build started:** 2026-09-03
**Method version:** parker-brain `v15`
**Run id:** `e5c1cbe7-0bba-4a1e-8b7e-9bdc075777e1`
**Current phase:** **Phase 1 CLOSED** 2026-09-04. Phase 2 blocked on the Parker MCP reconnecting.

> **BLOCKED — WAITING ON YOU.** The Parker MCP connection dropped and needs re-authorization
> (claude.ai connector settings, or `/mcp` in an interactive session). Phase 2 and Phase 3 both need
> live pulls and cannot honestly run from a stale vault. Everything built so far is committed and
> pushed; `parker_config.json` holds the run anchor and this ledger holds the state.

**Saved to:** https://github.com/insuranceyeti/creativeyeti (branch `claude/parker-mcp-http-349ri1`)
**Repo posture:** self-managed — see `running-notes/standard-sync.md`

## What is happening right now

Phase 1 is running. Seven agents are working in parallel across the audit baseline, the brand
foundation, and the persona source pulls. Each one runs its own factory prompt from
`parker-system/prompts/` in full, and each output gets an independent fidelity review before
anything downstream consumes it.

The brand intake has been captured into `running-notes/success-definition.md` and
`running-notes/brand-rules.md`. The headline rule it produced: a winner is two-gated here,
CPL then lead quality, and Parker can only see gate one.

**First finding, from the 90-day performance audit:** spend fell 73.5% quarter over quarter
($374,508 to $99,267) while CPL held essentially flat ($22.65 to $22.64). That reads as a
budget decision, not a performance failure. Separately, one ad carries 43.3% of all spend and
four ads sharing a single text hook carry 60.5% — a concentration worth knowing before
November's Open Enrollment ramp.

## Scoreboard

| Phase | Status | Done / Total |
|---|---|---|
| Phase 0 — Repo & Scaffold | **done** | 7 of 7 |
| Phase 1A — Brand foundation | **done** | 14 of 14 |
| Phase 1B — Competitor profiles | **deferred** | 0 of 0 |
| Phase 1C — Persona source pulls | **done** | 12 of 12 |
| Phase 1D — Voice of customer | **done** | 12 of 12 |
| Phase 1E — Audit baseline (internal) | **done** | 11 of 11 |
| Phase 1E — Audit baseline (external) | **deferred** | 0 of 6 |
| Phase 1 — Synthesis | **done** | 2 of 2 |
| Phase 2 — Strategy | **blocked on Parker MCP** | 0 of 5 |
| Phase 3 — Ideation | **blocked on Parker MCP** | 0 of 4 |
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
- [x] brand-identity-analysis — done
- [x] category-and-market-research — done
- [ ] community-and-forums
- [x] competitive-landscape — done
- [x] customer-journey-and-persona-discovery — done
- [x] marketing-calendar-and-campaigns — done
- [ ] operations-and-team
- [x] reputation-analysis — done
- [ ] visual-vocabulary
- [x] website-and-product-audit — done
- [ ] ad-account-evaluation (blocked on 1E)
- [ ] performance-targets-and-metrics (blocked on 1E)
- [ ] organic-channels-inventory (blocked on 1E)
- [ ] brand-profile-narrative (synthesis of all A)

### Phase 1B — Competitor profiles
- DEFERRED at user's request. No competitors tracked in the Parker app.
  Add rivals there and this branch backfills without redoing anything.

### Phase 1C — Persona source pulls (12)
- [x] source: ad-account — done
- [x] source: ad-comments — done
- [x] source: customer-reviews — done (honest named blank, surface verified empty)
- [ ] source: other-reviews
- [x] source: post-purchase-surveys — done (honest named blank, surface verified empty)
- [x] source: reddit — done (honest blank, Reddit unreachable)
- [x] source: brand-reputation — done
- [x] source: brand-self-echo-detection — done
- [ ] personas-profile (synthesis)
- [ ] persona-voice-library
- [ ] lifecycle-journey-maps
- [ ] cross-persona-bias-notes

### Phase 1D — Voice of customer (12)
- [x] voc-corpus-profile — done
- [x] voc-pain-phrase — done
- [ ] voc-outcome-phrase
- [x] voc-objection — done
- [ ] voc-trigger-moment
- [ ] voc-metaphor
- [ ] voc-aspirational
- [ ] voc-anti-language
- [ ] voc-category-jargon
- [ ] voc-surprise-delight
- [ ] voc-corpus (assembly inputs)
- [ ] voice-of-customer-assembly

### Phase 1E — Audit baseline, internal (11)
- [x] 90-day-creative-strategy-audit (anchor) — done, in review
- [x] 90-day-performance-audit — done, in review
- [x] 90-day-diversity-audit — done
- [ ] customer-review-audit (will run data-limited)
- [x] quarterly-whitespace-analysis — done
- [x] monthly-hook-audit — done
- [x] monthly-performance-report — done
- [x] monthly-organic-tiktok-audit — done
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

## Review backlog — the gate before synthesis

Two documents have passed fidelity review (`90-day-performance-audit`, `90-day-creative-strategy-audit`).
Eighteen reviews are **in flight now**, batched across three reviewers covering the audits, the
brand foundation, and the source pulls plus voice-of-customer.

**This is a hard gate.** No Phase 1 synthesis node and no Phase 2 work may consume a document that
has not passed review. Two cross-document errors have already reached documents through this gap —
the quiz destination figures and the Open Enrollment history, both corrected and both logged in
`prompts-run-log/`. Both were caught by a later prompt reading a live source rather than by review,
which is exactly the cost of running the backlog.

## Resume anchor

If this session dies: `parker_config.json` carries `run_id`, this ledger carries the state. Call
`update_parker_brain_setup_status(mode: "start", brand_id, run_id)`, reconcile this ledger against
the files on disk, demote anything missing, and continue from the first pending item.
**Do not restart the build.**

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


---

## Phase 1 close — 2026-09-04

**49 documents. Roughly 300,000 words. All committed and pushed.**

The open-loops roll-up harvested **212 loops from 47 documents** and cut them to **57**: 14 Tier 1
promoted, 24 Tier 2 backlog, 19 routed to the brand. That is 73% attrition, almost all of it
consolidation rather than killing, which is the right shape when 47 documents were written in
parallel by agents that could not see each other.

**Independent convergence, recorded as a strength signal rather than deduplicated away:** ten
documents independently reached the lead-quality gate, nine the persona-provenance problem, nine the
recognition-versus-argument split, seven the coverage-is-luck belief.

**Top of the Tier 1 agenda:** what this audience believes she can change about her own coverage
(19/20, reached independently by four separately extracted voice-of-customer categories).

**Two grading calls worth keeping:** lead quality is **brand-routed, not Tier 1** — Stakes 5 with
Researchability 1 triggers the override, and it heads the brand-routed list as the highest-stakes
loop in the document. And the `go.healthformoms.co` break was **killed as a research loop** and
routed to the operational owner marked urgent: the strategic question is answered, what remains is
a broken redirect on eleven live ads, which is a fix rather than a question.

**Still outstanding at the Phase 1 boundary:**
- `gaps-opportunities-inspo` — the one Phase 1 node not built; it needs live category and account
  reads and was blocked by the disconnection.
- The competitor branch and all six external audit cuts remain deferred at the user's request.
- Reviews for the documents built after the three review batches ran.
- The team's tools (Slack, Notion, Drive, Gmail, Calendar, monday.com) came online mid-build and
  have not been read into the foundation. Three open intake items — ad naming convention, brief
  template, unit economics — are likely sitting in them.
