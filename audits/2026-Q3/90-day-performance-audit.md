---
brand: health-for-moms
doc: 90-day-performance-audit
quarter: 2026-Q3
generated_on: 2026-09-03
refresh_by: 2026-12-02
date_range: 2026-06-06 to 2026-09-03
prior_window_compared: 2026-03-08 to 2026-06-05
data_sources_read: [Parker MCP search_facebook_ads_sql live pulls against Meta ad account HealthForMoms act 484897827497337, Parker MCP get_brand_persona brand context document, Parker MCP list_custom_metrics, Parker MCP search_chat_history, running-notes/missing-context.md]
prior_quarter_baseline: none. This is the t0 baseline run, no prior 90-day performance audit exists
data_limitations:
  - "Placement-level breakdown is not exposed by the Parker MCP ad tool. The demographics block returns age, gender, device and platform only. Section five is therefore written on the platform split of Facebook, Instagram, Audience Network, Messenger and Threads, and every read of Feed versus Reels versus Stories share is marked data-limited."
  - "Reach and frequency are not returned by the tool for this account, so the frequency check that ad-account-analysis.md calls central to reading audience saturation could not be run."
  - "Account-level hook rate and hold rate are not in the period summary. Both are reported as spend-weighted figures across the top ten spending ads, with the coverage share stated on every use."
  - "No prior 90-day performance audit exists. Every trajectory read in this doc is built by pulling the prior 90-day window directly rather than by carrying a baseline forward."
  - "Northbeam is not connected. All attribution is Meta-reported on the Meta default window. Do not read these numbers as multi-touch."
  - "The Phase 0 brand intake was not run. Naming convention and attribution settings were never supplied by the team, so ad-name parsing in this doc is inventory bookkeeping only and never a creative claim."
  - "Customer reviews and post-purchase surveys are dark surfaces with zero rows, and no competitors are tracked, so no outside-in check on the delivery reads was possible."
---

# 90-day performance and delivery audit — Health For Moms — 2026-Q3

## Executive summary

The single biggest thing that happened to this account in the last 90 days is that it got small. Spend over the 90 days from June 6 to September 3, 2026 was $99,266.98. Over the prior 90 days, from March 8 to June 5, it was $374,507.92. That is a drop of 73.5 percent, from $4,161 a day down to $1,103 a day. Leads fell by exactly the same 73.5 percent, from 16,535 to 4,384. **Verified** across two matched 90-day pulls from the Meta account HealthForMoms, act 484897827497337, on the Meta default attribution window.

Here is the part that matters more than the drop itself. Cost per lead did not move. It was $22.65 in the prior window and $22.64 in this one, a one-cent difference on a $275,000 change in spend. **Verified** from the same two pulls. Against the brand's own stated tiers, where under $15 is fantastic, $15 to $20 is good, $20 to $25 is meh and over $25 is not good, the account has been parked in the "meh" band for six straight months. So the account did not shrink because it broke. It shrank and held its efficiency exactly where it was, which reads as a budget decision rather than a performance failure. **Inferred** from the flat CPL against a collapsing spend base, since a fatigue-driven collapse would have pushed CPL up as it fell. The month-by-month shape backs that up: April peaked at $156,716, then May $105,666, June $42,698, July $18,390 at the trough, and August back to $42,748.63. The rebound in August, with 90 ads carrying delivery against July's 25, looks like a deliberate restart, not a drift.

Where the money went is now dangerously narrow. One ad, "Moms43 - 4 - V3," took $43,002.86 of the $99,266.98, which is 43.3 percent of everything the account spent in 90 days. Widen that to the four ads carrying the same text hook, the "POV: Telling your husband you found better health insurance, saved $400 a month, AND the deductible is zero" line, and you get $60,817.69 of spend, or 60.5 percent. **Verified** by ad-level pull. Read through Andromeda v2, that is not four ads. Four videos that open on a mother and a young child in a warm domestic setting, cut the same way, carrying the same overlay, are exactly the case the entity-ID rules describe as one fingerprint wearing four creative IDs. The account is very likely buying far less incremental reach than its ad count suggests. **Inferred** from the visual-hook descriptions and the shared text hook, not from a Meta entity-ID readout, which Parker cannot see.

