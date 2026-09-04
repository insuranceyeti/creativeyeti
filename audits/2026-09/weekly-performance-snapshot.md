---
brand: health-for-moms
doc: weekly-performance-snapshot
week: 2026-W36
generated_on: 2026-09-04
refresh_by: 2026-09-11
date_range: 2026-08-29 to 2026-09-04
prior_week_compared: 2026-08-22 to 2026-08-28
prior_week_snapshot_lineage: "none. This is the first weekly snapshot for this brand, the t0 baseline. There is no prior snapshot to carry forward, so the prior week was built by pulling 2026-08-22 to 2026-08-28 directly rather than by reading a baseline forward. Every week-over-week figure below is a live matched pull, not a carried number."
data_sources_read: [live Meta ads manager via Parker MCP search_facebook_ads_sql on account HealthForMoms act 484897827497337 (11 pulls run 2026-09-04), Parker MCP search_facebook_ad_comments_sql (25 comments since 2026-08-22), audits/2026-09/monthly-performance-report.md, sub-context-docs/marketing-calendar-and-campaigns.md, running-notes/brand-rules.md, running-notes/success-definition.md, running-notes/missing-context.md]
knowledge_docs_read: [parker-system/creative-strategy-context/ad-account-analysis.md, parker-system/creative-strategy-context/ad-metrics-glossary.md, parker-system/creative-strategy-context/killer-performance-ads.md, parker-system/creative-strategy-context/andromeda-v2.md]
data_limitations:
  - "No prior weekly snapshot exists. This is the t0 baseline run, so there is no carried-forward trajectory and no prior loop set to inherit. The six-week pattern reads below lean on the monthly report and the marketing calendar instead of on five earlier snapshots."
  - "Lifetime metrics lag the period series in this account's snapshot. moms-53 3 returns $1,955.60 lifetime against $2,097.43 over the trailing fourteen days, and the whole quiz destination returns $138.27 lifetime against $180.33 for the trailing seven. Every figure in this doc is therefore read off period pulls, never lifetime, except where lifetime is named as lifetime."
  - "Reach and frequency are not returned for this account, so the saturation check that ad-account-analysis.md calls central could not be run. Every fatigue read here rests on CPM against CPL, not on frequency."
  - "Placement-level breakdown is not exposed by the Parker MCP ad tool for this account. The demographics block returns age, gender, device and platform only, so there is no Feed versus Reels versus Stories read."
  - "Account-level hook rate and hold rate are not in the period summary. Both are reported spend-weighted across the top 20 ads by spend, which carry 99.0% of this week's spend and 99.5% of the prior week's."
  - "Moms43 - 4 - V3 and MOMS39 - 2 - V2 - Copy return no landing_url field. Both are read as working-destination ads, inferred from their landing rates of 88.1% and 84.4% rather than read directly."
  - "Northbeam is not connected. Every number is Meta-reported on the Meta default attribution window. This is not multi-touch attribution."
  - "Lead quality is invisible to Parker. It sits with the partner insurance agencies, not in Meta. Nothing below clears gate two."
  - "No ad naming convention was ever supplied. Ad, ad set and campaign names are used as inventory handles only, never as evidence of what a creative is or does."
---

# Weekly performance snapshot — Health For Moms — 2026-W36

## Performance snapshot, past 7 days

The account spent **$16,314.41** and bought **637 leads** in the seven days to 2026-09-04, against **$12,222.18** and **512 leads** the week before. That is spend up 33.5% and leads up 24.4%. Blended cost per lead went from **$23.87 to $25.61**, up 7.3%, which lands the headline number in the brand's own "not good" band. CPM held almost perfectly flat at **$23.48** against $23.49. Click-through rate rose from **1.79% to 1.94%**. Spend-weighted across the top 20 ads, hook rate rose from **39.94% to 41.15%** and hold rate slipped from **4.20% to 3.78%**, still nowhere near the 12% to 15% floor ad-account-analysis.md calls healthy. *Verified* from matched period pulls on both windows.

Now strip the broken page out, because the headline is lying. Ads pointed at `go.healthformoms.co/save/` took **$2,574.92** this week, which is 15.8% of the money, and returned **18 leads at a $143.05 cost per lead**. They bought 1,892 link clicks and delivered **130 landing page views**, a **6.9% landing rate**. Everything else in the account converted 7,459 link clicks into 6,373 landing page views, **85.4%**. On the clean segment the week reads **$13,559.16 for 617 leads at a $21.98 cost per lead**, against **$21.74** the week before. That is a **1.1% move**, not a 7.3% one. *Verified* by landing-url filtered pulls on both weeks. So the week was healthy and the read is quiet: the account added 22.3% more clean spend and bought 21.0% more leads at a cost per lead that barely moved. The entire apparent deterioration is one redirect that the monthly report told the team to fix this week. Instead of being fixed, it more than doubled, from $1,136.37 to $2,574.92. *Verified* from matched destination pulls.

