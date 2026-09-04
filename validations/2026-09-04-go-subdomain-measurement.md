---
brand: Health For Moms
doc: validation
source_loop: roll-up archived kill 1 — "What happens to a click that lands on `go.healthformoms.co/save/`?"
source_hypothesis: hypotheses/2026-09-04-go-subdomain-measurement.md
territory: Product
state: inconclusive
validated_on: 2026-09-04
revalidate_by: n/a — inconclusive findings do not enter the brand profile
---

# Validation — the `go.` cohort splits in two: one half's landing-page-view collapse is a pure counting artifact, the other half's lead collapse is real, and the cause of the second cannot be assigned · INCONCLUSIVE

## What we found

The prediction was that the landing-page-view collapse on `go.healthformoms.co/save/` is a tracking artifact and the clicks are not actually lost. **It is true of one half of the 40 ads and false of the other half, and the two halves are separated by campaign and creation date at once, which makes the cause of the second half unassignable from inside this account.**

The 40 `go.` ads are not one population. They fall into two creation clusters with no overlap: 24 ads created 2026-03-06 to 2026-03-13, and 16 ads created 2026-08-17 to 2026-08-31. The March cluster lives almost entirely in `Internal - ABO - TEST`; every August ad lives in `USHA - CBO - OTP`. Measured on leads per link click — the ratio that never touches the suspect metric — the March cluster is **healthy and indistinguishable from `www.`**, and the August cluster has **collapsed by an order of magnitude**.

Both clusters show the same wrecked landing-page-view number. So the landing-page-view collapse is not what separates a good `go.` ad from a bad one, and it never was. It has been present on that subdomain since at least March 2026, through a period when the ads on it were converting perfectly well.

One thing did resolve cleanly and firmly: **`click_quality` is landing page views divided by link clicks, times one hundred.** It is the suspect metric under a second name. Every prior build document that cited a click-quality score of 8–11 as corroboration for the landing-page-view collapse was citing the same measurement twice and calling it two witnesses.

## The evidence

**The decisive ratio, computed by hand.** Parker's `click_to_leads` field could not be used for this: it divides leads by *all* clicks, not link clicks. `Yeti State Angle - 1 - V3` reports `click_to_leads` 6.2, which is 80 leads ÷ 1,291 clicks, not 80 ÷ 800 link clicks. Confirmed on three more rows — 31 ÷ 527 = 5.88, 417 ÷ 4,490 = 9.29, 635 ÷ 12,050 = 5.27 — so every ratio below is computed from the raw `leads` and `link_clicks` counts.

**The March `go.` cohort converts normally.** Across the eight `Internal - ABO - TEST` ads on `go.` carrying leads, plus the eight trivial ones that carry none, the cohort took **2,854 link clicks and produced 248 leads — 8.69% leads per link click**. Ad by ad: `Yeti State Angle - 1 - V3` 80 leads on 800 link clicks (10.00%), `Yeti State Angle - 1 - V1` 50 on 439 (11.39%), `Yeti State Angle - 2 - V3` 19 on 160 (11.88%), `Yeti State Angle - 2 - V1` 31 on 353 (8.78%), `Yeti State Angle - 1 - V2` 39 on 544 (7.17%), `OMC-Health for Moms-[B3-C8-V5] - Copy` 10 on 108 (9.26%), `Yeti State Angle - 3 - V3` 15 on 278 (5.40%), `OMC - C11 - 2b` 4 on 92 (4.35%). Against `www.healthformoms.co/save/` lifetime — **30,702 leads on 288,916 link clicks, 10.63%** — and against `www.` ads created since 2026-08-01 — **1,192 leads on 12,551 link clicks, 9.50%** — the March `go.` cohort is normal. **Verified**, ad-level lifetime pulls 2026-09-04.

**The August `go.` cohort has collapsed.** The `USHA - CBO - OTP` ads on `go.` took **2,196 link clicks and produced 18 leads — 0.82%**. `Moms Nahuel WV#1 - V9 - Copy` 6 leads on 690 link clicks (0.87%), `moms-63 2b - Copy` 5 on 656 (0.76%), `moms-63 3e - Copy` 7 on 331 (2.11%), `moms-53 3 - Copy` **0 leads on 511 link clicks**. That is a 10.6x gap against the March cohort on the same subdomain.

**The matched pairs are the cleanest evidence and they indict the August cohort.** Four creative files ran to both destinations with meaningful volume on each side, controlling for creative entirely:

`00b743c5…` (`moms-63 2b`) took 3,404 link clicks to 417 leads on `www.` — 12.25%, $13.26 cost per lead, created 2026-08-14 in `USHA - ABO - TEST - MOMS` — against 656 link clicks to 5 leads on `go.` — 0.76%, $167.10, created 2026-08-31 in `USHA - CBO - OTP`. `6a45457e…` (`moms-63 3e`) took 3,531 link clicks to 339 leads on `www.` (9.60%, $15.46) against 331 to 7 on `go.` (2.11%, $72.00). `e6225ca2…` (`moms-53 3`) took 2,055 link clicks to 119 leads on `www.` (5.79%, $16.43) against **511 link clicks to zero leads** on `go.` `645496c4…` (`Moms Nahuel WV#1 - V9`) took 7,196 link clicks to 635 leads on `www.` (8.82%, $27.91, created 2026-04-06) against 690 to 6 on `go.` (0.87%, $273.23, created 2026-08-17). Pooled: **`www.` 1,510 leads on 16,186 link clicks (9.33%) against `go.` 18 leads on 2,188 link clicks (0.82%) — an 11.3x gap on identical video files.** **Verified**, `include: ["extended"]` media-hash pulls 2026-09-04.

**The reverse lens is what splits the cohort, and it is the single most important number here.** Leads per *landing page view* — taking the suspect counter at face value and asking whether it behaves like a real number. Across `www.` the account converts arrivals to leads at 13.66% lifetime (30,702 of 224,701), and per ad at 13.99% (`moms-63 2b`), 11.25% (`moms-63 3e`), 10.25% (`Moms Nahuel WV#1 - V9`) and 7.65% (`moms-53 3`) — a band of roughly 8 to 14%. The **March `go.` cohort converted 248 leads out of 299 recorded landing page views — 82.9%**, which is not a possible on-page conversion rate for cold insurance traffic and is the direct proof that the counter is undercounting arrivals there. The **August `go.` cohort converted 18 leads out of 156 recorded landing page views — 11.5%**, sitting squarely inside the account's normal band. For the August ads, the landing-page-view number behaves exactly like a truthful one.

**`click_quality` is a restatement of the suspect metric.** Reproduced to two decimals on seven ads across both domains: 63 ÷ 690 = 9.13 (reported 9.13), 92 ÷ 800 = 11.50 (11.5), 54 ÷ 656 = 8.23 (8.23), 9 ÷ 511 = 1.76 (1.76), 2,981 ÷ 3,404 = 87.57 (87.57), 32,529 ÷ 35,471 = 91.71 (91.71), 6,198 ÷ 7,196 = 86.13 (86.13). It is `100 × landing_page_views / link_clicks` and nothing else. `ad-metrics-glossary.md` carries no entry for it. **Verified** arithmetically. It must never again be cited as independent corroboration of a landing-page-view finding.

**The confound could not be broken.** `USHA - CBO - OTP` holds $3,534.55, 2,209 link clicks and 19 leads at a $186.03 cost per lead — and **2,196 of those 2,209 link clicks are the `go.` ads themselves**. The campaign's number *is* the destination's number; they are the same traffic. The only non-`go.` ad in that campaign is a `quiz.healthformoms.com` variant with 10 link clicks and 1 lead, which decides nothing. Campaign, creation date and destination are perfectly collinear in the failing cell, and no cut of this account separates them.

The 2×2 that results: `go.` × March = 8.69%; `go.` × August = 0.82%; `www.` × spring = 8.82% (`Moms Nahuel WV#1 - V9`); `www.` × August = 9.50%. Exactly one of the four cells fails. It is not the domain alone — the March `go.` cohort worked. It is not the date alone — the August `www.` cohort worked. It is the intersection, and the intersection is also one single campaign.

## Evidence against, and how it weighed

The evidence *for* the prediction is strong and it is not soft: 2,854 link clicks and 248 leads at a normal 8.69% on the supposedly broken destination, and a physically impossible 82.9% leads-per-arrival that can only mean the counter is missing arrivals. The March cohort settles that the landing-page-view number on `go.` cannot be read as a count of lost clicks. The claim that this destination "loses nine of ten clicks" is, as a general statement about the subdomain, not supported.

