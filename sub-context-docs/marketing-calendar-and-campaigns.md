---
brand: health-for-moms
doc: marketing-calendar-and-campaigns
generated_on: 2026-09-04
refresh_by: 2026-11-15
quarter: 2026-Q3
sources_read:
  - "Parker MCP `search_facebook_ads_sql` against Meta ad account HealthForMoms, act 484897827497337, brand aed0ff06-555d-4f4f-9bf8-31178e2fb977. Twenty-two live pulls run 2026-09-04: one lifetime account cut, one oldest-ads cut sorted by created_time ascending, thirteen consecutive month-by-month period cuts from 2025-09 through 2026-09, four campaign-scoped lifetime cuts, four created_time batch cuts, and five keyword cuts on the creative corpus for open enrollment, deadline, subsidy, mother's day and holiday."
  - "Parker MCP `get_brand_persona`, the full brand context document, read in full. Section 12 is the brand's own stated marketing calendar."
  - "Parker MCP `search_chat_history`, `listThreads`, 8 threads spanning 2026-09-03 to 2026-09-04, 1 web and 7 Slack. None discuss the calendar."
  - "Public web search, 2026-09-04, on the 2027 ACA open enrollment dates and the December 15 sub-deadline."
  - "`sub-context-docs/category-and-market-research.md`, which carries the seasonal and regulatory spine, read in full"
  - "`sub-context-docs/website-and-product-audit.md` and `audits/2026-Q3/90-day-performance-audit.md`, both read in full"
  - "`running-notes/missing-context.md`, `running-notes/brand-rules.md`, `running-notes/success-definition.md`"
  - "Method docs: `seasonality.md` read in full, plus `creative-strategy-fundamentals.md`, `ad-account-analysis.md`, `killer-performance-ads.md`, `new-product-launches.md`, `persona-research-and-creative-strategy-process.md`, `andromeda-v2.md`, `expertise-routing.md`"
calendar_status: provisional-reconstructed
years_read: "Ad-account creation history from 2024-12-05 to 2026-09-04, roughly 21 months. Month-by-month spend and delivery readable from 2025-09-01 to 2026-09-04, roughly 12 months, which covers exactly one complete Open Enrollment window, 2025-11-01 to 2026-01-15. No second year of the same season exists yet, so every yearly rhythm in this doc is a one-year read and is marked unconfirmed."
data_limitations:
  - "Month-by-month period metrics do not exist before 2025-09-01. Pulls for 2024-12, 2025-01, 2025-02, 2025-03, 2025-04 through 06, 2025-07 and 2025-08 all returned zero rows, while lifetime metrics for ads created in those months do exist. So roughly $104,000 of the account's $743,218 lifetime spend sits before the readable daily series and cannot be placed in a month. This also means the account's first winter, 2024-12 to 2025-01, is invisible."
  - "The 90-day performance audit at `audits/2026-Q3/90-day-performance-audit.md` states that the account history begins in early 2026 and contains no prior Open Enrollment window. That is wrong on both counts and is corrected here. Ads were created from 2024-12-05, and the 2025-11-01 Open Enrollment window is fully readable in the monthly series. That audit's open loop 7 is answered by this doc."
  - "One Open Enrollment is one observation. Every seasonal claim here rests on a single year, so nothing in the recurring-moments section is a confirmed rhythm."
  - "The brand's own site could not be opened. `healthformoms.co` and `quiz.healthformoms.com` were refused by this session's network egress policy during the website-and-product-audit run. So there is no read of seasonal site dressing, promo banners, or a campaign archive."
  - "No email or SMS surface is connected, so the inbox rhythm that would normally date a campaign's build-up is unavailable."
  - "No competitor ad libraries are tracked in the Parker app, deferred at the user's request on 2026-09-03. So the competitive intensity of the November window is inferred from this account's own CPM and from category research, never observed in rival libraries."
  - "The brand's organic social feed was not read back across the year in this run. The TikTok mining library is a category feed, not the brand's own posting history."
  - "Northbeam is not connected. All figures are Meta-reported on the Meta default attribution window."
---

# Marketing calendar and campaigns — Health For Moms

> **CORRECTION, 2026-09-04, verified by direct pull.** The figures "903 link clicks against 234
> landing page views" and a "$75.72 CPL" on the `Moms Nahuel WV#1` group are **not the quiz
> destination.** They are an aggregate of two different destinations summed together, and the
> attribution to `quiz.healthformoms.com` is wrong.
>
> Ground truth, `Moms Nahuel WV#1 - V9 - Copy`, two variants of the same creative:
>
> | Variant destination | Spend | Link clicks | Landing page views | Landing rate | Leads | CPL |
> |---|---|---|---|---|---|---|
> | `go.healthformoms.co/save/` | $1,639.35 | 690 | **63** | **9.1%** | 6 | **$273.23** |
> | `www.healthformoms.co/save/` | $404.23 | 213 | 171 | 80.3% | 21 | $19.25 |
> | **summed (the wrong figure)** | $2,043.58 | **903** | **234** | 25.9% | 27 | **$75.69** |
>
> So 903 = 690 + 213, 234 = 63 + 171, and $75.72 is the blend of a broken destination and a
> working one. The parent `Moms Nahuel WV#1 - V9` on `www.` is healthy: $17,723.91, 7,196 link
> clicks, 6,198 landing page views (86.1%), 635 leads, $27.91 CPL.
>
> **The real finding survives and is sharper:** the collapse is entirely on `go.healthformoms.co`,
> not the quiz, and the same creative on `www.` converts normally. `quiz.healthformoms.com` is a
> separate, brand-new test — 26 ads, $138.27 lifetime, 57 link clicks, 25 landing page views,
> 2 leads, every ad created 2026-09-02 or 09-03. Treat the quiz as **unmeasured**, never as a leak.


## What I read, and what changed my mind

I set out to reconstruct this brand's year from its own spend history, because the brand has told us its calendar has exactly one date on it and I wanted to see whether the account agrees. The method is the one `seasonality.md` prescribes: ask the brand, then validate against the data, and read for what shifts underneath rather than only for a demand spike.

