# Refresh schedule — Health For Moms

This is the one place that tracks when every standing doc was last run and when it is due to be re-run. Each doc's own `generated_on` and `refresh_by` frontmatter is the source of truth; this file aggregates them so the whole brain's freshness can be read at a glance instead of opening every doc. The cadence policy — which doc type refreshes how often, and the real-world triggers that override the calendar — lives in `parker-system/system/refresh-cadence.md`.

**Generated 2026-09-04** at the stamp step of the initial build, by reading the frontmatter of all 56 standing docs on disk.

**One note on how this file is organized.** Several docs carry a `refresh_by` that is shorter or longer than the template's default bucket for their type — the persona set and `visual-vocabulary.md` came back monthly rather than semi-annual, `reputation-analysis.md` and `operations-and-team.md` came back quarterly, and five docs were pulled early to land before Open Enrollment opens on 2026-11-01. **The doc's own frontmatter governs and this file follows it.** Where a doc sits in a bucket other than its template default, the line says so.

## How Parker uses this

- When you load this brain or consult a standing doc, read this schedule and compare each `due` date to today from `get_current_time`. A doc whose due date has passed is overdue; one inside roughly two weeks of its due date is due soon.
- Surface what is overdue or due soon plainly, and offer to re-run the generating prompt by name — "your ad-account read is from March and it is now July, want me to refresh it." Do not silently keep using a doc past its due date, and do not re-run without surfacing the recommendation first.
- A refresh is a re-run of the generating prompt. It takes the prior version as context, carries forward what is still true, and re-stamps `generated_on` and `refresh_by`. After a re-run, update that doc's line in this schedule to the new dates, and append one entry to `running-notes/routine-log.md`.
- The triggers in `parker-system/system/refresh-cadence.md` outrank the calendar. A rebrand, a new SKU, a pricing move, a new competitor, an attribution change, or a validated finding that changes the read makes a doc due early regardless of the date here. When a trigger has fired, flag the doc as due now and note the trigger.
- When two or more sub-context slices have been re-run, `sub-context-docs/brand-profile-narrative.md` is due regardless of its own date, because it is a synthesis of them.

## Standing triggers already known for this brand

- **Open Enrollment opens 2026-11-01.** Five docs were deliberately dated to land before it rather than on their normal interval: `strategy/strategic-roadmap.md`, `strategy/persona-strategy-input.md`, `strategy/messaging-strategy-input.md`, `strategy/creator-talent-strategy-input.md`, and `sub-context-docs/website-and-product-audit.md`, plus `category-and-market-research.md` and `marketing-calendar-and-campaigns.md` at 2026-11-15. A season can move the buyer and the angle here, not just the offer.
- **The roadmap is unapproved.** `strategy/strategic-roadmap.md` carries `status: drafted, awaiting review`. It is due early if the team approves it, rejects it, or reorders the priorities.
- **Tier-1 loop 1 resolving** — what this audience believes she can change about her own coverage — makes the roadmap and both persona docs due regardless of date.
- **Gate two opening.** If the partner agencies ever hand over lead-quality data, every performance doc in this brain is due, because every read in it currently clears gate one only.
- **Competitors being added in the Parker app** makes `sub-context-docs/competitive-landscape.md` and the whole deferred external-audit branch due immediately.

## Due now or due soon, as of 2026-09-04

- **Nothing is overdue.** The brain was built 2026-09-03 and 2026-09-04.
- **Due soon:** `audits/2026-09/weekly-performance-snapshot.md` on 2026-09-11, and `audits/2026-09/biweekly-iterations-report.md` on 2026-09-18.

## The schedule, by cadence

### Weekly and biweekly

- `audits/2026-09/weekly-performance-snapshot.md` — last run 2026-09-04 — due 2026-09-11 (+7d)
- `audits/2026-09/biweekly-iterations-report.md` — last run 2026-09-04 — due 2026-09-18 (+14d)

### Monthly — roughly 30 days