On delivery, the auction moved the account younger and very slightly less female. Spend on 25-to-34-year-olds rose 8.6 points to 38.6 percent while 45-to-54 fell 4.7 points to 12.7 percent, and female share slipped from 96.8 percent to 95.2 percent, falling in every single month from March's 97.5 percent to August's 94.8 percent. **Verified** from the age and gender breakdowns on both windows plus six monthly pulls. The baseline metric furthest outside a healthy range is hold rate. Spend-weighted across the top ten ads, which carry 87.3 percent of this window's spend, hold rate is 3.83 percent. In the prior window, weighted across the top ten carrying 63.1 percent of spend, it was 11.09 percent. The glossary's starting-point floor is 12 to 15 percent. Hook rate went the other way, up from 37.28 percent to 43.40 percent. The account got much better at stopping the scroll and much worse at holding anyone once it did. With Open Enrollment on November 1 and a stated two-month planning lead, that combination is the thing to fix before the money goes back on.

## Totals

The headline counts for the 90 days from June 6 to September 3, 2026, pulled from the Meta ad account HealthForMoms, act 484897827497337, on the Meta default attribution window. Prior-window figures for March 8 to June 5, 2026 sit alongside each one.

- **Total spend:** $99,266.98, against $374,507.92 prior. Down 73.5 percent.
- **Ads with delivery:** 147, against 443 prior. Of this window's 147, 117 were created inside the window and 30 are carryover.
- **Total leads:** 4,384, against 16,535 prior. Down 73.5 percent.
- **Cost per lead:** $22.64, against $22.65 prior. Flat.
- **Total impressions:** 4,324,098, against 15,823,676 prior.
- **CPM:** $22.96, against $23.67 prior.
- **CTR:** 1.80 percent, against 2.44 percent prior.
- **Link clicks:** 50,885, against 213,333 prior. Cost per link click $1.95, against $1.76 prior.
- **Landing page views:** 42,108, against 187,037 prior.
- **Purchases and purchase value:** 0 and $0. **ROAS is 0 and always will be here.**
- **Average ROAS across the account:** not applicable. This is a lead-generation account with no purchase event. Reporting a ROAS figure for this brand would be a fabrication, so the honest total is the CPL above.
- **Custom conversions in the window:** 310 events on the pixel custom event across 24 ads, and 42 on the Call event across 15 ads.

Two notes the reader should carry through the rest of the doc. First, the sibling audits and any later report must judge this account on CPL, lead volume, CPM, CTR, hook rate and hold rate, never on ROAS, AOV or purchase value, because the business model is a match-and-consult referral to partner insurance agencies rather than a direct sale. **Stated** in `running-notes/missing-context.md` and confirmed by the zero-purchase pull. Second, the spend-weighted hook rate of 43.40 percent and hold rate of 3.83 percent quoted throughout are computed across the ten highest-spending ads, which together carry $87,726.37 of the window's spend, or 87.3 percent. The tool does not return an account-level figure for either.

## Age group breakdown by spend

Across the 90 days from June 6 to September 3, spend by age bracket ran as follows. The 35-to-44 bracket took $42,327.61, or 42.6 percent. The 25-to-34 bracket took $38,345.57, or 38.6 percent. The 45-to-54 bracket took $12,584.77, or 12.7 percent. The 55-to-64 bracket took $2,978.64, or 3.0 percent. The 18-to-24 bracket took $2,507.04, or 2.5 percent. The 65-and-over bracket took $515.15, or 0.5 percent. **Verified** from the age breakdown on the 90-day pull. In the prior window those same brackets ran 46.5 percent, 30.0 percent, 17.4 percent, 3.9 percent, 1.5 percent and 0.7 percent.

The account is concentrated to an unusual degree in a twenty-year band. Combined, 25-to-44 now takes 81.2 percent of all spend, up from 76.5 percent in the prior window. Everything from 45 upward now shares 16.2 percent, down from 22.0 percent. The direction of travel is clean and it is monotonic through the middle of the quarter, not a one-month wobble. Reading the monthly pulls in order, the 45-to-54 share went 13.6 percent in March, 19.3 percent in April, 17.8 percent in May, 13.2 percent in June, 11.1 percent in July, then back to 14.4 percent in August. The 25-to-34 share went 33.3, 27.4, 31.1, 38.7, 41.6, then 35.5. **Verified** across six monthly pulls. So the drift toward younger moms ran hardest from April through July and then partly reversed in August.

