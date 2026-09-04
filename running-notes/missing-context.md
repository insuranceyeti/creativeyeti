# Missing context — the open questions

What Parker could not observe, could not reach, or was not told. Every entry here is an open
question, never a blocker. Prompts that hit one of these must label the affected claim
`data-limited` and say so plainly rather than filling the gap with a guess.

**Generated:** 2026-09-03 (Phase 0 surface test)

## Dark data surfaces — confirmed empty, not broken

These were tested with real pulls during Phase 0. They returned zero rows.

- **Customer reviews** — zero rows. The team confirmed this directly in Slack on 2026-09-03:
  *"we don't have reviews but you can pull from competitor reviews or health insurance Reddit etc."*
  **Substitution rule for this brand:** wherever a prompt calls for customer-review evidence, use
  Facebook ad comments (live and rich), Reddit, and competitor/category reviews instead, and label
  the source explicitly. Never present substituted evidence as this brand's own review corpus.
- **Post-purchase surveys** — zero responses. No survey platform connected and no CSV uploaded.
- **Competitor ad library** — no external brands tracked in the Parker app. The competitor branch
  and the external audit cuts are **deferred at the user's request** (2026-09-03), not failed.
  Adding rivals in the Parker app backfills this branch without redoing anything else.
- **Northbeam** — not connected. All attribution is Meta-reported. Read performance on Meta
  numbers and say so; do not imply multi-touch attribution.

## Live surfaces — for contrast

Brand context document, Meta ads (`HealthForMoms`, act `484897827497337`), Facebook ad comments,
the TikTok mining library (23 relevancy-scored videos), and Parker chat history (4 threads,
1 web + 3 Slack).

## Account shape — read this before any performance analysis

**This account is lead generation, not ecommerce.** Last 90 days: 136 ads, $98,276.68 spend,
**4,336 leads at $22.67 CPL**, and **zero purchases**. ROAS is 0 across the board because there
is no purchase event, not because the ads fail.

- Judge performance on **CPL, lead volume, CPM, CTR, hook rate and hold rate**. Never on ROAS,
  AOV, or purchase value.
- Audience skew is sharp: **95.2% female**, **81.2% aged 25-44**, **99.5% mobile**,
  60% Facebook / 39% Instagram.
- The business model is a match-and-consult referral to partner insurance agencies, not a
  direct sale, so "conversion" means a qualified lead handed to an agent.

## Brand intake — not yet captured

The Phase 0 brand intake was not run before the build began. These remain open until the team
answers them, and the build proceeds without them.

- Main business objective right now
- Primary campaign objective
- North-star metric and whether hitting its goal is the whole definition of success
- Secondary metrics they still weigh
- Whether higher spend wins when two ads in one ad set diverge
- Where they read performance (in-platform vs a third-party tool)
- Ad naming convention
- Brief template (would be saved verbatim to `briefs/_brief-template.md`)
- Who they consider real competitors, plus aspirational brands
- Unit economics: customer value, gross margin, LTV or payback window, max tolerable CPA

## Operational breaks the brain found but cannot fix — for the team, not for Parker

These are not research questions. Each one is a thing that is wrong right now, on live spend, and it needs an owner outside this brain.

### The quiz destination does not register arrivals — found 2026-09-04, urgent

`moms-53 3 - Copy` (three variants, `ADSET_PAUSED` today) points at **`quiz.healthformoms.com/#/indvfam`** and returned **9 landing page views against 511 link clicks** across 2026-06-06 to 2026-09-03 — a click quality of **1.76%**. Its sibling `moms-53 3` carries the **same creative, same hook, same body copy**, points at `www.healthformoms.co/save/` instead, and returns **76.12%**. `verified live`, `search_facebook_ads_sql`, 2026-09-04, Meta default attribution.

**Two possible causes and the data cannot separate them.** Either almost nobody who clicks actually lands on the quiz, or they land and the pixel does not fire on that domain. The first is lost spend; the second is blind measurement on every quiz-pointed ad this account has ever run. Both are urgent and neither is a creative problem.

**What it blocks:** no brief may be built on a figure sourced from a `quiz.healthformoms.com` ad until this is settled, because every conversion rate on those ads is currently unreadable.

**Who can answer it:** whoever owns the website and the Meta pixel. Parker cannot see server logs or pixel configuration.

This is the same shape as the `go.healthformoms.co` redirect break the open-loops roll-up routed to the operational owner on 2026-09-04, on a different destination. Two destination problems found independently is a pattern worth a single audit of every landing URL in the account rather than two one-off fixes.