- `sub-context-docs/brand-profile-narrative.md` — last run 2026-09-04 — due 2026-10-04. Also event-driven; see below.
- `sub-context-docs/community-and-forums.md` — last run 2026-09-04 — due 2026-10-04
- `sub-context-docs/visual-vocabulary.md` — last run 2026-09-04 — due 2026-10-04 *(template default is quarterly; the doc set itself monthly)*
- `personas/personas-profile.md` — last run 2026-09-04 — due 2026-10-04 *(template default is semi-annual; the doc set itself monthly)*
- `personas/persona-voice-library.md` — last run 2026-09-04 — due 2026-10-04
- `personas/lifecycle-journey-maps.md` — last run 2026-09-04 — due 2026-10-04
- `personas/cross-persona-bias-notes.md` — last run 2026-09-04 — due 2026-10-04
- `personas/voice-of-customer/voc-pain-phrase.md` — last run 2026-09-04 — due 2026-10-04
- `personas/voice-of-customer/voc-outcome-phrase.md` — last run 2026-09-04 — due 2026-10-04
- `personas/voice-of-customer/voc-objection.md` — last run 2026-09-04 — due 2026-10-04
- `personas/voice-of-customer/voc-trigger-moment.md` — last run 2026-09-04 — due 2026-10-04
- `personas/voice-of-customer/voc-metaphor.md` — last run 2026-09-04 — due 2026-10-04
- `personas/voice-of-customer/voc-aspirational.md` — last run 2026-09-04 — due 2026-10-04
- `personas/voice-of-customer/voc-anti-language.md` — last run 2026-09-04 — due 2026-10-04
- `personas/voice-of-customer/voc-category-jargon.md` — last run 2026-09-04 — due 2026-10-04
- `personas/voice-of-customer/voc-surprise-delight.md` — last run 2026-09-04 — due 2026-10-04
- `personas/voice-of-customer/voc-corpus-profile.md` — last run 2026-09-03 — due 2026-10-03
- `source-pulls/ad-account.md` — last run 2026-09-03 — due 2026-10-03
- `source-pulls/ad-comments.md` — last run 2026-09-03 — due 2026-10-03
- `source-pulls/brand-self-echo-detection.md` — last run 2026-09-03 — due 2026-10-03
- `source-pulls/reddit.md` — last run 2026-09-03 — due 2026-10-03. Surface unreachable at build; the doc is an honest named blank.
- `source-pulls/customer-reviews.md` — last run 2026-09-04 — due 2026-10-04. Surface verified empty; honest named blank.
- `source-pulls/other-reviews.md` — last run 2026-09-04 — due 2026-10-04
- `source-pulls/post-purchase-surveys.md` — last run 2026-09-04 — due 2026-10-04. Surface verified empty; honest named blank.
- `open-loops/open-loops-roll-up.md` — last run 2026-09-04 — due 2026-10-04
- `audits/2026-09/monthly-hook-audit.md` — last run 2026-09-03 — due 2026-10-03 (+30d)
- `audits/2026-09/monthly-performance-report.md` — last run 2026-09-03 — due 2026-10-03 (+30d)
- `audits/2026-09/monthly-organic-tiktok-audit.md` — last run 2026-09-04 — due 2026-10-04 (+30d)
- `audits/2026-09/monthly-tiktok-mining.md` — last run 2026-09-04 — due 2026-10-04 (+30d)
- `audits/2026-Q3/customer-review-audit.md` — last run 2026-09-04 — due 2026-10-04. Ran data-limited; the review surface is empty.

### Quarterly — roughly 90 days