That August reversal is the interpretive key, and it lines up with a creative event rather than a targeting change. August is the month the account went from 25 ads with delivery to 90, and 117 of this window's 147 ads were created inside the window. **Verified** by a created-time filtered pull. When the account was starved of fresh creative through June and July, the auction pushed budget into the narrowest, cheapest-to-convert pocket it could find, which was moms in their late twenties and early thirties. When new creative arrived in August, the delivery spread back out toward the forties. That is the breakdown effect doing its job, not a targeting error: Meta was pacing a shrinking budget toward the segment where it predicted costs would stay lowest, and the reallocation followed the creative supply. **Inferred** from the alignment of the ad-count rebuild with the age reversion, across six monthly windows.

Held against who the brand says it is for, the concentration is defensible but incomplete. Of the five named ICPs in the brand context document, Marissa is 33, Courtney is 36 and Danielle is 38, all sitting squarely inside the 81.2 percent the account is buying. Nicole is 41, on the edge of it. But the brand also told us the audiences it wants to test are "all different ages of moms with ages of kids," which explicitly includes younger moms with babies and older second-chapter moms. **Stated** in Section 10 of the brand context document. Right now 18-to-24 gets 2.5 percent and 55-plus gets 3.5 percent combined, so two of the brand's own stated test audiences are receiving almost no money at all. Note also that the account's own top spender skews younger than the account average: "Moms43 - 4 - V3" puts 43.9 percent of its budget on 25-to-34 and only 9.7 percent on 45-to-54. The single ad carrying 43.3 percent of the account is itself pulling the whole age curve down.

## Gender breakdown by spend

Over the 90 days from June 6 to September 3, female-attributed spend was $94,543.40, or 95.2 percent. Male-attributed spend was $4,161.85, or 4.2 percent. Spend against unknown gender was $556.02, or 0.6 percent. **Verified** from the gender breakdown on the 90-day pull. In the prior window the same split was 96.8 percent female, 2.5 percent male and 0.6 percent unknown. So female share fell 1.6 points and male share rose 1.7 points.

On its face this is a rounding error, and any single month's move would be. What makes it worth naming is that it never once goes the other way. Female share reads 97.5 percent in March, 97.0 in April, 96.1 in May, 95.7 in June, 95.2 in July and 94.8 in August. Male share reads 1.9, 2.4, 3.3, 3.7, 4.3 and 4.6 across the same months. **Verified** across six monthly pulls. Six consecutive months of movement in one direction is a trend, not noise. Male spend has roughly two and a half times its March share.

The split is close to intentional and the brand should not read the drift as a leak yet. Health For Moms is built around mothers, its ICPs are all women, and 95.2 percent female delivery on broad targeting means the creative is doing its qualifying job well before the auction has to. Per the hook-psychology frame, the opening lines are doing the "qualify" work loudly: a hook that says "POV: Telling your husband you found better health insurance" names its audience in its first four words, and the "if you're a mom and your deductible is insane" hook on ad `120247145872230519` does it even more directly. That is why male share is 4 percent and not 20. **Inferred** from the text and verbal hooks on the top-spending ads read against the delivery split.

What the trend probably reflects is the household, not a new buyer. Health insurance is a family purchase, and the creative itself keeps putting a husband in the frame, as the top ad's hook does. Dads shopping the same family plan are a plausible source of the extra two points. But that is a guess Parker cannot settle from delivery data alone, because there is no gender cut on leads available in this tool and no survey or review corpus to check it against. The honest position is that the gender picture is stable and intentional, the movement is real but small, and the question of who those men are is left open below rather than answered here. **Data-limited**: lead-level gender attribution is not exposed, and both the review and post-purchase-survey surfaces are dark.

## Placement breakdown