## Total ads launched last week

**58 ads were created between 2026-08-29 and 2026-09-04, and 42 of them carried delivery.** That is a big build week by this account's own history, which the marketing calendar puts at a fresh batch every two to four weeks. But the count flatters what actually shipped. Of the 58, **28 are duplicates pointed at `quiz.healthformoms.com`** and **3 are duplicates pointed at the broken `go.` page**, and those 3 took **$2,080.15** of the week's money on their own. The duplicates are not new creative. They are the account's three best working files, moms-63 2b, moms-63 3e and moms-53 3, copied on 2026-08-31 and again on 2026-09-02 and re-aimed at two different destinations. *Verified* from a created-time pull cross-checked against grouped media hashes, which show the same three video files carrying three ad IDs each.

Two things in the batch are genuinely new and both are worth naming. **moms62** is eight files launched 2026-09-03, still the same POV husband savings hook over fresh domestic footage, and it took $155.68 for 9 leads at a **$17.30 cost per lead** on three days of delivery. Too young to call, but it opened in the good band. **moms 68** is the one that matters: **15 files created 2026-08-31**, a satirical skit format with a woman in a black leather jacket playing out a mock insurance sales pitch, under text hooks like *"HEALTHCARE IN 2026 BE LIKE:"* and *"This is why health insurance in America is a scam..."*. It is the largest format change this account has made since the claymation set died in July. It received **$4.23 and 163 impressions all week**. *Verified* from a name-filtered period pull.

## Rising ads

Five ads gained real spend. Four sit on the working destination and one does not.

- **moms-63 3e.** $1,372.61 to **$3,720.72**, up $2,348.11 or 171%. CPL $14.92 to **$17.15**. Hook rate 40.34% to 43.92%, hold rate 2.97% to 2.89%, CPM $18.77 over the fortnight, the cheapest impressions of any big spender. Created 2026-08-14.
- **moms-53 3.** $465.61 to **$1,631.82**, up $1,166.21 or 250%. CPL $10.58 to **$19.43**. CTR 3.17% and cost per link click **$1.04**, both the best in the account. Hook rate 37.69% to 34.65%. Created 2026-08-25.
- **moms-65 1a.** $201.98 to **$1,174.65**, up $972.67 or 482%. CPL $28.85 to **$20.98**, the only riser whose cost per lead improved as it scaled. Hook rate 28.60% to 33.27%. Created 2026-08-27.
- **moms55-1.** $7.75 to **$704.90**. CPL **$22.74**. Hook rate 43.79%, the car-line "insurance math" opener. Created 2026-08-28, so this is its first real week.
- **moms-63 2b - Copy.** Zero to **$1,065.76**, created 2026-08-31 straight onto the broken page. **6 leads at $177.63**, 795 link clicks into 66 landing page views. Rising purely on delivery, not on performance, and it should not be read as a creative result at all.

*Verified* from matched per-ad pulls on both weeks.

The four clean risers converge hard. **Three of them carry the identical POV husband text hook** the account has run since April, word for word apart from the heart emoji, and what differs is the picture: a mother and son walking outdoors, a stylish mom at a modern black front door, a woman in sunglasses in her car doing insurance math out loud. That is exactly the vehicle-and-hook move Andromeda v2 puts one rung below a format change, and it is the same lever the monthly report identified as the account's cheapest win. The account is doing more of the one thing August proved. **moms-53 3 is the exception and the interesting one**, the state-list angle delivered mom to mom, and it is buying the cheapest clicks in the account by a wide margin at $1.04 while its cost per lead nearly doubled as spend tripled. Cheap clicks, dearer leads: the click is being won and something after it is not converting.

One fall is worth naming because it is not a fall. **moms-63 2b dropped 65%, from $2,302.41 to $804.85, while its sibling moms-63 3e rose 171%.** Both live in the Moms63 ad set, both carry the same text hook, and their visual hooks are near twins. Read at ad-set level as ad-account-analysis.md requires when multiple ads run in one ad set, Moms63 went from $3,675.02 at a $15.91 CPL to **$4,525.57 at a $17.27 CPL**. That is Meta rotating budget between two files it very likely groups under one entity ID, not a verdict on either creative. *Inferred* from the shared text hook and near-identical visual hook fields read against the entity-ID grouping rules in andromeda-v2.md, since Meta does not expose entity grouping and frequency is not returned for this account.

## Patterns and data points worth knowing

