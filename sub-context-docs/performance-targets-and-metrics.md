---
brand: health-for-moms
doc: performance-targets-and-metrics
generated_on: 2026-09-04
refresh_by: 2026-12-03
quarter: 2026-Q3
sources:
  - "Live ads manager via Parker MCP `search_facebook_ads_sql`, Meta account HealthForMoms act 484897827497337, seven pulls run 2026-09-04: trailing 90 days grouped by name, trailing 7 days grouped by name, lifetime filtered to static, lifetime filtered to video, an efficiency ranking filtered to ad-name groups spending $1,000 or more, an adIds lookup on the four `Moms Nahuel WV#1 - V9 - Copy` variants, and an engagement cut on the top spenders"
  - "Parker MCP `list_custom_metrics`, run 2026-09-04: four auto-detected pixel events, zero formulas, no revenue metric of any kind"
  - "Parker MCP `check_northbeam_connection` state as recorded at Phase 0: not connected"
  - "`running-notes/success-definition.md` and `running-notes/brand-rules.md`, the brand intake captured 2026-09-03"
  - "`sub-context-docs/marketing-calendar-and-campaigns.md`, whose thirteen consecutive monthly pulls are the spine of the metric story here"
  - "`sub-context-docs/ad-account-evaluation.md`, the sibling creative diagnosis this scoreboard is read against"
  - "`sub-context-docs/reputation-analysis.md` and `sub-context-docs/website-and-product-audit.md` for the channel map"
  - "audits/2026-Q3/90-day-performance-audit.md, audits/2026-Q3/90-day-creative-strategy-audit.md, audits/2026-Q3/90-day-diversity-audit.md, audits/2026-Q3/quarterly-whitespace-analysis.md, audits/2026-09/monthly-performance-report.md, audits/2026-09/monthly-hook-audit.md, audits/2026-09/weekly-performance-snapshot.md"
knowledge_docs_read:
  - parker-system/creative-strategy-context/expertise-routing.md
  - parker-system/creative-strategy-context/ad-account-analysis.md
  - parker-system/creative-strategy-context/ad-metrics-glossary.md
  - parker-system/creative-strategy-context/killer-performance-ads.md
  - parker-system/creative-strategy-context/andromeda-v2.md
  - parker-system/creative-strategy-context/analyzing-public-ad-accounts.md
  - parker-system/creative-strategy-context/seasonality.md
  - parker-system/creative-strategy-context/creative-strategy-by-brand-size.md
benchmark_status: "brand-confirmed on the cost-per-lead tiers and the two-gate winner definition; provisional-account-derived on the winner set, the CPM, CTR, hook-rate and hold-rate bars, and every efficiency threshold below"
account_purpose: "The account is the business. Health For Moms is a lead-generation front end for a match-and-consult referral to partner insurance agencies, with no purchase event, no repeat buyer and no other discoverable acquisition channel. Paid Meta is not an accelerant here, it is the oxygen. Inferred from the account shape, the zero-purchase pull and the reputation read, not stated by the brand."
history_windows_read: "trailing 7 days, trailing 30 days via the August monthly cut, trailing 90 days against the matched prior 90 days, thirteen consecutive months from 2025-09 to 2026-09, and full lifetime from the first ad created 2024-12-05"
data_limitations:
  - "No max tolerable cost per acquisition, customer value, gross margin, lifetime value or payback window was captured at intake. Without a business ceiling, every use of the word efficient in this doc is relative to the account's own trailing number, never to a profit threshold."
  - "Lead quality is invisible to Parker. It lives with the partner insurance agencies, not in Meta. The pixel's only shadow of it is a `Call` event that fired 42 times against 4,336 leads in the window, which is far too thin to read as a quality proxy."
  - "Northbeam is not connected and no third-party attribution tool exists. Every figure is Meta-reported on the Meta default attribution window. Nothing here is multi-touch."
  - "Reach and frequency are not returned for this account, so cost per thousand accounts reached cannot be computed and the saturation check `ad-account-analysis.md` calls central cannot be run."
  - "Placement is not exposed. The demographics block returns age, gender, device and platform only."
  - "Account-level hook rate and hold rate are not in the period summary. Both are reported spend-weighted across named top-spender sets, with the coverage share stated every time."
  - "Month-by-month period metrics do not exist before 2025-09-01, so roughly $104,000 of the account's $743,218 lifetime spend cannot be placed in a month and the account's first winter is invisible."
  - "One Open Enrollment is one observation. Every seasonal claim here rests on a single year and none of it is a confirmed rhythm."
  - "No competitor libraries are tracked, so every benchmark below is the brand against itself. Nothing is benchmarked against the category."
  - "The brand's own site could not be opened from the build session, so there is no read of funnel steps, form length or quiz logic beyond what the ad-level landing-rate data shows."
---

# Performance targets and metrics - Health For Moms

## Business state and what the account is for

**This account is not a marketing channel for the business. It is the business.** Health For Moms sells nothing directly. It runs paid ads to a `/save/` page, collects a form fill, and hands that lead to a partner insurance agency where a licensed advisor makes the actual sale on a phone call. There is no cart, no checkout and no purchase event anywhere in the account. Lifetime, across twenty-one months, it has spent **$743,218.09 for 39,569 leads at a blended $18.78 cost per lead, and recorded exactly zero purchases**. **Verified**, two lifetime pulls run 2026-09-04.