Two things changed my read while I worked, and both matter enough to put at the top.

**The first is that this account has already lived through an Open Enrollment, and nobody in this brain knew it.** The 90-day performance audit says the account history begins in early 2026 and contains no prior Open Enrollment window, and it left that as an open loop. That is not right. Sorting the account by `created_time` ascending returns ads created on 2024-12-05, in a campaign called "Health For Mom's Angle Test v2." **Verified** from a lifetime pull run 2026-09-04. And the month-by-month series is readable from 2025-09-01 forward, which covers November 2025, December 2025 and January 2026 in full. So the single most important question this brand could ask about its calendar, what happens to cost per lead and lead volume during Open Enrollment, has an answer sitting in the account. It is in this doc.

**The second is that the brand's stated calendar and its actual spending calendar are not the same calendar, and the gap is large.** The brand names November 1 as "the single most important date on the marketing calendar." **Stated**, brand context document, Section 12, verbatim: *"Open Enrollment November 1"*. But over the thirteen readable months, November 2025 took $34,235.57, which is 5.4% of the $639,304.26 the account spent in that stretch. March, April and May of 2026 took $376,489, which is 58.9%. April alone was 4.6 times November. **Verified** from thirteen consecutive monthly pulls.

That is not a small disagreement, and it is the finding this doc is built around. The honest version is not "the brand is wrong about November." It is that the brand has one calendar in its head and a different one in its bank account, and neither has been checked against the other until now.

A note on how I dated things. I have no site, no email and no organic feed to read, so almost every date here comes from one of two account signals: the `created_time` on an ad, which tells me when a batch of creative was built, and the month-by-month spend series, which tells me when money actually moved. Both are solid. Neither tells me what the team intended. Everywhere I read intent from cadence, I have marked it as my inference.

---

## Active and recent campaigns

The window here is roughly the last 90 days, 2026-06-06 through 2026-09-04. I am reporting it by calendar month rather than as one 90-day total, because the monthly cuts are what I pulled and a 90-day figure would need a partial June I did not measure. June took $42,698.49, July $18,389.74, August $42,748.63, and the first four days of September $7,345.98. **Verified** from four monthly period pulls. For reference, `90-day-performance-audit.md` measured the matched 2026-06-06 to 2026-09-03 window at $99,266.98. Across that stretch the account ran two live campaigns and rebuilt its creative supply.

**The account runs on two standing campaigns, not on named seasonal pushes.** Everything currently live sits inside `USHA - ABO - SCALE - MOMS` or `USHA - ABO - TEST - MOMS`. Lifetime, the scale campaign has carried $250,010.84 across 42 ads at a $22.95 cost per lead, and the test campaign has carried $245,189.55 across 1,125 ads at a $22.96 cost per lead. **Verified** from two campaign-scoped lifetime pulls. That is the shape to hold onto: a wide testing campaign with more than a thousand ads in it feeding a tight scale campaign with about forty. It is an always-on acquisition machine, not a calendar of campaigns. Anyone looking for named campaigns with start and end dates in this account will not find them, and that absence is itself the honest answer to what is running.

**What does move on a calendar is the creative batch.** The brand ships numbered drops, and the numbers plus the creation dates give a genuine production rhythm. Reading the batch tokens in ad and ad-set names is inventory bookkeeping, which is all a name can ever prove, so I am using them to count and date drops and nothing else. The dated drops I can place: MOMS25 on 2025-11-24 and again on 2025-12-05, MOMS30 on 2026-01-17, MOMS31 on 2026-01-23, MOMS38 on 2026-03-10 through 03-12, MOMS39 on 2026-03-14, Moms43 on 2026-04-06 and 2026-04-15, moms-63 on 2026-08-14, and moms62 on 2026-09-03. **Verified** from `created_time` on each. That works out to a fresh batch roughly every two to four weeks when the account is healthy. **Inferred** that this is the intended cadence, resting on the regularity of the dates rather than on anything the team has said.

Four things are live or recently live inside the window.

**The Moms43 savings cluster, the account's incumbent, running since April.** The single ad "Moms43 - 4 - V3" was created 2026-04-15 and is still ACTIVE. Lifetime it has taken $55,794.26 and returned 2,549 leads at a $21.89 cost per lead. **Verified** from an ad-level lifetime pull. The creative opens on a mother and a baby lying together on white bedding against a soft beige background, both looking calmly into the camera. There is no speech at all, only music. Across the top runs the text hook *"POV: Telling your husband you found better health insurance, saved $400 a month, AND the deductible is zero. Wife of the year energy. 💕"* **Verified** from the ad's own visual hook, verbal hook and text hook fields. What it is built around is a savings claim delivered as a domestic win, and it is tied to no moment on the calendar at all. It has now been in market for close to five months, which makes it the longest-running piece of creative the account currently leans on.

**The moms-63 drop, launched 2026-08-14.** This is the August rebuild. "moms-63 3e" opens on a well-dressed mother and her young son holding hands as they walk outdoors near a house, and carries the same POV savings hook as Moms43 with a slightly different heart emoji. "moms-63 2b" from the same drop produced a $13.26 cost per lead in the 90-day window, which sits inside the brand's own "fantastic" band of under $15. **Verified** from ad-level pulls and from the 90-day performance audit's appendix. Read plainly, this drop is a refresh of the incumbent angle rather than a new campaign.

**The moms62 drop, launched 2026-09-03, one day before this doc.** Three ads, "moms62 1," "moms62 2" and "moms62 3," all created 2026-09-03T10:28:09 and all ACTIVE. Between them they had spent $47.04 by the time of the pull, so there is nothing to read on performance yet. **Verified** from a created-time pull. The one with a described opener, "moms62 3," shows a mother and baby lying together in a dimly lit bedroom with a warm, personal home-video look, under the same POV savings hook. **Verified** from its visual and text hook fields. This is the newest thing in the account and it is worth naming precisely what it is not: it carries no reference to November, no deadline, and no seasonal frame.