**The account built format variety and then starved it.** 15 satirical skit files went live on 2026-08-31 and drew $4.23 between them. In the same week, $2,080.15 went to three copies of already-proven ads pointed at a page that eats 93% of its traffic. Whatever the intent, the money went to duplicates of the known and not to the one genuinely different thing in the batch. The monthly report asked for a footage sprint and a real format test before November. Half of that arrived, and the half that arrived cannot be judged on 163 impressions.

**The comment thread turned into an objection wall this week.** 25 comments landed since 2026-08-22. **10 of them, 40.0%, are the single word "Help," and every one sits on Moms43 - 4 - V3**, which is the same unexplained pattern the monthly flagged at 61.0% of August's comments. What is new is the rest. A mom wrote *"Preexisting health condition of cancer disqualified me"* on 2026-09-02, which is the pre-existing-conditions objection the monthly named, now with a named condition attached. Another wrote *"I called them they spammed me and wasted hours of my time to tell me it was going to cost $400/month LOL. SO IT DOESNT SAVE YOU $400 it literally costs just the same if not more than regular scammy health insurance."* on 2026-09-03, directly under the savings claim that carries most of the account's spend. A third, tied for most-liked with 1 like, reads *"I'm sure the mom that can afford matching outfits prob just pays in cash 🤦‍♀️"*, sitting under the well-dressed-mom footage that all three top risers use. And one simply says *"I thought it was a Disney world membership."* Against golden rule four in killer-performance-ads.md, zero confusion, that last one is a straight miss. *Verified* by a full comment pull since 2026-08-22.

**Open Enrollment is 58 days out and nothing seasonal has shipped.** The marketing calendar puts the brand's own stated planning window at two months, which started on or about 2026-09-01. Of the 58 ads created last week, none references enrollment, a deadline, or the January subsidy change, consistent with a lifetime corpus that returns zero ads on "deadline" across 2,122 files. The build is a volume ramp, not a seasonal one. December is the month to plan against, not November: the calendar's thirteen-month series shows November 2025 held cost per lead nearly flat at $13.08 while December broke to $18.28 on the most expensive impressions of any month.

## Open loops

**1. The account made 15 genuinely different files and gave them $4.23.**
The moms 68 batch launched 2026-08-31 with a satirical skit format nothing else in this account looks like, and drew 163 impressions across 15 files in five days. In the same window three duplicates of existing winners took $2,080.15. This is not a one-off. The Moms53 drop of 2026-08-25 put seven files up together and one of them, moms-53 3, took **$1,955.60 of the batch's $1,960.50, or 99.75%**, leaving $4.90 for the other six. The Moms65 drop of 2026-08-27 put eleven files up and moms-65 1a took **$1,283.97 of $1,375.03, or 93.4%**. *Verified* by ad-set-scoped lifetime pulls run 2026-09-04.
*Pull: Surprise.* An account whose own diagnosis is that it has almost no creative diversity built a batch of diversity and then did not spend on it, and the same winner-takes-all split shows up in three separate drops inside three weeks.
**Question: What decides which new files in this account get delivery in their first week?**
If new formats are being starved by budget structure rather than by performance, then every format test this brand runs before November will die without ever being measured, and the fix is a media-buying change rather than a creative one.
*Territory: Messaging.*

**2. A caller says the $400 saving is not real.**
On 2026-09-03 a commenter wrote that she called, spent hours, and was quoted $400 a month, under an ad whose text hook promises saving $400 a month. That hook carries the majority of the account's spend.
*Pull: Tension.* The account's single most-used claim and a public account of what happened on the phone cannot both be a fair description of the offer.
**Question: What do moms actually end up paying after they call the agency?**
If the quoted price commonly lands near what she already pays, the savings claim is buying clicks the funnel cannot close, and that shows up as the cheap-click, dear-lead pattern already visible on moms-53 3. **This one only the brand can answer.**
*Territory: Product.*

**3. The state list is being shown to moms in states that are not on it.**
On 2026-09-02 a commenter asked, under the approved-state-list ad, *"Why is this being shown in IL if it's not on the list???😭🤦🏼‍♀️"*. Two more this window name Georgia and Texas.
*Pull: Pattern.* Three separate commenters in seven days say the ad reached them somewhere it cannot serve them, which is a different problem from the demand-loss question the monthly report already opened.
**Question: How much of this account's spend lands on moms in states the product cannot sell into?**
If the share is meaningful, the cheapest efficiency gain available before Open Enrollment is a geo exclusion, not a creative change.
*Territory: Personas.*

## Appendix - Parker media links

Links and paths preserved exactly as returned by the Parker MCP.

**M001: moms-63 3e.** The week's top spender at $3,720.72 for 217 leads at $17.15, hook rate 43.92%, CPM $19.40. The POV husband line over outdoor mother-and-son footage. Discussed in the snapshot and as riser one. Created 2026-08-14.
Facebook ad id: 120247093478820519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4
Landing page: https://www.healthformoms.co/save/