The reason that read matters more than any number below is that it removes every escape hatch a normal efficiency conversation has. A retail brand with a bad month can point at shelf sell-through. An ecommerce brand with a high acquisition cost can point at repeat purchase. This brand has neither. It has no discoverable organic search presence, no press, no review corpus on any surface, no retail, no marketplace, no email or SMS surface connected, and no organic social beyond a Facebook page that carries the ads. **Verified** in `reputation-analysis.md` against live searches. So **every dollar in this account is acquisition, and every mismatch is an acquisition mismatch.** There is no second engine to carry a weak quarter.

**Where it sits on spend.** Read against `creative-strategy-by-brand-size.md`, the account has lived in two different bands inside one year and is currently in the lower one. At its April 2026 peak it ran **$156,716 in a month**, which is squarely the fifty-thousand-a-month tier and above it. Right now it runs about **$42,700 a month** on August's number and roughly **$17,700 a week** on the trailing seven days, which is the same tier from underneath. **Verified.** That band's priorities are the ones that apply: volume of output matters as a real lever rather than an occasional push, reaching genuinely new audiences becomes the question rather than sweeping up existing demand, and the brand's own picture of who its customer is deserves checking against the data rather than trusting. All three land hard here. The account's format menu shrank from 20 to 15, its delivery is concentrated in a twenty-year age band, and its own comment section is full of women discovering they do not qualify.

**What the account is trying to maximise, plainly.** Qualified lead volume at a cost the partner agencies can work profitably. The brand's stated sequence is efficiency first, then scale: *"Both scale and efficiency, but efficiency first."* **Stated**, intake 2026-09-03. The account's own behaviour agrees with the first half and not obviously with the second. It held cost per lead at a two-cent variance through a 73.5% spend collapse, which is an efficiency-preserving posture. It has not scaled since April.

## How to read this brand's numbers

Read this section before any figure below, because it is the lens.

**One. Never report ROAS, average order value, purchase value or add-to-cart for this brand.** ROAS reads 0 on all 128 delivering ad-name groups because there is no purchase event, not because the ads fail. Quoting a return figure here is a fabrication, not a conservative estimate. **Verified** and set as a standing rule in `running-notes/brand-rules.md`. The judgment set is **cost per lead, lead volume, CPM, CTR, hook rate and hold rate.**

**Two. A winner is two-gated and Parker can only see gate one.** The brand said it verbatim: *"CPL is important to scale but then we look at the lead quality as well before really scaling."* **Stated.** Gate one is cost per lead, visible on every ad. Gate two is whether the lead holds up downstream, and it lives with the partner agencies. **Never call an ad a winner on cost per lead alone.** The correct phrase is a candidate that passed gate one, with gate two named as the open question, every single time. The pixel offers only a whisper of gate two: `list_custom_metrics` returns four auto-detected events, `offsite_conversion.fb_pixel_custom`, `.Call`, `.click` and `.invitee_meeting_scheduled`, with no formulas and no revenue metric. **Verified**, 2026-09-04. In the 90-day window the `Call` event fired **42 times against 4,336 leads across 15 ads**. That is under one percent and it is not a quality proxy.

**Three. Cost per lead is nearly blind to the creative here, and that is the single most important thing on this page.** Across two structurally different quarters, cost per lead moved from **$22.65 to $22.63**. In between, spend fell 73.5%, ad count fell 70.4%, the dominant format went from a long tail to one container at roughly 70% of spend, the dominant emotion swapped from anger at 55.2% to pride at 49.5%, the awareness posture flipped from 80.2% problem-aware to 56.2% solution-aware, and a whole Life Force desire fell 98.6%. **Verified** from matched pulls. A metric that will not move through that much upheaval is not measuring the creative. It is measuring the offer, and the offer did not change. What *did* move is everything cost per lead cannot see: spend-weighted hold rate fell from 11.09% to 3.83%, CTR fell 26.2% from 2.44% to 1.80%, and cost per link click rose from $1.76 to $1.95. So when a later strategy asks whether the creative got better, cost per lead will not answer it. Read the movement metrics alongside.

**Four. Segment by destination before grading anything.** One broken redirect distorts every blended number this account produces. Ads pointed at `go.healthformoms.co/save/` convert 6.9% to 9.1% of their link clicks into landing page views. Everything else in the account converts 84.6% to 85.4%. **Verified** by landing-url filtered pulls in both the monthly and weekly reports. In the week to 2026-09-04 that one destination took 15.8% of the money and moved the headline cost per lead from a clean $21.98 to a reported $25.61. The blended number was lying by $3.63. Any ad routed through `go.` should be treated as **unscored**, not as a loser, because grading creative on a page that eats nine of every ten clicks will get good creative killed.

**Five. The quiz is unmeasured, not leaking.** This is a canonical correction and it is worth restating in the scoreboard doc because it is a numbers error, not a creative one. The figures "903 link clicks against 234 landing page views" and a "$75.72 cost per lead" are **two destinations summed**, not the quiz. I re-ran the split at ad level on 2026-09-04: `go.healthformoms.co/save/` took $1,639.35 for 690 clicks, **63** landing page views, a 9.1% landing rate, 6 leads and a **$273.23** cost per lead at a click quality score of 9.13; `www.healthformoms.co/save/` on the same creative file took $404.23 for 213 clicks, 171 landing page views, an 80.3% landing rate, 21 leads and a **$19.25** cost per lead at click quality 80.28. **`quiz.healthformoms.com` is a brand-new test at $138.27 lifetime across 26 ads, all created 2026-09-02 or 09-03. Treat it as unmeasured.** And note the mechanism that caused the original error, because it will recur: a `groupBy: name` pull returns that whole family as one row summing four variants across three destinations, and stamps the newest variant's URL on it. **Verified** by running the grouped and ad-level pulls side by side.

