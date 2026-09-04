---
brand: Health For Moms
doc: hypothesis
source_loop: roll-up archived kill 1 — "What happens to a click that lands on `go.healthformoms.co/save/`?" (raised by operations-and-team.md 1, website-and-product-audit.md 2, monthly-hook-audit.md 6; killed on reason 5, infrastructure)
territory: Product
score: inherited — reopened, not re-graded
state: proceeding
last_updated: 2026-09-04
---

# Hypothesis — the landing-page-view collapse on `go.healthformoms.co` is a tracking artifact, not nine in ten clicks evaporating

## Reopening note

The consolidated roll-up archived this question on kill reason 5 — infrastructure — with the verdict "the destination leaks." That archive requires new evidence citing its reasoning before revival, and there is some: the kill was written off landing-page views and cost per lead, and the same 40 ads contain `Yeti State Angle - 1 - V3` at 800 link clicks, 92 landing page views and **80 leads at $14.70**. An ad that lost nine of ten clicks cannot produce 80 leads. The archived verdict may be right, but it was not established on evidence that could distinguish a broken destination from a broken counter, so it is reopened here rather than re-litigated blind.

This brand has already had one confident wrong conclusion about this exact destination — the quiz misattribution corrected 2026-09-04 and logged in `prompts-run-log/2026-09-03-full-buildout.md`. That correction is the reason this hypothesis is built around a metric that cannot be contaminated by the suspect one.

## The prediction

Parker's bet: **the landing-page-view number on `go.healthformoms.co/save/` is undercounting arrivals, not reporting them.** If that is right, the clicks are not lost, the `$32.79` blended cost per lead across those 40 ads is a real cost per lead rather than a measurement error, and the ads that look catastrophic look that way for some reason other than the destination. Marked as **inferred** — it inherits the loop's uncertainty and is a hypothesis, never a fact.

The falsifier is explicit: if leads-per-link-click on `go.` is genuinely far below `www.` for the same creative, the prediction is wrong and there is real funnel loss.

## The test

**1. The decisive pull — leads per link click, computed by hand.** `search_facebook_ads_sql`, `groupBy: "ad"`, `metricsMode: "lifetime_only"`, `filters: [{field:"landing_url", operator:"contains", value:"go.healthformoms"}]`, `metricSets: ["traffic","funnel","costs"]`, paginated to all 40 ads. Landing page views are the suspect metric, so they are **barred as a denominator**. Leads ÷ link clicks bypasses the suspect counter entirely: link clicks are counted on Meta's side of the boundary, leads are counted at the far end, and neither depends on the page-view pixel. Parker's own `click_to_leads` field is **not** this ratio — it divides by all clicks — so the ratio is computed by hand from the raw counts. Same pull run against `www.healthformoms.co/save/` for the comparison.

**2. Matched pairs by `media_hash`.** Add `include: ["extended"]` to both pulls and find every creative file that ran to both destinations. This controls for creative quality completely — same video, same copy, same hook — and is the cleanest evidence the account can produce. Compare each pair on leads per link click.

**3. The confound the prediction could be hiding behind.** The good `go.` performers sit in `Internal - ABO - TEST` and the bad ones in `USHA - CBO - OTP`. Pull the whole `USHA - CBO - OTP` campaign across all destinations, and pull `www.` ads created since 2026-08-01. If that campaign converts badly on destinations other than `go.`, the destination is exonerated and the campaign is the cause; if recent `www.` ads convert normally, a general August-onward account problem is ruled out.

**4. The time dimension.** `go.` ads exist from 2026-03-13 and from 2026-08-17 onward. Split the cohort on creation date and read each half separately, because a destination that broke on a date would show exactly that seam.

**5. What `click_quality` actually is.** Reproduce the reported score arithmetically from the raw counts on several ads across both domains. If it equals landing page views ÷ link clicks, it is the suspect metric wearing a second name, it is **not** independent corroboration, and every prior document that cited it as a second witness was citing the same witness twice. `ad-metrics-glossary.md` has no entry for it, so it is derived from the numbers rather than looked up.

**The disconfirming read, inside the same pulls.** Leads per landing page view is the reverse lens and it is read as hard as the forward one. Across `www.` the account converts arrivals to leads at roughly 8–14%. If a `go.` cohort shows a leads-per-arrival rate inside that band, its landing-page-view count is behaving like a real number and the prediction fails for that cohort; if it shows an impossible rate — more leads than the page supposedly received could plausibly produce — the counter is undercounting and the prediction holds.

## What each outcome would mean

**Validated.** Leads per link click on `go.` sits within normal distance of `www.` for matched creative across the cohort, and leads-per-arrival on `go.` is implausibly high. The collapse is a counter problem; the ads are not losing clicks; the archived "leaks" verdict is corrected.

**Invalidated.** Leads per link click on `go.` is far below `www.` for the same creative files, and leads-per-arrival on `go.` sits in the normal 8–14% band. Then the landing-page-view number is telling the truth, the clicks really are being lost before the page, and the archived verdict stands.

**Inconclusive.** The cohort splits — some `go.` ads convert normally per link click and others collapse — so both readings are true of different ads and the single prediction does not describe the destination. Or the collapse is real but campaign, date and destination are collinear in the data, so the cause cannot be assigned. Evidence is plentiful; it points both ways.

**Insufficient evidence.** The `go.` ads carry too few leads and too little spend to separate signal from noise at all.

## Binding constraints carried into the run

Lead-gen, zero purchases: never ROAS, AOV or purchase value. A winner is two-gated — cost per lead then lead quality — and Parker cannot see gate two (42 `Call` events against 4,336 leads), so no ad on either destination gets called a winner on cost per lead alone, whatever this finding says.