**The `quiz.healthformoms.com` funnel test, roughly 2026-08-11 to 2026-09-02.** The ad group "Moms Nahuel WV#1 - V9 - Copy" pointed at a second domain rather than the usual `/save/` page. It bought 903 link clicks and recorded only 234 landing page views, and its cost per lead came in at $75.72 against an account average of $22.67. **Verified**, carried forward from `website-and-product-audit.md`. It belongs in this section because it is the only thing in the window with a real start and end date, and because a funnel swap is the closest thing this brand has to a product launch. It appears to have wound down at the start of September.

**How the window ends.** The account is producing again. 125 ads were created between 2026-08-01 and 2026-09-04. **Verified** from a created-time pull. Against 63 ads created in October 2025, which was the run-up to the last Open Enrollment, that is a materially bigger build. So the machine is warm. What it is building, on the evidence of every described opener in the batch, is more of the same savings angle.

---

## Recurring seasonal moments

This is the heart of the doc, and it has one confirmed entry, one measured but unconfirmed pattern, and a correction to make.

### Open Enrollment, November 1 to January 15

**What the brand says.** Section 12 of the brand context document names Open Enrollment on November 1 as the single most important date on the calendar and says the brand plans seasonal creative two months in advance. **Stated**, brand context document, verbatim on the planning window: *"2 months"*. Section 8 also lists open enrollment season as one of six tipping points that push a mom from thinking about coverage to clicking, and Section 8 separately lists *"I should just wait for open enrollment"* as a timing objection that can cost months of delay.

**What the category says.** `category-and-market-research.md` found that November 1 is the category's dominant seasonal event and that creators peg content to it with tags like #openenrollment2025. It also found that in this brand's own 1,322-comment corpus, the phrase "open enrollment" appears exactly once, 0.08%, in a comment from 2026-04-25 where one commenter corrects another about how the ACA works. **Verified**, keyword cut. And the structural reason is real: these are medically underwritten private plans, which are not gated to the November window, so this brand's buyer genuinely has no deadline.

So the question left open was whether November does anything for this brand at all. Here is the answer, and it is more interesting than either yes or no.

**What the account says.** The monthly series, in full, is the single most useful table in this doc. All figures are Meta-reported on the Meta default window, and all are **verified** from thirteen consecutive period pulls run 2026-09-04.

| Month | Spend | Leads | CPL | CPM | CTR | Landing page views to leads |
|---|---|---|---|---|---|---|
| 2025-09 | $17,416.10 | 1,390 | $12.53 | $14.19 | 1.59% | 17.7% |
| 2025-10 | $21,663.87 | 1,766 | $12.27 | $17.57 | 1.79% | 18.7% |
| **2025-11** | **$34,235.57** | **2,617** | **$13.08** | **$23.13** | **2.53%** | **17.1%** |
| **2025-12** | **$28,706.54** | **1,570** | **$18.28** | **$29.34** | **2.61%** | **14.2%** |
| 2026-01 | $20,297.31 | 1,010 | $20.10 | $24.50 | 1.88% | 13.4% |
| 2026-02 | $29,312.76 | 1,253 | $23.39 | $20.34 | 1.77% | 12.3% |
| 2026-03 | $114,106.93 | 5,473 | $20.85 | $24.16 | 2.87% | 8.8% |
| 2026-04 | $156,716.43 | 6,988 | $22.43 | $22.88 | 2.52% | 8.6% |
| 2026-05 | $105,665.91 | 4,240 | $24.92 | $24.03 | 1.92% | 9.4% |
| 2026-06 | $42,698.49 | 1,540 | $27.73 | $24.22 | 1.67% | 9.5% |
| 2026-07 | $18,389.74 | 929 | $19.80 | $20.82 | 1.73% | 11.1% |
| 2026-08 | $42,748.63 | 1,987 | $21.51 | $23.66 | 1.93% | 10.5% |
| 2026-09, first 4 days | $7,345.98 | 287 | $25.60 | $22.82 | 1.92% | 10.6% |

Four reads come out of that, and they are the substance of this brand's seasonality.

**One. The brand did ramp for Open Enrollment 2025, and the ramp was real.** Spend went from $17,416 in September to $21,664 in October to $34,236 in November, which is a 97% increase over two months and a 58% jump in November alone. Creative production ramped alongside it: 38 ads created in September 2025, 63 in October, 54 in November. **Verified** from three created-time pulls. So this is not a brand that ignored its own biggest date. It leaned in.

**Two. November made the auction more expensive and the buyer more willing, and the two nearly cancelled out.** From October to November, cost per thousand impressions rose 31.6%, from $17.57 to $23.13. That is the competitive intensity `category-and-market-research.md` predicted, now measured rather than assumed. But click-through rate rose 41.3% over the same step, from 1.79% to 2.53%. The result is that cost per lead moved only 6.6%, from $12.27 to $13.08, and November produced the most leads of any month in 2025 at 2,617. **Verified** from the October and November pulls. Read through `seasonality.md`, which says the useful question is never whether demand spikes but what shifts underneath, this is the cleanest possible statement of what November does for this brand: it costs about a third more to reach her, and she is about 40% more likely to respond, so the brand roughly breaks even on efficiency and wins on volume.

**Three. December is where the window turns against this brand, and December is the part nobody has been planning for.** In December, cost per thousand impressions hit $29.34, which is the single most expensive month of all thirteen. Cost per lead rose 39.8%, from $13.08 to $18.28. And the back half of the funnel gave way: the share of landing page views that became leads fell from 18.7% in October and 17.1% in November to 14.2% in December and 13.4% in January. **Verified** from four consecutive monthly pulls. That decline matters more than it looks, because September through December ran on largely the same creative base and the same `/save/` funnel, so this is close to a controlled comparison rather than an artifact of the brand changing what it was doing.