This section cannot be written to the standard the audit asks for, and the reason needs stating plainly rather than buried. The Parker MCP ad tool returns a demographics block containing exactly four dimensions for this account: age, gender, device and platform. There is no placement dimension. Parker checked this twice, once on the account summary and once on a per-ad breakdown for the top spender, and no Facebook Stories, Instagram Stories, Facebook Reels, Instagram Reels, Facebook Feed, Instagram Feed, Audience Network or Messenger split was returned in either. **Verified** by two pulls. So the share per placement that this section is supposed to enumerate is unavailable, and every placement claim below is marked data-limited.

What is available is the platform split, which is the nearest honest proxy. Over the 90 days from June 6 to September 3, Facebook took $59,847.83, or 60.3 percent. Instagram took $38,814.78, or 39.1 percent. Audience Network took $506.18, or 0.5 percent. Threads took $95.42, or 0.1 percent. Messenger took eight cents. **Verified** from the platform breakdown. In the prior window: Facebook 60.3 percent, Instagram 39.3 percent, Audience Network 0.2 percent, Threads 0.2 percent. The headline read is that the Facebook and Instagram balance is remarkably stable, identical to a tenth of a point on Facebook across two 90-day windows. Device is even more lopsided and equally stable: mobile took 99.5 percent of spend in both windows, desktop 0.5 percent.

Two things inside that stability are worth interpreting. First, the monthly platform reads are noisier than the 90-day totals let on. Facebook ran 62.2 percent in March, 60.5 in April, 57.8 in May, 63.3 in June, 57.8 in July and 58.2 in August. **Verified** across six monthly pulls. The June spike to 63.3 percent is the month the account was most starved of new creative and leaning hardest on the carryover POV ads, and the two months either side of it, at 57.8 percent, are the months with more creative variety in market. Read through the placement-signal logic in `ad-account-analysis.md`, heavier Facebook delivery points at an older, more deliberate, lean-back audience, and that is consistent with the account's older skew being strongest at the edges of the window. Second, Audience Network more than doubled its share, from 0.2 percent to 0.5 percent. That is $506 and it does not matter on its own, but Audience Network is off-platform inventory with the shallowest attention of anything the account buys, and a rising share of it while total spend is falling is usually a sign the system is reaching for cheaper impressions.

The fit question the audit is meant to answer cannot be closed. The account is 99.5 percent mobile and its creative is video built for a vertical mobile feed, so at the platform level there is no mismatch to name. But whether that vertical creative is landing in Reels, where a habitual short-form viewer is primed for it, or in Feed, where the same 9:16 asset reads as a poorly fitted post, is precisely the question the missing placement cut would answer, and it is the question that decides whether the hold-rate collapse in the next section is a creative problem or a placement problem. **Data-limited.** Getting placement-level reporting exposed for this account is the highest-value reporting fix available before Open Enrollment, and it is logged in the frontmatter as an infrastructure gap rather than as an open loop.

## Baseline account metrics, last 90 days

The core numbers for the 90 days from June 6 to September 3, with the prior 90-day window alongside. Cost per lead is $22.64, against $22.65, effectively flat. CPM is $22.96, against $23.67, down 3.0 percent. CTR is 1.80 percent, against 2.44 percent, down 0.64 points. Cost per link click is $1.95, against $1.76, up 10.8 percent. Spend-weighted hook rate across the top ten ads, which carry 87.3 percent of this window's spend, is 43.40 percent, against 37.28 percent weighted across the prior window's top ten, which carried 63.1 percent of that spend. Spend-weighted hold rate on the same basis is 3.83 percent, against 11.09 percent. **Verified** from ad-level pulls in both windows, with the weighting computed on spend. Frequency and reach are not returned by the tool, so the saturation check is **data-limited**.

The account is healthy on cost and unhealthy on attention. CPM at $22.96 is cheap for a regulated insurance category and it improved while spend fell, which tells you the account is not being punished in the auction. CPL held its exact position through a 73.5 percent contraction, which is genuinely hard to do and says the core state-angle offer still converts. But against the brand's own tiers, holding steady means holding steady in the "meh" band of $20 to $25 for the whole quarter, and the brand's stated goal is "SCALE BABY!" You cannot scale from a meh CPL by adding budget alone, because the thing that usually gives first is exactly the metric that has already given: attention depth.

