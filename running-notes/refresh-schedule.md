# Refresh schedule — Health For Moms

This is the one place that tracks when every standing doc was last run and when it is due to be re-run. Each doc's own `generated_on` and `refresh_by` frontmatter is the source of truth; this file aggregates them so the whole brain's freshness reads at a glance instead of opening every doc. The cadence policy — which doc type refreshes how often, and the real-world triggers that override the calendar — lives in `parker-system/system/refresh-cadence.md`.

**Built:** 2026-09-05, from the frontmatter of all 51 standing docs.

## How Parker uses this

- When you load this brain or lean on a standing doc, read this schedule and compare each due date to today. A doc past its due date is overdue; one inside roughly two weeks of it is due soon.
- Surface what is overdue or due soon plainly, and offer to re-run the generating prompt by name — "your weekly snapshot is from September 4th and it's now the 20th, want me to refresh it." Do not silently keep using a doc past its date, and do not re-run without surfacing the recommendation first.
- A refresh is a re-run of the doc's own generating prompt in `parker-system/prompts/`. It takes the prior version as context, carries forward what is still true, and re-stamps both dates. After a re-run, update that doc's line here.
- **The triggers in `parker-system/system/refresh-cadence.md` outrank the calendar.** A rebrand, a new SKU, a pricing move, a new competitor, an attribution change, or a validated finding that changes the read makes a doc due early regardless of the date below. When a trigger has fired, flag the doc as due now and name the trigger.
- When two or more sub-context slices have been re-run, `sub-context-docs/brand-profile-narrative.md` is due regardless of its own date, because it is a synthesis of them.

## Live triggers already firing for this brand

Three things are set to move dates early, and they are named here so nobody has to rediscover them.

1. **Open Enrollment opens 2026-11-01.** The roadmap is deliberately set to 2026-11-01 rather than its natural 2026-12-03 because of it. `seasonality.md` is explicit that a season moves the buyer and the angle, not just the offer.
2. **The enhanced ACA subsidies expire 2026-01-01.** The larger structural event, bigger than Open Enrollment itself. Anything reading the category or the calendar is due early as that approaches.
3. **Roadmap approval.** The roadmap is still `drafted, awaiting review`. When the team approves or adjusts it, `idea-bank/evaluation-2026-09-04.md` is due immediately, because the rank was built on it.

## The schedule, by cadence

### Quarterly — roughly 90 days

- `sub-context-docs/ad-account-evaluation.md` — last run 2026-09-04 — due **2026-12-03**
- `sub-context-docs/performance-targets-and-metrics.md` — last run 2026-09-04 — due **2026-12-03**
- `sub-context-docs/organic-channels-inventory.md` — last run 2026-09-04 — due **2026-12-03**
- `sub-context-docs/competitive-landscape.md` — last run 2026-09-04 — due **2026-12-03**
- `sub-context-docs/visual-vocabulary.md` — last run 2026-09-04 — due **2026-10-04** (shortened from the standard 90 days by the doc itself)
- `sub-context-docs/marketing-calendar-and-campaigns.md` — last run 2026-09-04 — due **2026-11-15**
- `strategy/persona-strategy-input.md` — last run 2026-09-04 — due **2026-11-01**
- `strategy/product-priority.md` — last run 2026-09-04 — due **2026-10-15**
- `strategy/messaging-strategy-input.md` — last run 2026-09-04 — due **2026-11-01**
- `strategy/creator-talent-strategy-input.md` — last run 2026-09-04 — due **2026-11-01**
- `strategy/strategic-roadmap.md` — last run 2026-09-04 — due **2026-11-01** (Open Enrollment trigger, pulled forward from 2026-12-03)

### Semi-annual — roughly 180 days

- `sub-context-docs/reputation-analysis.md` — last run 2026-09-04 — due **2026-12-05**
- `sub-context-docs/customer-journey-and-persona-discovery.md` — last run 2026-09-03 — due **2027-03-02**
- `sub-context-docs/category-and-market-research.md` — last run 2026-09-03 — due **2026-11-15** (pulled forward; the subsidy expiry and the enforcement record both move)
- `sub-context-docs/community-and-forums.md` — last run 2026-09-04 — due **2026-10-04**
- `sub-context-docs/website-and-product-audit.md` — last run 2026-09-03 — due **2026-11-01**
- `personas/personas-profile.md` — last run 2026-09-04 — due **2026-10-04**
- `personas/persona-voice-library.md` — last run 2026-09-04 — due **2026-10-04**
- `personas/lifecycle-journey-maps.md` — last run 2026-09-04 — due **2026-10-04**
- `personas/cross-persona-bias-notes.md` — last run 2026-09-04 — due **2026-10-04**
- `personas/voice-of-customer/voice-of-customer.md` — the assembly; carries no dates of its own, refreshes with its slices below
- `personas/voice-of-customer/voc-corpus-profile.md` — last run 2026-09-03 — due **2026-10-03**
- `personas/voice-of-customer/voc-pain-phrase.md`, `voc-outcome-phrase.md`, `voc-objection.md`, `voc-trigger-moment.md`, `voc-metaphor.md`, `voc-aspirational.md`, `voc-anti-language.md`, `voc-category-jargon.md`, `voc-surprise-delight.md` — all last run 2026-09-04 — all due **2026-10-04**