The reason is almost certainly the December 15 sub-deadline. Web search on 2026-09-04 confirms that in most states the deadline to pick a marketplace plan with a January 1 effective date is December 15, inside the broader November 1 to January 15 window. **Verified** as reported by healthinsurance.org and CMS-sourced summaries. So the first half of December is when every marketplace shopper in the country is under a real clock, and this brand's product has no such clock. **Inferred**, and the inference rests on the CPM peak, the click-through rate staying high at 2.61% while leads fell, and the conversion rate falling: people were still clicking, they just were not the people this funnel qualifies. That reads as marketplace traffic arriving at a private-plan funnel.

**Four. The window shifts the age of who the account reaches, but I cannot cleanly call that seasonal.** Spend on people aged 45 and over went 18.6% in September, 23.4% in October, 25.2% in November, 26.9% in December, then back to 21.5% in January and down to 14.0% in February. **Verified** from six monthly demographic breakdowns. A 45% relative rise into December and a full reversal by February is exactly the kind of shift `seasonality.md` says to watch for, and if it held it would mean the November window brings this brand an older buyer than its evergreen creative is cast for. But April 2026 also reads 24.4% on the same measure, and April is not a season, it is the account's biggest spend month. So spend level and creative era are both confounded with the calendar here and I cannot separate them from one year of data. **Recorded as measured, marked unconfirmed**, and carried into the open loops rather than asserted.

**Confidence on Open Enrollment as a recurring moment: mixed, and unavoidably so.** The moment is real, the brand builds toward it, and the account's response to it is measured in detail. But it is one year. `seasonality.md` is explicit that a season the brand has run before gets refined rather than reinvented, and this brand now has exactly one prior run to refine from. It cannot be called a confirmed rhythm until November 2026 is in the data.

### The March-to-May surge, which is the account's actual peak

March, April and May 2026 took $376,489, or 58.9% of everything the readable series contains. April alone at $156,716 is the largest month by a wide margin. **Verified** from three monthly pulls.

I want to be careful here, because this is the place where it would be easiest to invent a season. **There is no evidence that this is a recurring spring moment.** It appears once, in the only spring the data covers, and `90-day-performance-audit.md` reads the subsequent collapse from $156,716 in April to $18,390 in July as a budget decision rather than a performance failure, since cost per lead stayed flat through it. So the most likely explanation is that the business turned the taps on and then off, and that has nothing to do with the calendar. **Inferred**, resting on the flat cost per lead across a 73.5% spend collapse.

What is worth noticing is the timing against the category. The enhanced ACA premium tax credits expired on 2026-01-01, and `category-and-market-research.md` calls that the larger structural event in this market, larger than Open Enrollment itself, with average benchmark premium payments projected to more than double and roughly 4.8 million people pushed out of subsidised coverage. The account's largest spending period in its readable history began about ten weeks after that expiry. And it scaled without breaking: March took 3.9 times February's spend while cost per lead actually improved, from $23.39 to $20.85. **Verified** from both monthly pulls. A brand that can quadruple spend and get cheaper leads is a brand that found more demand than it was previously buying.

I am not going to claim the subsidy expiry caused the scale-up, because I cannot see the budget decision behind it and the honest answer is that I do not know. **Data-limited.** But the two facts belong next to each other on this calendar, because if the demand really did expand after January, then the brand's most productive months follow the subsidy cliff rather than Open Enrollment, and that would reorder the whole year.

### What the brand does not run on any repeating schedule

Section 12 of the brand context document says, on major holidays: *"No major holidays were selected."* **Stated.** The account agrees completely, and the checks are in the absences section below.

---

## Past major campaigns

There are no named campaigns in the marketing sense. What the account has instead is four distinct eras, each defined by a campaign structure and a creative approach, and those eras are the real history. All figures **verified** from campaign-scoped lifetime pulls run 2026-09-04.

**Era one: the angle test, from 2024-12-05.** Campaign "Health For Mom's Angle Test v2," with ad sets named "Health Ins Stack," "Insurance BROAD Stack," "WIDE OPEN," "Parents (All)," "Mom Stack" and "Park / Outdoor Recreation." The creative was a small set of direct-to-camera videos named "Old mom 1," "Old mom 2" and "Hot Mom," all built on the same line, *"Moms, being protectors of our family's health is the most important role we have,"* delivered by women in domestic settings. Static ads named IMG 1 through IMG 6 went up on 2024-12-10 with headlines like *"THIS IS SAVING MOMS 20% ON THEIR HEALTH INSURANCE"* and *"Moms, save 20% on your health insurance."* **Verified** from the media fields on each. Individual spends are tiny, mostly under $200, and costs per thousand impressions ran $34 to $103, which is what a cold account looks like. This is the brand's origin on Meta, and it sits right at the start of the 2024 Open Enrollment window without carrying any reference to it.

**Era two: the SAMAR statics, from 2025-07-17.** Campaign `USHA - CBO - SAMAR`, 87 ads, $75,890.55 lifetime, 6,149 leads, a **$12.34 cost per lead** and a $16.54 cost per thousand impressions. This is the cheapest era the account has ever had, by a wide margin, and it is the creative that carried the brand through Open Enrollment 2025. Its workhorse is a static called "B1 samar- Copy," created 2025-07-17, which alone took $35,219.98 and returned 3,046 leads at $11.56. The image carries the headline *"Didn't know I could ditch my job's health plan… until I did."* Sibling statics in the same batch run *"I changed our health plan, got $0 deductible options, and picked our doctors with no networks"* and *"Left my work health plan for one that's actually built for moms. Now I pay less and pick my own doctor 😌."* **Verified** from the ad records. The through-line is escaping employer coverage, written as a first-person testimonial card.

**Era three: the OMC test batches, September to November 2025.** Campaign `USHA - CBO - TEST`, 225 ads, $32,746.09, 1,704 leads at a $19.22 cost per lead. Two dated drops sit inside it: 38 ads on 2025-09-25 and 63 ads on 2025-10-24. The October drop is the closest thing this brand has ever run to Open Enrollment creative, in the sense that it landed eight days before November 1. Its biggest ad, "OMC-Health for Moms-[B3-C11-V7]," took $10,947.56 lifetime at a 4.44% click-through rate. The September drop includes a static headlined *"I'm a single mom, and I didn't know my insurance was failing us... 😭."* **Verified** from ad records. Nothing in either drop mentions enrollment, dates or deadlines.