**Six. Ad count is not effective ad count.** Read through `andromeda-v2.md`, four ads sharing one text hook and a near-identical opening frame of a mother with a small child are very likely one entity ID wearing four creative IDs. Those four carried 60.5% of the quarter. So when this doc says 128 delivering ad-name groups, the number of genuinely distinct things Meta is choosing between is smaller, probably much smaller. **Inferred**, because Meta does not expose entity grouping and frequency is not returned for this account.

## Performance history and metric story

The spine of this section is thirteen consecutive monthly pulls run 2026-09-04, reported in `marketing-calendar-and-campaigns.md`. All figures Meta-reported on the Meta default window. **Verified.**

| Month | Spend | Leads | CPL | CPM | CTR | Landing page views to leads |
|---|---|---|---|---|---|---|
| 2025-09 | $17,416.10 | 1,390 | $12.53 | $14.19 | 1.59% | 17.7% |
| 2025-10 | $21,663.87 | 1,766 | $12.27 | $17.57 | 1.79% | 18.7% |
| **2025-11** | **$34,235.57** | **2,617** | **$13.08** | **$23.13** | **2.53%** | 17.1% |
| **2025-12** | **$28,706.54** | **1,570** | **$18.28** | **$29.34** | 2.61% | **14.2%** |
| 2026-01 | $20,297.31 | 1,010 | $20.10 | $24.50 | 1.88% | 13.4% |
| 2026-02 | $29,312.76 | 1,253 | $23.39 | $20.34 | 1.77% | 12.3% |
| 2026-03 | $114,106.93 | 5,473 | $20.85 | $24.16 | 2.87% | 8.8% |
| **2026-04** | **$156,716.43** | **6,988** | $22.43 | $22.88 | 2.52% | 8.6% |
| 2026-05 | $105,665.91 | 4,240 | $24.92 | $24.03 | 1.92% | 9.4% |
| 2026-06 | $42,698.49 | 1,540 | $27.73 | $24.22 | 1.67% | 9.5% |
| **2026-07** | **$18,389.74** | 929 | $19.80 | $20.82 | 1.73% | 11.1% |
| 2026-08 | $42,748.63 | 1,987 | $21.51 | $23.66 | 1.93% | 10.5% |
| 2026-09, first 4 days | $7,345.98 | 287 | $25.60 | $22.82 | 1.92% | 10.6% |

**Twelve months, told as a story.** The cheapest leads this account has ever bought were in autumn 2025, at $12.27 to $12.53, on CPMs of $14 to $18. Cost per lead has roughly doubled since, and the shape of the rise is instructive because it is not one event. It steps up through December and January as the auction gets expensive, plateaus in the low twenties through the spring scale-up, peaks at **$27.73 in June** when the account was starved of new creative, and comes back to $21.51 in August when 85 new files went live.

Underneath that, one number falls almost monotonically and nobody has flagged it: **the share of landing page views that become leads went from 18.7% in October 2025 to 8.6% in April 2026, and sits at 10.5% in August.** **Verified** across thirteen pulls. That is the funnel step after the click and before the lead, and it more than halved. Some of it is the destination break, which only exists from mid-August. Most of it is not. The best available read is that the account traded qualified traffic for cheap traffic as it scaled, and the form-fill rate paid for it. **Inferred**, confidence **mixed**, because Parker cannot see the page itself and cannot separate a page change from a traffic-quality change.

**Six months.** March through August 2026 took **$480,326.13** for **21,157 leads at $22.70**. Inside that, the account went from its largest month ever to its smallest in three, and cost per lead moved from $20.85 to $21.51 with a $27.73 spike in between. The 73.5% quarter-over-quarter collapse sits in the middle of this window: **$374,507.92 down to $99,266.98**, leads down by exactly the same 73.5%, cost per lead moving one cent. **Verified** across two matched pulls. Leads and spend falling in perfect lockstep while efficiency does not move is what a budget decision looks like. A fatigue collapse pushes cost up as it falls. **Inferred**, confidence **strong** on the mechanism, and the reason itself is a brand-routed loop below.

**Three months.** The trailing 90 days to 2026-09-03, pulled live 2026-09-04: **$100,065.31, 4,421 leads, $22.63 cost per lead, $22.96 CPM, 1.80% CTR, 4,358,580 impressions, 51,299 link clicks at $1.95 each, 42,425 landing page views, zero purchases.** 128 ad-name groups delivered. Delivery ran **95.3% female, 81.2% aged 25 to 44, 99.5% mobile**, and 60.3% Facebook to 39.1% Instagram. The upstream audits measured this window at $99,266.98 and $22.64 the day before; the small gap is normal data settling on a window whose last day had not closed. Both readings tell the same story.

**One week.** 2026-08-28 to 2026-09-03: **$17,696.22, 692 leads, $25.57 cost per lead, $23.45 CPM, 1.94% CTR**, 77 groups delivering. **Verified**, live pull. Strip the broken destination and the weekly snapshot reads it at $21.98 clean against $21.74 the week before, a 1.1% move rather than a 7.3% one. Two things inside the week matter for the scoreboard. The incumbent is aging: `Moms43 - 4 - V3` took $3,543.83 for 109 leads at **$32.51** on a $27.32 CPM, against $22.28 across the full quarter, with its hook rate unchanged at 46.11%. Per `ad-account-analysis.md`, CPM climbing while attention holds steady is the shape of an audience being used up, and frequency would confirm it if the tool returned it. And the newer, cheaper work is now the biggest line item: `moms-63 3e` took $3,638.53 at **$17.00** on the cheapest impressions in the account at $19.32.