**Note on the persona cadence.** Every persona and voice-of-customer doc here sits on a 30-day clock rather than the standard 180, because the corpus is thin and one-sided. The only first-party surface is ad comments, so the personas refresh as fast as new comments arrive.

### Annual — roughly 365 days

- `sub-context-docs/brand-identity-analysis.md` — last run 2026-09-03 — due **2027-03-03**
- `sub-context-docs/operations-and-team.md` — last run 2026-09-04 — due **2026-12-04** (shortened; the team's tools came online mid-build and have not been read in)

### Source pulls — the raw evidence under the personas

- `source-pulls/ad-account.md` — last run 2026-09-03 — due **2026-10-03**
- `source-pulls/ad-comments.md` — last run 2026-09-03 — due **2026-10-03**
- `source-pulls/brand-self-echo-detection.md` — last run 2026-09-03 — due **2026-10-03**
- `source-pulls/reddit.md` — last run 2026-09-03 — due **2026-10-03** (honest blank; Reddit was unreachable)
- `source-pulls/customer-reviews.md` — last run 2026-09-04 — due **2026-10-04** (verified empty surface)
- `source-pulls/post-purchase-surveys.md` — last run 2026-09-04 — due **2026-10-04** (verified empty surface)
- `source-pulls/other-reviews.md` — last run 2026-09-04 — due **2026-10-04**
- `source-pulls/brand-reputation.md` — last run 2026-09-04 — due **2026-12-03**

### Event-driven — no calendar date, re-run when the trigger fires

- `sub-context-docs/brand-profile-narrative.md` — last run 2026-09-04, backstop due **2026-10-04**. Refreshes whenever two or more of its input slices do.
- `idea-bank/evaluation-2026-09-04.md` — last run 2026-09-04. **Due immediately on roadmap approval or adjustment.** Also triggered when the bank grows enough to change the rank, when the roadmap's own 2026-11-01 date lands, or when any of the brand-routed questions C1, E1, B1 or B3 is answered — each moves several positions.
- `idea-bank/index.md` — last run 2026-09-04. Captured continuously by the weekly hunt; no fixed date.
- `open-loops/open-loops-roll-up.md` — last run 2026-09-04 — due **2026-10-04**, and re-run by the weekly research cycle whenever loops resolve.
- Competitor rotation — **not applicable yet.** No rivals tracked; the branch is deferred at the team's request.

### Audit cadence

- `audits/2026-Q3/90-day-creative-strategy-audit.md` (anchor) — last run 2026-09-03 — due **2026-10-15**
- `audits/2026-Q3/90-day-performance-audit.md` — last run 2026-09-03 — due **2026-12-02**
- `audits/2026-Q3/90-day-diversity-audit.md` — last run 2026-09-03 — due **2026-12-02**
- `audits/2026-Q3/customer-review-audit.md` — last run 2026-09-04 — due **2026-10-04** (ran data-limited; reviews are empty)
- `audits/2026-Q3/quarterly-whitespace-analysis.md` — last run 2026-09-04 — due **2026-12-03**
- `audits/2026-Q3/gaps-opportunities-inspo.md` — last run 2026-09-04 — due **2026-12-03**
- `audits/2026-09/monthly-hook-audit.md` — last run 2026-09-03 — due **2026-10-03**
- `audits/2026-09/monthly-performance-report.md` — last run 2026-09-03 — due **2026-10-03**
- `audits/2026-09/monthly-organic-tiktok-audit.md` — last run 2026-09-04 — due **2026-10-04**
- `audits/2026-09/monthly-tiktok-mining.md` — last run 2026-09-04 — due **2026-10-04**
- `audits/2026-09/biweekly-iterations-report.md` — last run 2026-09-04 — due **2026-09-18**
- `audits/2026-09/weekly-performance-snapshot.md` — last run 2026-09-04 — due **2026-09-11**
- External audit cuts — **deferred with the competitor branch.** Six cuts, none built.

### Exempt — self-cadenced or always-on

- The idea bank is captured continuously. Briefs are per-campaign artifacts and are not refreshed.
- `running-notes/brand-rules.md`, `success-definition.md`, `missing-context.md`, `standard-sync.md` — updated as facts change, not on a clock.
- `brand-lens.md` — grows continuously as the brand teaches Parker something durable. No due date.

## Nothing is overdue as of 2026-09-05

The soonest two are `weekly-performance-snapshot.md` on 2026-09-11 and `biweekly-iterations-report.md` on 2026-09-18. The weekly refresh routine will catch both.