The evidence *against* is equally strong and it is not explained away: four identical creative files converting at 9.33% on `www.` and 0.82% on `go.`, including one taking 511 link clicks to zero leads, and an August cohort whose leads-per-arrival rate of 11.5% is exactly what a genuinely-lost-clicks story predicts. If the August `go.` pixel were simply undercounting the way the March one demonstrably was, leads would still have been counted at full rate — they were counted at full rate in March on the same subdomain — and the August cohort would look like the March cohort. It does not.

Neither side folds. The honest reading is that the two cohorts are describing two different situations on one subdomain: a long-standing page-view counting fault that has always been harmless, and a lead collapse that arrived with the August cluster and is real. The prediction as written — a single claim about the destination — is true of the first and false of the second.

One live limitation, named because it bears on the strongest evidence for the prediction. Parker stamps each ad's *current* landing URL, and the March ads are paused; there is no way from these pulls to confirm the URL those ads carried while they were actually delivering. What supports it being `go.` at the time is that their click-quality scores run 2 to 16, the `go.` signature, where any `www.` ad in the account runs 35 to 92. That is strong but circumstantial, and if those ads in fact ran to `www.` and were re-pointed later, the whole March-cohort argument falls and the verdict moves to invalidated.

## Why this is the verdict

The hypothesis set the bar in advance. **Validated** required normal leads per link click on `go.` across the cohort *and* an implausible leads-per-arrival rate. **Invalidated** required leads per link click far below `www.` for matched creative *and* a normal leads-per-arrival rate. The March cohort meets the validated bar exactly. The August cohort meets the invalidated bar exactly. Both conditions were met, by different halves of the same 40 ads, and the hypothesis's own third state names this: "the cohort splits — some `go.` ads convert normally per link click and others collapse — so both readings are true of different ads and the single prediction does not describe the destination," and "the collapse is real but campaign, date and destination are collinear, so the cause cannot be assigned." Both of those happened. **Inconclusive.**

This is inconclusive rather than insufficient, and the distinction matters for what the next pass should do. There is no shortage of data — 8,918.29 dollars, 5,392 link clicks and 272 leads on `go.`, against 288,916 link clicks and 30,702 leads on `www.`, with four clean matched pairs. The evidence is plentiful and it points both ways. What is missing is not volume but a cut that separates campaign from destination, and this account does not contain one, because every August `go.` ad is in `USHA - CBO - OTP` and virtually all of that campaign's traffic is `go.` ads. Resolving it requires evidence from outside Parker, named in the recommendation below.

The doc does not enter `brand-profile.md`. Nothing was confirmed, and only validated insights take that path.

## What this corrects, and what it does not

It corrects one thing firmly, and that correction should propagate regardless of the unresolved verdict: **`click_quality` is a restatement of landing page views ÷ link clicks and is not independent evidence.** `audits/2026-Q3/90-day-creative-strategy-audit.md`, `audits/2026-09/monthly-performance-report.md`, `audits/2026-09/weekly-performance-snapshot.md`, `sub-context-docs/ad-account-evaluation.md` and `sub-context-docs/performance-targets-and-metrics.md` each cite a click-quality score alongside the landing-page-view ratio as though it were a second, corroborating measurement. It is the same measurement. Those passages overstate their evidence even where their conclusion may hold.

It does **not** establish that the destination is broken, and it does not establish that it is fine. The archived roll-up verdict — "it is a broken redirect or a broken pixel" — remains possible and is now better supported for the August ads specifically than it ever was for the subdomain as a whole. Its generalisation to all 40 ads is refuted: the March cohort bought leads at normal rates on that subdomain.

## Loops this opens

Written as open questions, observation first, with no test design and no closure path built in — per the open-loops generation rubric.

**One.** Sixteen ads created in August on `go.healthformoms.co/save/` produce leads at 0.82% of link clicks while the identical video files on `www.` produce them at 9.33%, and the March ads on that same subdomain produce them at 8.69%. **What changed for that subdomain between March and August 2026?**

**Two.** Every ad in `USHA - CBO - OTP` points at `go.`, and the campaign's entire result is those ads' result. **What is `USHA - CBO - OTP` set up to do that the account's other campaigns are not?**

**Three.** The landing-page-view counter on `go.` recorded 299 arrivals for a March cohort that produced 248 leads, a rate no page achieves. **Which of the events on that subdomain are firing, and which are not?**

**Four.** Statics carry a $12.30 lifetime cost per lead against video's $22.23, and the `www.` statics in this pull convert at 15–22% leads per link click against video's 6–12%. **What is different about how a mom arrives from a static?**