**Lifetime, and the split that reframes the whole history.** Video carries **$574,310.36 and 25,834 leads at $22.23** across 1,257 name groups, on a $23.68 CPM and a 2.28% CTR. Static carries **$168,907.73 and 13,735 leads at $12.30** across 308 name groups, on a **$17.99 CPM** and a 1.76% CTR. **Verified**, two filtered lifetime pulls 2026-09-04. Statics took 22.7% of the money, delivered 34.7% of the leads, cost 44.7% less per lead, and bought impressions 24% cheaper. **Not one has run in the last 90 days.** The autumn 2025 months where cost per lead sat at $12 are the months the static library was live. That is not proof of causation and it is the most important correlation on this page.

## Efficiency and return targets

**What the brand gave us, and it is a real bar rather than an aspiration.** The cost-per-lead tiers are stated directly in the brand context document: **under $15 fantastic, $15 to $20 good, $20 to $25 meh, over $25 not good.** **Stated**, brand context, confirmed at intake. That is unusually usable. Most brands hand over one number or none.

**Where the account actually sits against it.** The trailing 90 days blend to **$22.63**, which is the middle of the "meh" band. The account has now been parked in that band for six straight months, from March through August, and it was in "fantastic" as recently as October 2025. **Verified** across thirteen monthly pulls. The trailing week reads $25.57 blended, which crosses into "not good," and $21.98 once the broken destination is stripped, which does not. So the honest statement is: **the account is missing its own good-tier target and has been for two quarters, and it is missing it by about three dollars a lead.**

**There is no return target and there cannot be one.** Return on ad spend is undefined for a business with no purchase event. There is no target ROAS, no target marketing efficiency ratio and no contribution-margin bar in this brain, and inventing one would be the exact failure this prompt warns against.

**The bar that is genuinely missing is the ceiling.** No max tolerable cost per acquisition was captured at intake, and neither was customer value, gross margin, lifetime value or a payback window. **Stated** as unanswered in `running-notes/brand-rules.md`. That absence has a specific consequence worth naming rather than filing: the brand's tiers say $22.63 is "meh," but nothing in this brain can say whether $22.63 is *profitable*. A lead sold onward to a partner agency has a price, and that price is the number that decides whether the account should scale, hold or cut. Until it exists, every efficiency read here is the account graded against its own history, which is a real bar but not a business one.

## New vs returning focus

**One hundred percent acquisition, and structurally so.** There is no purchase event, no returning buyer, no subscription, no replenishment and no repeat-purchase path in this account. Lifetime, most-aware creative carries **0.1% of spend** and unaware carries **0.0%**, which is $75.22 across two ads in the account's entire life. **Verified** from the lifetime awareness cut in the whitespace analysis. Problem-aware carries 60.9% and solution-aware 28.6%.

That zero at the bottom of the funnel is correct and should not be flagged as a hole. For an ecommerce brand it would be a neglected retention story. Here there is nobody to retain. The zero at the *top* is the real one. The brand's stated ambition is "SCALE BABY!", and an account that has never once addressed a woman who was not already unhappy with her insurance has a hard ceiling on how many people it can reach.

**Where the stated focus and the actual spend disagree.** The brand says it wants to test *"All different ages of moms with ages of kids,"* including younger mothers with babies and older second-chapter mothers. **Stated.** The account puts **81.2% of spend on the 25-to-44 band**, 2.5% on 18-to-24 and 3.5% on 55-plus combined. **Verified.** Two of the brand's own stated test audiences receive almost no money. That is not a targeting error so much as a creative one, since the account runs broad and the creative does the qualifying, but it is a gap between the plan and the spend.

## Spend levels and trajectory

**Everything is on one platform.** Meta carries 100% of measured paid spend. Inside Meta, the 90-day placement split by platform runs **Facebook $60,371.84 at 60.3%, Instagram $39,090.49 at 39.1%, Audience Network $506.54 at 0.5%, Threads $95.83 at 0.1%, Messenger eight cents.** **Verified**, live pull 2026-09-04. That Facebook-to-Instagram balance is remarkably stable, identical to a tenth of a point across two matched 90-day windows. Device is 99.5% mobile in both.

One split inside the lifetime data is worth carrying: **statics delivered 50.4% Facebook to 49.4% Instagram, while video delivered 60.4% to 39.0%.** **Verified**, two lifetime pulls. The modality is moving the platform mix by ten points, which per the placement-signal logic in `ad-account-analysis.md` means the static library was reaching a meaningfully different, more Instagram-weighted audience than the video library reaches now.

**The trajectory, in one line: peaked in April, cut by three quarters by July, rebuilding since August, still less than a third of peak.**

| Window | Spend | Direction |
|---|---|---|
| Peak month, 2026-04 | $156,716.43 | The largest month in the readable history |
| Trough month, 2026-07 | $18,389.74 | Down 88.3% from peak |
| Latest full month, 2026-08 | $42,748.63 | Up 132.5% from the trough, 27.3% of peak |
| Trailing 7 days annualised to a month | roughly $75,800 | Ahead of August's pace |
| Trailing 90 days | $100,065.31 | Down 73.5% on the matched prior 90 |

**Verified** across monthly and period pulls. The last row is the one to hold: at the current weekly run rate the account is pacing well above August, which is consistent with a November ramp beginning. Creative production supports that read. **125 ads were created between 2026-08-01 and 2026-09-04**, against 63 in October 2025, which was the run-up to the last Open Enrollment. **Verified** from created-time pulls. The machine is warmer now than it was a year ago at the same point in the season.

## Ad platforms in use

**Meta, and nothing else that Parker can see.** One connected ad account, `HealthForMoms`, act 484897827497337, currency USD. **Verified** from the account list returned on every pull.