Hold rate is the number to act on. At 3.83 percent it sits far below the 12 to 15 percent starting-point floor, and it did not get there gradually. It got there because the account's center of gravity moved from one kind of ad to another. The prior window's top spender, "MOMS38 - 1 - V1," was a woman filming herself close-up, visibly frustrated, opening on the spoken line "My deductible is $6,000" under the text hook "Health Insurance is a scam." It ran a 32.76 percent hook rate, a 17.29 percent hold rate and a 7.08-second average play time on $54,173.20. This window's top spender, "Moms43 - 4 - V3," opens on a mother and baby lying in bed on white bedding, looking peacefully into the camera, with no spoken words at all, only music, under the POV overlay about telling your husband about the savings. It runs a 45.35 percent hook rate, a 3.28 percent hold rate and a 4.04-second average play time on $43,002.86. **Verified** from both ads' full media fields and period metrics. The account traded a talking-head problem-solution opener that kept people for seven seconds for a silent lifestyle montage that stops thumbs brilliantly and then has nothing to say.

That trade explains the CTR decline too, and it is the same story in a different metric. CTR fell from 2.44 percent to 1.80 percent while hook rate rose six points. More people are stopping and fewer are clicking, which is what happens when the opener promises something the next few seconds do not pay off. Per the killer-performance-ads standard, seconds one through three owe the viewer a reason to keep watching and seconds three through five owe them the best benefit or a re-hook, and a music-only montage delivers neither. The evidence that this is fixable rather than structural sits inside this very window: "Moms43 - 5 - V1," a UGC selfie video with a screenshot overlay of someone complaining about high deductibles, opening on the spoken line "This is why you can't simply just say 'Oh, I have insurance, I'm covered,'" runs a 7.59 percent hold rate and a 2.14 percent CTR on $10,125.67. Same window, same account, roughly double the hold of the top spender. **Verified** from its ad record.

Two more reads to carry into next quarter. First, the newer creative is cheaper. The 117 ads created inside this window spent $26,403.17, which is 26.6 percent of the total, and returned 1,303 leads at a $20.26 CPL. The 30 carryover ads spent $72,863.81, or 73.4 percent, and returned 3,081 leads at a $23.65 CPL. **Verified** by a created-time filtered pull. The account is putting nearly three quarters of its money behind its more expensive cohort, and the newer work is landing in the brand's "good" band while the old work sits in "meh." That is a very different posture from the prior window, when 401 net-new ads carried 90.7 percent of spend at a $22.82 CPL. The account has gone from a fast-cycling creative machine to one leaning on a handful of survivors. Second, per Andromeda v2, that concentration is a delivery risk and not only a creative one. When 60.5 percent of spend sits on four ads sharing a text hook and a near-identical opening frame of a mother with a young child in a home, the system is very likely treating them as one entity rather than four, which caps incremental reach and pushes frequency up on the same pool of moms. Parker cannot confirm that from the account, because entity-ID grouping is not something Meta exposes and frequency is not returned here, so this stays **inferred** from the visual-hook and text-hook evidence rather than verified.

Heading into Open Enrollment on November 1, with the brand's own two-month planning lead meaning the ramp should already be underway, the watch list is short. Hold rate is the metric to move, the talking-head problem-solution opener is the proven lever for moving it, and the account needs genuinely different opening frames rather than more variants of the mother-and-child montage before the budget goes back on.

## Open loops

**1. The auction keeps moving money to younger moms.**
Spend on 25-to-34-year-olds climbed 8.6 points to 38.6 percent of the account while 45-to-54 gave up 4.7 points to land at 12.7 percent, and the account's single biggest ad puts 43.9 percent of its own budget on 25-to-34 against just 9.7 percent on 45-to-54. The brand meanwhile says it wants to test moms of all ages with kids of all ages.
*Pull: Tension.* The delivery data and the brand's stated audience ambition point in opposite directions, and both cannot be the right description of who this account is for.
**Question: What is making Meta concentrate this account's spend on moms aged 25 to 34?**
If the answer is that the creative only speaks to that age, the fix is casting and setting. If the answer is that younger moms simply convert cheaper here, the age spread the brand wants to test may cost more per lead and the team should know that before Open Enrollment.
*Territory: Personas.*