**M002: Moms43 - 4 - V3.** $3,166.14 for 101 leads at $31.35, hook rate 46.26%, CPM $27.36. Spend down 12% week over week. Carries all 10 "Help" comments. Created 2026-04-15. No landing_url returned; working destination inferred from an 88.1% landing rate.
Facebook ad id: 120241073380060519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

**M003: moms-53 3.** $1,631.82 for 84 leads at $19.43, a 3.17% CTR and a $1.04 cost per link click, both best in the account. The "Approved State List ✔️" opener. Riser two, and the ad carrying the Illinois, Georgia and Texas comments. Created 2026-08-25.
Facebook ad id: 120247254787160519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4
Landing page: https://www.healthformoms.co/save/

**M004: moms-65 1a.** $1,174.65 for 56 leads at $20.98, up 482% in spend with cost per lead improving from $28.85. Stylish mom at a modern black front door. Riser three. Created 2026-08-27.
Facebook ad id: 120247285907980519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247285907980519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/bb071de9e8d0e46ca498a10528b066d07bf324999cb3e1b0d11d83c83592cc67.mp4
Landing page: https://www.healthformoms.co/save/

**M005: moms-63 2b - Copy.** $1,065.76 for 6 leads at $177.63 on the broken destination, created 2026-08-31. 795 link clicks, 66 landing page views, click quality 8.30. The riser that is not a result.
Facebook ad id: 120247339552100519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247339552100519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
Landing page: https://go.healthformoms.co/save/

**M006: moms-63 2b.** $804.85 for 45 leads at $17.89 on the working destination, down 65% in spend as its ad-set sibling M001 rose. The entity-ID rotation discussed in rising ads. Created 2026-08-14.
Facebook ad id: 120247093361410519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
Landing page: https://www.healthformoms.co/save/

**M007: moms55-1.** $704.90 for 31 leads at $22.74, hook rate 43.79%. Woman in orange-tinted sunglasses and a Budweiser tank in her car, doing insurance math in the school pickup line. Riser four, first full week. Created 2026-08-28.
Facebook ad id: 120247304910390519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247304910390519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b3ef51c46ea047450eeba20ec707c5b9022d136aa15f90b609da424269526a11.mp4
Landing page: https://www.healthformoms.co/save/

**M008: moms 68 1#.** $0.85 and 32 impressions all week. The satirical skit format discussed in launches and in open loop 1. Woman in a black leather jacket, text hook "This is why health insurance in America is a scam...". Created 2026-08-31.
Facebook ad id: 120247340952300519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247340952300519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/7aa5cf3b3cd5d470e40e939f3ab051cd97d6c2ae5d4dcac6ca317f9fe5dda470.mp4
Landing page: https://www.healthformoms.co/save/

**M009: moms 68 20# (alt music).** $0.70 and 39 impressions. Second file from the starved batch, text hook "POV: No one's safe in 2026... (health insurance)". Created 2026-08-31.
Facebook ad id: 120247341364200519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247341364200519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/fddda9c526978d089b7d4fffe0f09af7d793d470613196b4ba4c743c665c57b1.mp4
Landing page: https://www.healthformoms.co/save/

**M010: moms62 3.** $46.81 for 2 leads at $23.41 on three days. The 2026-09-03 drop, mother and baby in a dim bedroom, home-video look, same POV savings hook. Created 2026-09-03.
Facebook ad id: 120247381576000519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247381576000519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0253305133ef166bb67b315dedcc72721f9192b3ecc70f83c503c4664a6f7de1.mp4
Landing page: https://www.healthformoms.co/save/

**M011: moms-67 4#.** $107.74 for zero leads, the largest of the 28 ads on the quiz destination. Created 2026-09-03. Treated as unmeasured, not underperforming.
Facebook ad id: 120247380940680519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247380940680519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/50ac45c62c1386238854a24b156f56f119620062459f1314a7fb3611355040ff.mp4
Landing page: https://quiz.healthformoms.com/2

**M012: Moms43 - 5 - V1.** $1,025.37 for 33 leads at $31.07 on a $41.45 CPM, the most expensive impressions of any ad with real spend this week. Named as context on the aging side of the account. Created 2026-06-01.
Facebook ad id: 120243987355020519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120243987355020519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0fe2980848d12fe1c6fd107a759e68fe37d8776c34235b5fab3c15e751af171d.mp4
Landing page: https://www.healthformoms.co/save/

**Funnel destinations appearing in this window**

- https://www.healthformoms.co/save/
- https://go.healthformoms.co/save/
- https://quiz.healthformoms.com/2
- https://quiz.healthformoms.com/#/indvfam

This is everything I know about Andromeda v2.