No Google, TikTok, Pinterest, YouTube, Reddit, Snapchat or programmatic surface is connected to Parker or visible in any source in this brain. Whether the brand runs any of them outside Parker's view is not knowable from here and is **routed to the brand**. What can be said is that nothing in the brand context, the intake, the four Parker chat threads or the reputation read mentions a second platform.

The concentration is worth naming without judging it. A brand running one platform at this spend level is not obviously making a mistake, and per `creative-strategy-by-brand-size.md` the flag worth raising is the opposite one, a brand spreading onto a new platform before it has mastered its main one. This brand has not done that. The risk it carries instead is single-point exposure: one auction, one policy regime, one delivery system, and a category where platform moderation risk is real.

## KPI benchmarks

Two kinds of bar apply here and they should never be blended.

**Brand-confirmed.** The cost-per-lead tiers: **under $15 fantastic, $15 to $20 good, $20 to $25 meh, over $25 not good.** **Stated**, brand context document. This is the bar that governs, because it is the brand's own.

**Provisional, account-derived, and clearly marked as mine.** The brand gave no bar for anything else, so the following are read off the account's own distribution and off the general defaults in `ad-metrics-glossary.md`, which that doc is explicit are starting points rather than laws.

| Metric | Account's own level | General starting bar | Read |
|---|---|---|---|
| Cost per lead | $22.63 over 90 days | brand's tiers | Missing the good band by about $3 |
| CPM | $22.96 over 90 days | none applicable | Cheap for a regulated insurance category, and it improved as spend fell |
| CTR | 1.80% over 90 days, down from 2.44% | above 1% | Above the floor, and falling while hook rate rises |
| Hook rate | 43.40% spend-weighted on the top ten carrying 87.3% of spend | 30% minimum, 45-50% strong | Genuinely strong. This is the account's best metric |
| Hold rate | 3.83% spend-weighted on the same set | 12-15% | Far below floor, and the metric the audits agree is broken |
| Landing rate, clicks to landing page views | 84.6% to 85.4% on the working destination | none applicable | Healthy. The `go.` destination's 6.9% to 9.1% is the outlier |
| Landing page views to leads | 10.5% in August, down from 18.7% in October 2025 | none applicable | The quietest deterioration in the account |
| Frequency | not returned | 1.2 or lower | Cannot be read. **Data-limited** |
| Cost per 1,000 accounts reached | not computable, reach not returned | none | Cannot be read. **Data-limited** |

The two hold-rate rows deserve a caveat rather than a verdict, and it belongs in the benchmark section rather than buried. The craft floor says 12% to 15%. This account's cheapest lead comes from an ad holding **2.39%**, and its best-holding ads sit in the worst cost band at $29.85 to $38.09. **Verified** across the efficiency ranking. So the general bar and this account's own evidence disagree, and this doc does not resolve that by picking a side. It sits in the loops.

## Purchase cycle, LTV, and metric meaning

**What the account can show.** The path is short and mechanical: see the ad, click, land on `/save/`, fill a form, get handed to a partner agency, take a phone call. Cost per link click is $1.95, 84.6% of those clicks reach the page, and roughly 10% of page views become a form fill. **Verified.** From impression to lead the whole thing can happen in under two minutes.

**What happens after the form is invisible, and that is where the economics live.** A licensed advisor at a partner agency runs a consultation, quotes plans and closes or does not. None of that returns to Meta. The pixel sees a `Call` event 42 times against 4,336 leads. **Verified**, live custom-metric read. So the account measures the *first* step of a multi-step, high-trust, phone-mediated sale and treats it as the outcome.

**What that does to the metrics, per the reading discipline in this prompt.** Health insurance is a slow, high-consideration, high-trust purchase. The buyer researches, asks whether the company is legitimate, worries about being sold to, and often waits. The brand's own context names *"I don't want to get on a call and be sold to"* as a live objection and *"I should just wait for open enrollment"* as a timing objection that can cost months. **Stated.** For a product shaped like that, a last-click form fill systematically **oversells** the creative that produces fast, low-friction clicks and **undersells** the creative that does the trust work. That is the mirror image of the usual warning, and it is the right way round for this brand: the metric is not missing the slow creative, it is over-rewarding the fast creative, because the form fill is cheap to produce and says nothing about whether a licensed advisor can close the person on the other end.

The comment corpus is the clearest evidence that this is not theoretical. The largest substantive cluster in the 90-day window, ten of 38 real comments, is people discovering after clicking that they do not qualify, on grounds no ad mentions: pre-existing conditions, income under $30,000, having an employer plan available, and pregnancy. **Verified** verbatims. Those are leads the account paid for and the funnel then turns away.

**Lifetime value: unknown, and unjudgeable until it exists.** No customer value, no gross margin, no payback window, no cohort data. **Data-limited.** The honest position, and the one `ad-account-analysis.md` and this prompt both insist on, is that **$22.63 cannot be called good or bad in isolation.** It can be called worse than this account's own $12.30 static history and worse than its own $12.27 October 2025 month, and those are real comparisons. It cannot be called inefficient against a business threshold, because no threshold exists.

## Provisional winner definition

**The brand's definition governs and it has two gates.** Gate one is cost per lead. Gate two is lead quality, assessed before real scale, and it is invisible to Parker. **Stated**, intake verbatim. Everything below therefore names candidates that passed gate one, never winners.

**The provisional set, built from the account itself.** Metric ranked by: **period cost per lead**, which is the metric the account is genuinely steering by and the one the brand named. Window: **2026-06-06 to 2026-09-03**. Comparable set: the **15 ad-name groups that spent $1,000 or more**, which together carry **$94,101.32 of the window's $100,065.31, or 94.0% of spend**, and blend to a $22.04 cost per lead. The spend floor is there because the top-decile rule must not crown an ad with trivial delivery, and $1,000 buys roughly forty-five leads at the account's own rate, which is enough to read. **Verified**, efficiency-ranked pull 2026-09-04.