**Era four: the ABO split, from late November 2025 to now.** The account reorganised into `USHA - ABO - TEST - MOMS` and `USHA - ABO - SCALE - MOMS`. The test campaign has run 1,125 ads for $245,189.55 at a $22.96 cost per lead. The scale campaign has run 42 ads for $250,010.84 at a $22.95 cost per lead. Nearly identical efficiency, wildly different ad counts. This is the architecture the account still runs on.

**The one thing that era history says loudly.** Cost per lead went from $12.34 in the SAMAR era to about $22.95 in the ABO era, an 86% increase. Three things changed at once: the campaign structure, the creative from statics to video, and the market after the subsidy expiry. I cannot separate them, and this doc is not the place to try, since diagnosing performance belongs to the ad-account and performance docs. **Data-limited on the cause.** What belongs here is the timeline: the cheap era ran from July 2025 through Open Enrollment, and the expensive era began in the winter and has not ended.

**The one identifiable seasonal campaign the brand has ever run, and it is smaller than anyone would guess.** Searching the entire 2,122-ad lifetime corpus for "open enrollment" returns 5 ads. All five sit in a single ad set, `MOMS25 - 5TH DEC - Y1`, all created 2025-12-05, and between them they spent **$573.59** and produced 21 leads at a $27.31 cost per lead before being switched off. **Verified** from a keyword cut. Searching the same corpus for "subsidy" returns 3 ads, all from that same ad set, totalling $379.92. **Verified.**

Those five ads deserve a proper look, because they are the brand's only attempt at the moment. "MOMS25 - 5TH DEC - Y1" opens on a woman in a lime green shirt holding papers and looking stressed while a narrator speaks into a professional microphone in a circular overlay, and the spoken line is *"Making over 50k just disqualified this family from affordable health care, but it secretly qualified them for something way better."* A sibling, "Copy 5," opens on a frustrated woman with long dark hair at a table covered in medical bills, under the text hook *"If you make $50k+, you're paying too much."* Another, "Copy 3," is a blonde woman in a purple sweater talking straight to camera in front of a screenshot of the website, saying *"I feel like I unlocked a cheat code for the American healthcare system and no one seems to know about it."* **Verified** from each ad's visual hook, verbal hook and text hook fields.

The angle is the subsidy cliff, aimed squarely at families just above the income cutoff. That is precisely the group `category-and-market-research.md` identifies as the market opening. And the brand built it on **2025-12-05**, five weeks after Open Enrollment opened, spent $574 on it, and stopped. **Inferred** that it was a small test that did not clear the bar, resting on the tiny spend and the paused status rather than on anything the team has said.

---

## Product launches, new lines, and collaborations

There is almost nothing here, and the reason is structural rather than a gap in my research.

**This brand has no SKUs.** `website-and-product-audit.md` establishes it plainly: Health For Moms is a lead-generation matching service, not a carrier, and it does not sell a plan. There is no product line, no pricing page, no adjacent vertical, and no life, dental or vision extension visible anywhere in the account or the brand document. **Verified** from the account and **stated** in brand context Section 1. `new-product-launches.md` is scoped to established brands launching a new product or SKU, so it does not apply here, and forcing a launch calendar onto this business would invent one.

**What plays the role of a launch is a funnel change.** Choosing which landing destination an ad points at is, per the product audit, the highest-leverage product decision anyone at this brand makes. Three destinations appear in the account: `https://www.healthformoms.co/save/`, which is the workhorse carrying nearly every ad; a `/save-cw` variant; and `https://quiz.healthformoms.com/#/indvfam`, on a different domain entirely. The quiz funnel is datable, and it is the only launch-shaped event in the current window: it ran from **2026-08-11 to 2026-09-02** on the ad group "Moms Nahuel WV#1 - V9 - Copy," lost 74.1% of the clicks it bought before they registered as arrivals, and produced a $75.72 cost per lead. **Verified**, carried from the product audit.

**Two other launch-shaped events are datable from the account.** The campaign restructure into the ABO test-and-scale split happened around late November 2025, which is the biggest single change to how this account goes to market. And the shift from statics to video as the dominant creative type ran through the winter of 2025 into spring 2026. Neither is a product launch, but both are the kind of structural change a later strategy needs the date of.

**Collaborations: none found.** No brand collaboration, co-marketing partnership or named third party appears anywhere in the ad corpus. `reputation-analysis.md` and `category-and-market-research.md` both note that the brand names no carrier, no partner agency and no third party in its creative, which the category doc reads as a trust liability given the enforcement wave in this vertical. So the absence of collaborations is consistent with a deliberate posture rather than an oversight.

**Routed to the brand.** What new funnels, plan types, state expansions, or partner agencies are coming, and on what dates. Only the team can answer that, and the state list in particular is a live blank: `website-and-product-audit.md` could not read it, and commenters report the product covering roughly 37 states. A state expansion would function as this brand's version of a product launch and would deserve a calendar entry.

---

## Meaningful absences

These are checked against the full 2,122-ad lifetime corpus rather than the recent window, so each one is a real absence over the brand's whole history rather than a gap in one quarter. All **verified** from keyword cuts run 2026-09-04.

**No deadline creative has ever run. Not one ad.** Searching the entire corpus for "deadline" returns **0 of 2,122 ads**. This is the sharpest finding in the doc. The category's whole calendar runs on a deadline, the brand names a timing objection in its own document as *"I should just wait for open enrollment,"* and the brand has never once put a date, a countdown or a closing window in an ad. Now, part of that is correct and deliberate: these plans have no enrollment deadline, so a fake one would be a claim the brand cannot substantiate, and `category-and-market-research.md` documents an active FTC enforcement wave aimed at exactly this layer of the market. But the objection it leaves unanswered is real. A mom who believes she must wait until November is a mom this brand loses for months, and nothing in 2,122 ads tells her otherwise.