**2. Spend fell by three quarters and nobody has said why.**
Monthly spend went from $156,716 in April to $18,390 in July and back to $42,749 in August, a 73.5 percent fall across the quarter, while cost per lead did not move at all, sitting at $22.65 then $22.64.
*Pull: Surprise.* A collapse this size normally shows up as rising costs somewhere, and here it left no mark on efficiency whatsoever, which is not what a performance problem looks like.
**Question: What drove the drop in monthly spend from April through July?**
Whether this was a budget decision, a partner-capacity limit on how many leads the agencies could take, or something else entirely changes what "scale" means for the November push. **This one only the brand can answer.**
*Territory: Product.*

**3. The account stopped holding attention.**
Spend-weighted hold rate across the top ten ads fell from 11.09 percent to 3.83 percent while hook rate rose from 37.28 percent to 43.40 percent, and average play time on the biggest ad is 4.04 seconds against 7.08 seconds on last window's biggest ad.
*Pull: Surprise.* Hook and hold almost always move together, and watching them split this far apart in one quarter contradicts what the account's own history predicted.
**Question: What are moms hearing in the first five seconds of the ads that still hold them?**
Hold rate is the clearest lever on CPL the account has, and knowing what the surviving high-hold ads actually do in seconds one through five would tell the team what to brief before November.
*Territory: Messaging.*

**4. The cheaper creative is getting the smaller budget.**
The 117 ads launched inside this window brought leads at $20.26 on 26.6 percent of spend, while the 30 older carryover ads brought them at $23.65 on 73.4 percent of spend.
*Pull: Gap.* There is a cheaper cohort sitting right there in the account and almost three quarters of the money is going somewhere else.
**Question: How much of the account's budget could move to newly launched creative before its cost per lead starts rising?**
Every dollar shifted at the current gap is worth about $3.39 per lead, and knowing where that advantage breaks down sets the ramp plan for Open Enrollment.
*Territory: Messaging.*

**5. Men keep showing up, month after month.**
Male-attributed spend rose in every single month of the last six, from 1.9 percent in March to 4.6 percent in August, while female share fell from 97.5 percent to 94.8 percent across the same run.
*Pull: Pattern.* One month would be noise, but six consecutive months moving the same way across independent monthly pulls is something accumulating.
**Question: Who are the men this account is reaching, and what do they do after they see the ad?**
Health insurance is bought for a household, and if dads are quietly becoming a real slice of the funnel, that is either a second buyer worth speaking to or wasted delivery worth excluding.
*Territory: Personas.*

**6. The same mom is in almost every frame.**
The four ads carrying 60.5 percent of the window's spend all open on a mother with a young child in a warm home setting, and the one that broke the pattern, a woman filming herself and talking straight to camera about a $6,000 deductible, was the account's biggest ad last quarter with more than five times the hold rate.
*Pull: Gap.* The account has almost no one else on screen, and the one time it cast differently it produced its best-holding ad.
**Question: Who else could carry the state angle on camera besides a mom at home with her toddler?**
The brand names casting as its top creative bottleneck, so knowing which other people can carry this message decides what it briefs creators to shoot before the November window.
*Territory: Creators and talent.*

**7. Parker has never seen this account through an Open Enrollment.**
The brand names November 1 as the single most important date on its calendar and plans seasonal creative two months ahead, but the account data available here begins in early 2026 and contains no prior Open Enrollment window.
*Pull: Curiosity.* The biggest moment of this brand's year is one the account history cannot yet explain anything about.
**Question: What happens to this brand's cost per lead and lead volume during an Open Enrollment window?**
Whether CPL improves on rising intent or worsens on rising competition decides how much budget and how much creative the team needs standing by on November 1.
*Territory: Product.*

## Appendix - Parker media links

Every ad discussed in the body of this audit, indexed so a strategist can reopen the media without searching. Links and paths are preserved exactly as returned by the Parker MCP.

**M001: Moms43 - 4 - V3.** The account's top spender this window at $43,002.86, 43.3 percent of all spend. Discussed in the executive summary, the age breakdown and the baseline metrics section as the low-hold silent montage.
Facebook ad id: 120241073380060519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