The top of that distribution, in order:

| Rank | Ad | Spend | Leads | CPL | Band | Hook / hold |
|---|---|---|---|---|---|---|
| 1 | `moms-63 2b` | $5,529.74 | 417 | **$13.26** | fantastic | 40.15% / 2.39% |
| 2 | `moms-63 3e` | $5,448.56 | 353 | **$15.44** | good | 42.89% / 2.88% |
| 3 | `moms-53 3` | $2,041.29 | 127 | **$16.07** | good | 35.49% / 3.89% |
| 4 | `MOMS39 - 2 - V2 - Copy` | $1,472.06 | 79 | $18.63 | good | 36.93% / 5.01% |
| 5 | `moms-65 1a` | $1,346.61 | 62 | $21.72 | meh | 32.62% / 4.26% |

For contrast, the bottom of the same set: `moms54-2` at **$34.94**, `Moms43 - 4 - V4` at $30.21 and `moms54-3` at $29.85, the last of which posted the account's best attention numbers in the same window at a 57.02% hook rate and a 13.66% hold rate.

**So the provisional winner definition, stated plainly:** for now, a gate-one candidate at this brand is an ad that has spent at least $1,000 in the window and delivered a cost per lead at or below **$16.07**, which is the top fifth of the meaningfully delivered set and sits inside the brand's own "good" band. Three ads currently clear it. Confidence **mixed**, because all three launched in August and none has run a full quarter, and because the ranking metric cannot see gate two at all.

**This is a starting point for the team call, not the brand's confirmed definition.** The two things that would replace it are a max tolerable cost per lead from the business, and any signal at all from the partner agencies about which of these three produces leads an advisor can actually close.

## Channel mix and how the channels relate

There is almost nothing to map here, and the emptiness is the finding.

**Paid Meta is the only demand-generating channel, and it is also the only demand-harvesting channel.** Normally this section separates the two, notes where one channel takes credit for work another did upstream, and reads the relationships. This brand has one channel. Search is not a harvest lane for it: the brand does not appear anywhere in the results for the category query a real buyer would type, while a named competitor holds a first-page position. **Verified** in `reputation-analysis.md`. Its own name is made of four of the most common words in American health policy, so it cannot separate itself from a decade of government and nonprofit content using the same words. There is no press, no review corpus on any surface, no Better Business Bureau profile for the operating entity, and no marketplace or retail presence.

**The one place a genuine cross-channel handoff exists is invisible.** The chain is Meta ad, landing page, form, then a phone call at a partner agency. That final step is where the money is made and it is where the measurement stops. So the brand's real cross-channel gap is not between Facebook and email. It is between the platform and the agency, and it is total.

**Organic is not feeding paid.** The brand runs no organic social account Parker can see beyond a Facebook page that carries the ads. The paid engine is not building one either: the top-spending ad bought **1,987,158 impressions and produced 116 page likes**, a page-like rate of 0.0058%, alongside 327 shares, 385 saves and 84 comments. **Verified**, engagement pull 2026-09-04. Read through the organic-seeding mechanism, this account is giving the platform no owned audience or language signal to start from. The full footprint read is in `organic-channels-inventory.md`.

**What this means for reading any single number.** Nothing in this account is being helped or flattered by another channel. There is no brand search halo to absorb, no email list re-converting the same people, no retail lift to argue about. When cost per lead moves here, paid Meta did it. That is unusually clean, and it is the one advantage of having no other channels.

## Attribution model and its gaps

**The model is Meta's own, on the Meta default attribution window, last touch inside the platform.** No override is set at the org level; every pull in this build returned `attribution: Meta default` with `matchesOrgDefault: true`. **Verified.** The brand confirmed it reads performance in-platform: *"In-platform, Meta Ads Manager. No third-party attribution."* **Stated**, intake.

**Where it goes blind, in order of how much it costs.**

**One, everything after the form.** The lead is the last thing Meta sees. Whether it was reachable, qualified, quoted, closed or refused happens on a phone call at a partner agency and never returns. This is the whole of gate two and it is 100% dark.

**Two, the disqualification rate.** A meaningful share of the leads this account buys are people the product screens out, and the account cannot see how many. Pregnancy is the widest and longest-running objection in the comment corpus at 42 comments across 15 ads over fourteen months, and medical underwriting screens her out. Chronic conditions do the same. **Verified.** Nobody has connected the disqualification rate to the cost per lead, and if it is meaningful, then the north-star metric has been rewarding creative that recruits people the funnel turns away.

**Three, the destination break.** Not an attribution model failure but a measurement failure with the same effect: for two and a half weeks, one destination made good creative look like a $273 lead. **Verified.**

**Four, no view-through visibility worth reading.** With one platform and no multi-touch tool, there is no way to see whether an ad seen in August contributed to a form fill in November. For a purchase with an Open Enrollment deadline attached, that window is exactly where the delay lives.

## Attribution stack

**There is no attribution stack. There is Meta Ads Manager.** No third-party attribution tool, no blended business dashboard, no post-purchase survey, no marketplace reporting, no retail sell-through. Northbeam is not connected, confirmed independently by the Phase 0 surface test and by the `northbeam_enrichment: not_connected` flag on every period pull in this build. **Verified.**