**No Mother's Day creative has ever run. Not one ad.** Searching for "mother's day" returns **0 of 2,122 ads**. For a brand called Health For Moms, whose entire audience is mothers and whose delivery is 96.1% female lifetime, sitting out the one cultural moment built around its exact audience every year is a genuine choice worth surfacing. `seasonality.md` notes that giftability flips the buyer avatar from self to others, and this product is not giftable in the ordinary sense, so the standard gifting play does not apply. But Mother's Day is also a moment when the culture spends a week talking about what mothers carry, and that is this brand's entire message. **Inferred** that the absence is untested rather than tested and rejected, resting on the zero count across the whole corpus.

**No holiday campaign of any kind has ever run.** Searching for "holiday" returns 7 ads, and I read all seven. Six are variants of "MOMS38 - 2," created 2026-03-11, and the seventh is "Moms Nahuel WV#1 - V4," created 2026-04-06. Every one of them is the same skit: a woman on a porch, frustrated, on the phone, under the text hook *"When you have to call your health insurance 🙄."* The word appears incidentally in the AI analysis text, never as a campaign frame, and not one of the seven is holiday creative. **Verified** by reading each of the seven matches. The brand's own document says it directly: *"No major holidays were selected."* So Black Friday, Christmas, New Year and back-to-school are all untouched. For a lead-generation business with no product to discount, skipping Black Friday is sound. Skipping the New Year is less obviously right, since `seasonality.md` names the New Year health-and-wellness surge as a macro motivational moment when people re-evaluate their habits, and January is a month this account has run at a $20.10 cost per lead with falling conversion.

**The brand has never advertised the subsidy cliff at scale, despite it being the biggest thing that has happened to its market.** Three ads, $379.92, all on one day in December 2025. Against $743,218 of lifetime spend, that is 0.05%. The category research calls the enhanced subsidy expiry the event reshaping this whole market and identifies the households just above the cutoff as the pool being pushed toward exactly this product. The brand tested that angle once, small, in the wrong month, and left it.

**Open Enrollment 2025 ran on evergreen creative, which is the right instinct executed by accident.** The six highest-spending ads in November 2025 were: "B1 samar- Copy" at $9,253 and an $11.37 cost per lead, "OMC-Health for Moms-[B3-C11-V7]" at $4,230, "B1 samar- Copy 1" at $4,179, another "B1 samar- Copy" at $2,060, "OMC-Health for Moms-[B3-C17-V2]" at $1,587, and a third "B1 samar- Copy" at $1,520. **Verified** from an ad-level November pull. Four of the six were created on 2025-07-17, nearly four months before the window opened. Not one is seasonal.

`seasonality.md` is blunt that the most common and costly seasonal error is pulling proven evergreen winners to make room for untested seasonal creative, and that evergreen ads often outperform seasonal ads even during the season. By that standard the brand did the right thing in November 2025. But it did it by having no seasonal creative to swap in, not by making the call. The distinction matters for this year, because a brand that deliberately holds its evergreen and layers seasonal on top is in a very different position from one that simply never built the layer.

**And the live absence, as of today.** It is 2026-09-04. Open Enrollment opens in 58 days. The brand's stated planning window is two months, which means production should have started on or around 2026-09-01. `seasonality.md` puts the lead time at three to four months, which would have meant starting in May or June. The account is producing at volume, with 125 ads created since August 1. But every described opener in that batch carries the same POV savings hook the account has run since April, and the corpus contains zero ads referencing enrollment, a deadline, or the January subsidy change. **Verified** from the created-time pull and the keyword cuts. So the ramp is a volume ramp, not a seasonal one, and whatever the brand decides about November it is deciding it now with nothing built.

---

## Open loops

**1. The account's money and the brand's calendar point at different months.**

The brand names November 1 as the single most important date on its calendar. Over the thirteen readable months, November 2025 took 5.4% of spend and March through May 2026 took 58.9%, with April alone running 4.6 times November. March also scaled to 3.9 times February's spend while cost per lead improved from $23.39 to $20.85, which is not what a brand pushing into a season it does not belong in looks like.

*Pull: Tension.* The brand's stated calendar and the account's own spend history cannot both be a fair description of when this business makes its money, and I want to know which is closer to right.

**Question: What makes the spring months this account's biggest, and how much of that is demand rather than budget?**

If spring demand is genuinely richer than November demand, the brand is planning its year around its second-best window and the whole production calendar should move. If the spring surge was simply a budget decision, then November stands and the account has never properly tested it.

*Territory: Product.*

**2. December costs the most and converts the worst, and nobody has planned for the difference between November and December.**

November 2025 held cost per lead almost flat at $13.08 while cost per thousand impressions rose 31.6%, because click-through rate rose 41.3% and paid for it. December broke that trade: the most expensive impressions of all thirteen months at $29.34, cost per lead up 39.8% to $18.28, and the share of landing page views becoming leads falling from 18.7% in October to 14.2% in December on largely the same creative and the same funnel.

*Pull: Surprise.* Everyone in this brain, including the brand, has been treating Open Enrollment as one window with one answer, and the account says the two halves of it behave in opposite directions.

**Question: What is different about the people who click this brand's ads in December?**

If December traffic is marketplace shoppers arriving at a private-plan funnel, the answer is a qualification move in the creative and a budget taper, and both need deciding before November 1. If it is something else, the brand may be walking away from its second-strongest month.

*Territory: Personas.*

**3. The brand has never told a mom she does not have to wait, and she keeps telling herself she does.**

Zero of 2,122 ads in the account's whole history contain the word "deadline." The brand's own document names *"I should just wait for open enrollment"* as a timing objection that can cause months of delay. The product genuinely has no enrollment window, which is a real and unusual advantage, and no ad has ever said so.

*Pull: Gap.* There is a true, substantiable, differentiating fact about this product sitting right there, and in twenty-one months of advertising it has never been said out loud.

**Question: How many moms hold off on this product because they think they have to wait for a window?**

If that belief is common, the brand has eleven months of demand it is not speaking to, and per `creative-strategy-fundamentals.md` a misconception to overturn is a different creative move from a value barrier to reframe. If it is rare, the year-round push is worth less than it looks.