**M002: MOMS38 - 1 - V1.** The prior window's top spender at $54,173.20, with a 17.29 percent hold rate and 7.08-second average play time. Discussed in the baseline metrics section as the talking-head opener the account moved away from.
Facebook ad id: 120239479305920519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239479305920519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/50a0309be06d87e55299b9e00d7962b88516c847dec96e80cfd47e6ba5959b66.mp4
Landing page: https://www.healthformoms.co/save/

**M003: Moms43 - 5 - V1.** $10,125.67 this window at a 7.59 percent hold rate and 2.14 percent CTR. Discussed in the baseline metrics section as the in-window counter-example that holds attention.
Facebook ad id: 120243987355020519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120243987355020519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0fe2980848d12fe1c6fd107a759e68fe37d8776c34235b5fab3c15e751af171d.mp4
Landing page: https://www.healthformoms.co/save/

**M004: Moms43 - 4 - V1.** $6,993.31 this window. Part of the POV text-hook cluster discussed in the executive summary and the baseline metrics section.
Facebook ad id: 120241073380110519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380110519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/f18c5a15a13e4412e35f654034f63f147ca73e40b35538419d22500d143b670d.mp4

**M005: Moms43 - 4 - V4.** $6,360.53 this window, and $18,518.27 in the prior window. Same ad set as M001 and M004.
Facebook ad id: 120241073380050519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380050519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/985c6a8045a5bcfb5e7450ad0f3a00ca783b996f4ba3633337e8c84e1aac8a39.mp4

**M006: moms-63 2b.** $5,529.30 this window at a $13.26 CPL, the cheapest lead cost among the top spenders and inside the brand's "fantastic" band. Created August 14, part of the August rebuild.
Facebook ad id: 120247093361410519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
Landing page: https://www.healthformoms.co/save/

**M007: moms-63 3e.** $5,243.54 this window at a $15.47 CPL. Part of the POV text-hook cluster.
Facebook ad id: 120247093478820519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4
Landing page: https://www.healthformoms.co/save/

**M008: MOMS34 - N1 - 3a.** $5,359.15 this window and $19,434.68 prior. A 46.27 percent hook rate against a 2.36 percent hold rate, the clearest single illustration of the hook-versus-hold split.
Facebook ad id: 120238654140050519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238654140050519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1c501ac53c00f4e6b9f3ee87626968c02aa9861c6958bcf6c338644cbaf1fa8d.mp4
Landing page: https://www.healthformoms.co/save/

**M009: moms-53 3.** $1,956.50 this window at a 3.14 percent CTR, the highest CTR among the top ten spenders. The "Approved State List" opener, closest in the current window to the brand's stated best-performing state angle.
Facebook ad id: 120247254787160519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4
Landing page: https://www.healthformoms.co/save/

**M010: Moms Nahuel WV#1 - V9 - Copy.** $1,639.35 this window at a $273.23 CPL, by far the worst lead cost in the top ten and a click-quality score of 9.13 against an account norm above 85. Referenced in the gender section for its directly qualifying verbal hook.
Facebook ad id: 120247145872230519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872230519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/645496c411d82a546a3e2deada69459c716615ad09f635ca0b978625c2778b37.mp4
Landing page: https://go.healthformoms.co/save/

**M011: moms54-2.** $1,467.48 this window. The $6,000-deductible tweet-overlay opener.
Facebook ad id: 120247063459400519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063459400519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/3a3e8a8b9f24c4b0e70dd7e422561de2773ffc4fd2dfdabd358971ca6be65f98.mp4
Landing page: https://www.healthformoms.co/save/

**M012: Moms36 - 3 - A - 2 - V4c.** $8,604.20 in the prior window at a 15.16 percent hold rate and a 9.82-second average play time, the longest watch time seen in either window. Prior-window reference for what high hold looks like in this account.
Facebook ad id: 120242277732810519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120242277732810519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/fe4ef9c25b9bd439ba7664d9b004e6a952789df99e759dd325e2a638e364cf42.mp4
Landing page: https://www.healthformoms.co/save/

---

This is everything I know about Andromeda v2.