What exists beyond the platform's own reporting is four auto-detected pixel events, `offsite_conversion.fb_pixel_custom`, `.Call`, `.click` and `.invitee_meeting_scheduled`, with **zero equation-based metrics defined**. **Verified**, `list_custom_metrics` 2026-09-04. Two of those four are interesting rather than useful at current volume: `.Call` fired 42 times in the window and `.invitee_meeting_scheduled` implies a booking step somewhere in the funnel that nobody in this brain has described. Both are worth understanding, and neither carries enough volume to steer by.

**The practical consequence.** The brand's working numbers and Parker's numbers should agree exactly, since both read the same Meta report on the same window. That is a real benefit of a thin stack and it should be said plainly. The cost is that the platform grades its own homework, and there is no second reading of any kind to check it against.

## Blended vs channel-level reporting

**With one channel, blended and channel-level are the same number, which removes the usual risk and creates a different one.** The classic failure this section guards against is a brand reading one smooth blended figure across many channels and losing sight of what each is doing. That cannot happen here.

The failure that *does* happen here is one level down: **blending across destinations.** August's headline cost per lead was $21.51. Strip the broken destination and 95.2% of the spend read $20.55 while the rest read $341.07. **Verified.** The blend moved the account from the edge of "good" into the middle of "meh" on the strength of a redirect nobody was watching. The same thing recurred in the week to 2026-09-04, where the blend read $25.57 and the clean segment read $21.98.

**So the standing reporting rule for this brand: always segment by landing destination before quoting a cost per lead, and say which segment the number describes.** A blended figure that mixes a 9% landing rate with an 85% landing rate is not a performance number, it is an average of two different things.

## In-store and retail attribution gap

**There is no retail. Health For Moms sells no physical product, has no shelf presence, no wholesale and no marketplace listing.** So the retail attribution gap this section normally covers does not exist here, and inventing one would be a fabrication.

The structurally equivalent gap does exist, and it is worth naming in the slot the retail gap usually occupies, because it does exactly the same damage. **A purchase that happens on a shelf after an ad did its job is invisible to the ad platform. So is a health plan sold on a phone call by a licensed advisor at a partner agency after this account paid for the lead.** The ad numbers understate the creative in exactly the way the retail gap understates it, for exactly the same reason: the conversion happens somewhere the pixel cannot follow.

Two consequences follow, and both are real openings rather than complaints. First, **the brand has no mechanism to follow up with the people who converted at the agency**, because they are not a customer list this account can see or exclude. That means the account may be paying to re-reach people it already converted, and there is no way to check, since frequency is not returned. Second, and more usefully, **the fix is not a tool, it is a handshake.** A single number coming back from the partner agencies, the share of leads that reached a quote, by ad or even by week, would close the largest measurement gap in this business. That is the highest-value reporting improvement available to this brand, and it costs nothing but a conversation.

## Open loops

**1. Nobody knows what happens to a lead after it leaves.**
The account has produced 39,569 leads in twenty-one months and Parker cannot see what became of any of them. The pixel's only shadow is a `Call` event that fired 42 times against 4,336 leads in the last 90 days, and the brand's own winner definition has two gates with the second one entirely outside Meta.
*Pull: Gap.* It fired when the custom-metric list came back with four auto-detected pixel events, no formulas and no revenue metric of any kind, in an account whose north star has a second gate written into it.
**Question: What happens to a Health For Moms lead after it reaches the partner agency?**
Every recommendation in this brain currently clears half the brand's own bar, and if a meaningful share of leads is being disqualified downstream then the metric the whole account steers by has been rewarding the wrong creative. **This one only the brand can answer.**
*Territory: Product.*

**2. There is no ceiling, so nothing can be called too expensive.**
The brand's tiers say a $22.63 lead is "meh," but no customer value, gross margin, lifetime value or max tolerable cost per acquisition was ever captured, so the tiers are a preference rather than a profit line. The account has been in the "meh" band for six straight months and nobody can say whether that is survivable or comfortable.
*Pull: Curiosity.* A brand with a precise four-tier grading scale and no unit economics behind it is grading itself against a number whose origin nobody in this brain can explain.
**Question: What is one lead worth to this business?**
Without it, "efficiency first" means efficiency relative to the account's own trailing number, which drifts, rather than to a threshold that holds. **This one only the brand can answer.**
*Territory: Product.*

**3. December is where the season turns against this brand, and nothing is being planned for it.**
The Open Enrollment window is measured now rather than assumed. November 2025 raised CPM 31.6% and CTR 41.3%, so cost per lead moved only 6.6% and November was the year's biggest lead month. December then hit a $29.34 CPM, the most expensive of thirteen months, cost per lead rose 39.8% to $18.28, and the share of landing page views becoming leads fell from 17.1% to 14.2% on largely the same creative and the same funnel.
*Pull: Surprise.* November behaved almost exactly as the category predicted and December did the opposite of what a rising-demand month should do, on a near-controlled comparison.
**Question: What is different about the mother who clicks in December compared with the one who clicks in November?**
Read through `seasonality.md`, the useful question in a season is never whether demand spikes but what shifts underneath it, and this brand's own numbers say something about the buyer changes between those two months. The answer decides whether December gets budget, different creative, or neither.
*Territory: Personas.*

**4. The number this team steers by did not move through a total creative overhaul.**
Cost per lead went $22.65 to $22.63 across two quarters while spend fell 73.5%, the dominant format changed, the dominant emotion swapped, the awareness posture inverted and hold rate fell from 11.09% to 3.83%. The one metric everyone watches was the one metric that stayed still.
*Pull: Tension.* A metric that survives that much upheaval untouched and a creative overhaul that large cannot both be describing the same account honestly.
**Question: What would tell this team that its creative got better, if cost per lead cannot?**
Every brief, every test verdict and every scale decision in this brain currently gets graded against a number that appears nearly blind to the thing it is grading.
*Territory: Messaging.*