- `sub-context-docs/ad-account-evaluation.md` — last run 2026-09-04 — due 2026-12-03
- `sub-context-docs/performance-targets-and-metrics.md` — last run 2026-09-04 — due 2026-12-03
- `sub-context-docs/organic-channels-inventory.md` — last run 2026-09-04 — due 2026-12-03
- `sub-context-docs/competitive-landscape.md` — last run 2026-09-04 — due 2026-12-03
- `sub-context-docs/operations-and-team.md` — last run 2026-09-04 — due 2026-12-04 *(template default is annual; the doc set itself quarterly)*
- `sub-context-docs/reputation-analysis.md` — last run 2026-09-04 — due 2026-12-05 *(template default is semi-annual; the doc set itself quarterly)*
- `audits/2026-Q3/90-day-creative-strategy-audit.md` (anchor) — last run 2026-09-03 — due 2026-10-15. Pulled early ahead of Open Enrollment rather than the standard +90d.
- `audits/2026-Q3/90-day-performance-audit.md` — last run 2026-09-03 — due 2026-12-02 (+90d)
- `audits/2026-Q3/90-day-diversity-audit.md` — last run 2026-09-03 — due 2026-12-02 (+90d)
- `audits/2026-Q3/quarterly-whitespace-analysis.md` — last run 2026-09-04 — due 2026-12-03 (+90d)
- `audits/2026-Q3/gaps-opportunities-inspo.md` — last run 2026-09-04 — due 2026-12-03 (+90d)

### Pulled early for Open Enrollment — 2026-11-01

- `strategy/strategic-roadmap.md` — last run 2026-09-04 — due 2026-11-01. Also due early on approval, rejection, or a Tier-1 loop resolving.
- `strategy/persona-strategy-input.md` — last run 2026-09-04 — due 2026-11-01
- `strategy/messaging-strategy-input.md` — last run 2026-09-04 — due 2026-11-01
- `strategy/creator-talent-strategy-input.md` — last run 2026-09-04 — due 2026-11-01
- `strategy/product-priority.md` — last run 2026-09-04 — due 2026-10-15
- `sub-context-docs/website-and-product-audit.md` — last run 2026-09-03 — due 2026-11-01
- `sub-context-docs/category-and-market-research.md` — last run 2026-09-03 — due 2026-11-15
- `sub-context-docs/marketing-calendar-and-campaigns.md` — last run 2026-09-04 — due 2026-11-15

### Semi-annual — roughly 180 days

- `sub-context-docs/brand-identity-analysis.md` — last run 2026-09-03 — due 2027-03-03 *(template default is annual; the doc set itself semi-annual)*
- `sub-context-docs/customer-journey-and-persona-discovery.md` — last run 2026-09-03 — due 2027-03-02
- `source-pulls/brand-reputation.md` — last run 2026-09-04 — due 2026-12-03
- `personas/voice-of-customer/voice-of-customer.md` — last run 2026-09-04 — due 2027-03-04. **Flag:** this doc carries `last_updated` rather than `generated_on` / `refresh_by`, so the due date here is assigned from the semi-annual default, not read from the file. Stamp proper frontmatter on its next re-run.

### Event-driven — no calendar date, re-run when the trigger fires

- `sub-context-docs/brand-profile-narrative.md` — refreshes when two or more of its input slices do, with a 30-day floor as its own frontmatter sets. Last run 2026-09-04.
- `idea-bank/evaluation-[YYYY-MM-DD].md` — re-run when the bank grows enough to change the rank or when the roadmap is re-approved. Built 2026-09-04 as part of Phase 3.
- `hypotheses/`, `validations/`, `re-validations/` — driven by the loop pipeline in `/research-loops`, not by this calendar. One hypothesis and one validation exist, both 2026-09-04, both on the `go.` subdomain measurement question, resolved inconclusive.
- Competitor rotation — **deferred for this brand.** No rivals are tracked in the Parker app except Ethos, which sells term life and is not in this category. Adding rivals there makes `competitive-landscape.md` and the external audit branch due immediately.

### Deferred — not built, so nothing to refresh

- `competitors/` — the whole per-rival branch, deferred at the team's request.
- `audits/2026-Q3/external/` and `audits/2026-09/external/` — all six external cuts, deferred with the competitor branch.

### Exempt — self-cadenced or always-on, no entry needed

- The idea bank is captured continuously; briefs are per-campaign artifacts, not refreshed.
- `running-notes/` and `brand-lens.md` grow by append as the brand teaches Parker something durable. `standard-sync.md` is driven by `/update-brain`, not by date.