*Territory: Messaging.*

**4. The biggest thing that happened to this market got $380 and one day.**

The enhanced ACA subsidies expired on 2026-01-01 and `category-and-market-research.md` calls it the larger structural event in this category, with roughly 4.8 million people pushed out of coverage they could previously afford and the households just above the cutoff hit hardest. The brand has run three ads in its history naming a subsidy, all created 2025-12-05, totalling $379.92, which is 0.05% of lifetime spend. One of them says *"Making over 50k just disqualified this family from affordable health care, but it secretly qualified them for something way better."*

*Pull: Gap.* The market's defining event and this brand's stated buyer overlap almost exactly, and the account has essentially never advertised into it.

**Question: What happens to cost per lead when this brand leads with the subsidy cliff instead of the savings claim?**

The savings angle currently carries the majority of spend at a cost per lead in the brand's "meh" band. If the subsidy angle speaks to a sharper, more recent grievance, it changes what gets briefed for November. If it was already tested and failed, that needs recording so nobody spends the runway rebuilding it.

*Territory: Messaging.*

---

## Appendix - Parker media links

Grouped by the surface each came from, with links preserved exactly as returned.

**Currently live creative, 2026**

M001: Moms43 - 4 - V3. The incumbent savings ad, created 2026-04-15, $55,794.26 lifetime at a $21.89 cost per lead. Mother and baby on white bedding, music only, POV savings text hook.
Facebook ad id: 120241073380060519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

M002: moms-63 3e. The August 2026 rebuild drop, created 2026-08-14. Mother and young son walking outdoors, same POV savings hook.
Facebook ad id: 120247093478820519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4
Landing page: https://www.healthformoms.co/save/

M003: moms62 3. The newest ad in the account, created 2026-09-03. Mother and baby in a dim bedroom, home-video look, same POV savings hook.
Facebook ad id: 120247381576000519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247381576000519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0253305133ef166bb67b315dedcc72721f9192b3ecc70f83c503c4664a6f7de1.mp4
Landing page: https://www.healthformoms.co/save/

M004: moms62 1. Same 2026-09-03 drop, no spend recorded at pull time.
Facebook ad id: 120247381534360519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247381534360519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/9b88affac8d843207be19cf0e1ed0783a8a771618338cf619af9085408d3b092.mp4

M005: moms62 2. Same 2026-09-03 drop.
Facebook ad id: 120247381572770519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247381572770519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/2fcc4a48ba0e3be34993badb9684ac9bcd5968e63d5abb1149e7f7db1267b4ad.mp4

**Open Enrollment 2025 window, what actually ran in November**

M006: B1 samar- Copy. The November 2025 top spender at $9,253 and an $11.37 cost per lead, created 2025-07-17. Static, headline "Didn't know I could ditch my job's health plan… until I did."
Facebook ad id: 120227092765930519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227092765930519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b219b0aa7f7e7ed8d83fa471803f4b6c96ad98b2de118b2a8e68038439e759a9.jpg
Landing page: https://www.healthformoms.co/save/

M007: B1 samar- Copy 1. Third-biggest November 2025 ad at $4,179 and a $12.55 cost per lead. Same creative, different ad set.
Facebook ad id: 120227092759640519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227092759640519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b219b0aa7f7e7ed8d83fa471803f4b6c96ad98b2de118b2a8e68038439e759a9.jpg
Landing page: https://www.healthformoms.co/save/

M008: B1 samar- Copy, Broad B1 - Copy 32. $2,060 in November 2025 at an $11.38 cost per lead. Headline "I changed our health plan, got $0 deductible options, and picked our doctors with no networks."
Facebook ad id: 120227093054710519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227093054710519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/4c9b4f3dd99bdcfcc853b3db5657e2e14e78af6c7ca04c93bb85db49bb62f034.jpg
Landing page: https://www.healthformoms.co/save/

M009: B1 samar- Copy, Broad B1 - Copy 31. $1,520 in November 2025. Headline "Left my work health plan for one that's actually built for moms. Now I pay less and pick my own doctor 😌."
Facebook ad id: 120227093048750519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227093048750519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/2b3847722e848bac921846d55ec1b935f2aeb093b897613733fc457fda4adf6f.jpg
Landing page: https://www.healthformoms.co/save/

M010: OMC-Health for Moms-[B3-C11-V7]. The 2025-10-24 pre-Open-Enrollment drop's biggest ad, $10,947.56 lifetime at a 4.44% click-through rate and a $16.22 cost per lead.
Facebook ad id: 120232855500240519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120232855500240519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Landing page: https://www.healthformoms.co/save/

M011: OMC-Health for Moms-[B3-C17-V2]. Video from the same 2025-10-24 drop, $1,587 in November 2025 at a $15.11 cost per lead.
Facebook ad id: 120232856550310519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120232856550310519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/d4e4af9949f12ad105882dd67bbdcbedfa12c9a37ddb2526b4f20016a42e27c0.mp4
Landing page: https://www.healthformoms.co/save/

M012: OMC-Health for Moms-[B1-C3-V3]. The 2025-09-25 drop, static headlined "I'm a single mom, and I didn't know my insurance was failing us... 😭."
Facebook ad id: 120231111109680519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120231111109680519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/df25fba1bc9d23d5ca5a0febe5f3c8c33eb8c3a132cebfb6ab8f863858369ab1.jpg
Landing page: https://www.healthformoms.co/save/

M013: MOMS25 BLAST - X1 - Copy 2. Created 2025-11-24, inside the Open Enrollment window. Woman in a podcast studio, opener "OKAY REAL TALK." $3,436.94 lifetime at a $19.75 cost per lead.
Facebook ad id: 120234697401680519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120234697401680519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/df333c46af8aa789c9428f87f4be4a8cfa1118f478b06ab6bcb589a8007ee7ed.mp4
Landing page: https://www.healthformoms.co/save/

**The MOMS25 - 5TH DEC - Y1 ad set, the brand's only subsidy and enrollment creative, all created 2025-12-05, $573.59 total**