**5. Three quarters of the budget disappeared and the account shows no scar.**
Monthly spend went from $156,716 in April to $18,390 in July and back to $42,749 in August, a 73.5% fall across the quarter, while cost per lead moved one cent. Leads fell by exactly the same percentage as spend, which is what a tap being turned down looks like rather than a machine breaking.
*Pull: Surprise.* A collapse that size normally leaves a mark on efficiency somewhere, and this one left none at all.
**Question: What drove the drop in monthly spend from April through July?**
Whether it was a budget call, a limit on how many leads the partner agencies could absorb, or something else entirely changes what the word "scale" can even mean for the November push. **This one only the brand can answer.**
*Territory: Product.*

## Appendix - Parker media links

Links and paths preserved exactly as returned by the Parker MCP.

**The provisional gate-one candidates**

**`moms-63 2b`** — the cheapest lead at meaningful spend, $5,529.74 for 417 leads at $13.26, 40.15% hook, 2.39% hold, $21.33 CPM. Created 2026-08-14.
Facebook ad id: 120247093361410519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
Landing page: https://www.healthformoms.co/save/

**`moms-63 3e`** — $5,448.56 for 353 leads at $15.44 on an $18.74 CPM, the cheapest impressions of any real spender, and the account's current top spender at $3,638.53 in the trailing week. Created 2026-08-14.
Facebook ad id: 120247093478820519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4
Landing page: https://www.healthformoms.co/save/

**`moms-53 3`** — $2,041.29 for 127 leads at $16.07, with a 3.15% CTR and a $0.69 cost per link click, both the best in the account. Created 2026-08-25.
Facebook ad id: 120247254787160519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4
Landing page: https://www.healthformoms.co/save/

**The incumbent and the aging read**

**`Moms43 - 4 - V3`** — $43,119.77 over the 90 days for 1,935 leads at $22.28, and $3,543.83 in the trailing week for 109 leads at $32.51 on a $27.32 CPM with hook rate unchanged at 46.11%. Lifetime $57,506.21 for 2,668 leads at $21.55. 116 page likes against 1,987,158 impressions. Created 2026-04-15.
Facebook ad id: 120241073380060519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

**The destination evidence**

**`Moms Nahuel WV#1 - V9 - Copy`, broken variant** — $1,639.35, 690 link clicks, 63 landing page views, 9.1% landing rate, 6 leads, $273.23 cost per lead, click quality 9.13. Created 2026-08-17.
Facebook ad id: 120247145872230519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872230519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Landing page: https://go.healthformoms.co/save/

**`Moms Nahuel WV#1 - V9 - Copy`, working variant** — identical video file. $404.23, 213 link clicks, 171 landing page views, 80.3% landing rate, 21 leads, $19.25 cost per lead, click quality 80.28. Created 2026-08-11.
Facebook ad id: 120247022199760519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247022199760519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Landing page: https://www.healthformoms.co/save/

**`Moms Nahuel WV#1 - V9 - Copy`, quiz variants** — $0.94 on 63 impressions and $0.60 on 17 impressions, both created 2026-09-02. Unmeasured.
Facebook ad ids: 120247367204750519 and 120247373812940519
Landing page: https://quiz.healthformoms.com/#/indvfam

**The static library, dark since June**

**`B1 samar- Copy`** — $54,224.86 lifetime across 39 variants, 4,441 leads at $12.21, $16.18 CPM. Created 2025-07-17.
Facebook ad id: 120228910482200519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120228910482200519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/59bf52c09c6081e3dfc63e0b17e649c989b490ad5b03079e469d1dc258e2cc0f.jpg
Landing page: https://www.healthformoms.co/save/

**`B1 - Copy 7`** — $30,339.32 lifetime across 5 variants, 2,584 leads at $11.74, $15.89 CPM. Created 2025-02-26.
Facebook ad id: 120216241083030519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120216241083030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/7e3133fccf8b205622146f7297669b76296123fb46177e5262ee89f0040ca8ba.jpg
Landing page: https://www.healthformoms.co/save/

**`B1 samar- Copy 1`** — $14,633.08 lifetime, 1,231 leads at $11.89, $15.05 CPM. Created 2025-07-17.
Facebook ad id: 120227092759640519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227092759640519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b219b0aa7f7e7ed8d83fa471803f4b6c96ad98b2de118b2a8e68038439e759a9.jpg
Landing page: https://www.healthformoms.co/save/

**The attention-versus-cost contrast**

**`moms54-3`** — the account's best attention numbers and one of its worst costs. 57.02% hook rate, 13.66% hold rate, $29.85 cost per lead on $1,283.69 at a $36.78 CPM. Created 2026-08-13.
Facebook ad id: 120247063711860519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063711860519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/5a62b11062812d9509cb2cd8c95e89777a15d1a6ac1cdb1f6e9a92eb77f93a9d.mp4
Landing page: https://www.healthformoms.co/save/

**Non-media sources**

**Custom metric definitions** — retrieved through Parker MCP `list_custom_metrics` for brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977` on 2026-09-04. Four auto-detected pixel events, zero formulas. No public link; reproduced by that call.

**Brand context document** — retrieved through Parker MCP `get_brand_persona` for brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`. Source of the cost-per-lead tiers and the stated objectives. No public link; reproduced by that call.

**Funnel destinations observed in this build**

- https://www.healthformoms.co/save/
- https://go.healthformoms.co/save/
- https://quiz.healthformoms.com/2
- https://quiz.healthformoms.com/#/indvfam

---

This is everything I know about Andromeda v2.

This is everything I know about seasonality in creative.

This is everything I know about tailoring creative strategy to brand size.