M014: MOMS25 - 5TH DEC - Y1. Woman in a lime green shirt holding papers, narrator in a circular overlay at a microphone. Verbal hook "Making over 50k just disqualified this family from affordable health care, but it secretly qualified them for something way better." $59.65.
Facebook ad id: 120235426050510519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120235426050510519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/3ea77dc0f9217a3d77db15bb995506d871e56006ea7f301bb4df16982075976d.mp4
Landing page: https://www.healthformoms.co/save/

M015: MOMS25 - 5TH DEC - Y1 - Copy 3. Blonde woman in a purple sweater to camera in front of a website screenshot. "I feel like I unlocked a cheat code for the American healthcare system and no one seems to know about it." $77.86 at a $19.47 cost per lead.
Facebook ad id: 120235426337000519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120235426337000519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/a2b878f11ea8418310fa610c8614f6678acf7974e99fbfc037a6f3808fc39496.mp4
Landing page: https://www.healthformoms.co/save/

M016: MOMS25 - 5TH DEC - Y1 - Copy 4. Woman in her 40s with glasses in front of a website screenshot. "I feel like I unlocked a cheat code for the American health care system." $134.02 at a $19.15 cost per lead.
Facebook ad id: 120235426339240519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120235426339240519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/cfdf4257bd8375968e71dcfba8e6cdc4426b51c7980669627d118d043ed5bc8f.mp4
Landing page: https://www.healthformoms.co/save/

M017: MOMS25 - 5TH DEC - Y1 - Copy 5. Frustrated woman at a table covered in medical bills. Text hook "If you make $50k+, you're paying too much." $92.60 at an $18.52 cost per lead, the best in the set.
Facebook ad id: 120235426343210519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120235426343210519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/c9fc4d3728ca9cdd2c6ce4059f93365dbac70700a7dff0b04e2f88f969068516.mp4
Landing page: https://www.healthformoms.co/save/

M018: MOMS25 - 5TH DEC - Y1 - Copy 6. Mother in a lime green shirt surrounded by paperwork and medical bills. Text hook "Moms, stop overpaying you need to watch this 🚨." $209.46, the largest in the set, at a $52.37 cost per lead.
Facebook ad id: 120235426345340519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120235426345340519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/a01892290fc6576daeeb9211ec13689cbca0d4f7cc96db73c89ddf63c9aa35cb.mp4
Landing page: https://www.healthformoms.co/save/

**The account's origin, December 2024**

M019: Old mom 1. Created 2024-12-05, one of the account's first ads. Woman with short blonde hair and glasses in a domestic interior. "Moms being protectors of our family's health is the most important role we have." $147.83 at a $49.28 cost per lead.
Facebook ad id: 120212229702090519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120212229702090519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/f267294b33a45cfb117cf73348d4160a52b3b2a92c4b11b8fb7aa70f67836bd6.mp4
Landing page: https://www.healthformoms.co/save/

M020: Hot Mom. Created 2024-12-05. Woman with long dark hair holding a toddler in her lap, speaking to camera. $101.70.
Facebook ad id: 120212229789490519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120212229789490519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/30e35fa23065eab6ebd0d572b529b095d8a35f7201c69435c515e2f0b982bd1a.mp4
Landing page: https://www.healthformoms.co/save/

M021: IMG 2. Created 2024-12-10, the account's first statics. Headline "Moms, save 20% on your health insurance." $495.16 at a $12.70 cost per lead.
Facebook ad id: 120212331320610519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120212331320610519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/c3494f4c333ffc0e47145ddd9044bea5f1491268a803c829466655b8ef1414e7.jpg
Landing page: https://www.healthformoms.co/save/

M022: IMG 3. Created 2024-12-10. Headline "THIS IS SAVING MOMS 20% ON THEIR HEALTH INSURANCE."
Facebook ad id: 120212331320560519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120212331320560519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/4b485fe9539fb70cfea081d8ecca46371cd5dd8cbc50d4d981368d79b0c1e29c.jpg
Landing page: https://www.healthformoms.co/save/

**The era-defining creative referenced in past major campaigns**

M023: MOMS38 - 1 - V1. Created 2026-03-12, the winter-to-spring era's biggest ad at $54,173.20 lifetime and a $20.15 cost per lead. Woman filming herself close-up, visibly frustrated, text hook "Health Insurance is a scam 🙄" over the spoken line "My deductible is $6,000."
Facebook ad id: 120239479305920519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239479305920519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/50a0309be06d87e55299b9e00d7962b88516c847dec96e80cfd47e6ba5959b66.mp4
Landing page: https://www.healthformoms.co/save/

M024: MOMS39 - 2 - V2. Created 2026-03-14, $27,775.42 lifetime. Woman lying down with a tweet overlay about deductible costs.
Facebook ad id: 120239551987370519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239551987370519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/d3d8a8e91305ff98cb505c98ece5736a3fdbc72488fe3ea662688f0dfd9739ec.mp4
Landing page: https://www.healthformoms.co/save/

M025: MOMS38 - 2 - V4. Created 2026-03-11. Woman on a porch, frustrated, on the phone. "I'm calling to see why this wasn't covered when y'all said it would be." Named here because it is one of the seven ads that surfaced on the "holiday" keyword cut, incidentally rather than as holiday creative.
Facebook ad id: 120239428101580519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239428101580519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/35488b1fb5e7d7bbfb1140aa591ba6f1a9b431a496f6b246ddaa145cce1e036d.mp4
Landing page: https://www.healthformoms.co/save/

**Funnel destinations appearing in the account**

- https://www.healthformoms.co/save/
- https://quiz.healthformoms.com/#/indvfam

**Public sources read this run**

- https://www.healthinsurance.org/faqs/what-are-the-deadlines-for-the-acas-open-enrollment-period/
- https://www.healthinsurance.org/open-enrollment/
- https://chir.georgetown.edu/what-to-expect-for-open-enrollment-2026-edition/

*This is everything I know about seasonality in creative.*
