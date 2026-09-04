---
brand: health-for-moms
doc: ad-account-evaluation
generated_on: 2026-09-04
refresh_by: 2026-12-03
quarter: 2026-Q3
data_sources_read:
  - "Live ads manager via Parker MCP `search_facebook_ads_sql`, Meta account HealthForMoms act 484897827497337, six pulls run 2026-09-04: trailing 90 days grouped by name, trailing 7 days grouped by name, lifetime filtered to static, lifetime filtered to video, an adIds lookup on the four `Moms Nahuel WV#1 - V9 - Copy` variants, and an engagement-metric cut on the top three spenders"
  - "Parker MCP `list_custom_metrics`, run 2026-09-04, four auto-detected pixel events and zero formulas"
  - "Parker MCP `search_tiktok_videos`, run 2026-09-04, to confirm the mining library is unaffiliated creators rather than brand organic"
  - "Facebook ad comments corpus as read by the upstream audits, 92 comments in the 90-day window and 1,322 lifetime"
  - "Brand context document via `get_brand_persona`, as read by the upstream audits"
audit_sources_read:
  - "audits/2026-Q3/90-day-creative-strategy-audit.md, generated 2026-09-03, the anchor"
  - "audits/2026-Q3/90-day-performance-audit.md, generated 2026-09-03, carrying a build-orchestrator correction dated 2026-09-04"
  - "audits/2026-Q3/90-day-diversity-audit.md, generated 2026-09-03"
  - "audits/2026-Q3/quarterly-whitespace-analysis.md, generated 2026-09-04"
  - "audits/2026-09/monthly-hook-audit.md, generated 2026-09-03"
  - "audits/2026-09/monthly-performance-report.md, generated 2026-09-03, reading August 2026"
  - "audits/2026-09/weekly-performance-snapshot.md, generated 2026-09-04, reading week 2026-W36"
  - "audits/2026-09/monthly-organic-tiktok-audit.md, generated 2026-09-04, read for the category-versus-brand boundary only"
  - "sub-context-docs/marketing-calendar-and-campaigns.md, generated 2026-09-04, carrying the canonical quiz-destination correction"
  - "No biweekly iterations report exists yet. That layer of the audit stack is missing."
knowledge_docs_read:
  - parker-system/creative-strategy-context/expertise-routing.md
  - parker-system/creative-strategy-context/ad-account-analysis.md
  - parker-system/creative-strategy-context/analyzing-public-ad-accounts.md
  - parker-system/creative-strategy-context/ad-metrics-glossary.md
  - parker-system/creative-strategy-context/killer-performance-ads.md
  - parker-system/creative-strategy-context/andromeda-v2.md
  - parker-system/creative-strategy-context/ad-formats/
account_stage_summary: "A twenty-one-month-old lead-generation account that has spent $743,218 lifetime for 39,569 leads. It scaled hard in spring 2026, then cut spend 73.5% while holding cost per lead flat, and is now rebuilding volume off a small set of survivors. It runs one creative idea in one format container, it has not run a static ad in over 90 days despite statics being the cheaper half of its own history, and it stops the scroll well while holding almost nobody."
data_limitations:
  - "Reach and frequency are not returned by the Parker MCP ad tool for this account, so the saturation check that `ad-account-analysis.md` calls central cannot be run. Every fatigue read here rests on CPM movement against CPL, never on frequency."
  - "Placement is not exposed. The demographics block returns age, gender, device and platform only, so there is no Feed versus Reels versus Stories read anywhere in this doc."
  - "Account-level hook rate and hold rate are not in the period summary. Both are reported spend-weighted across the top spenders, with the coverage share stated on every use."
  - "Lead quality is invisible to Parker. It sits with the partner insurance agencies. Nothing in this doc clears gate two of the brand's own winner definition."
  - "Northbeam is not connected. Every figure is Meta-reported on the Meta default attribution window. This is not multi-touch attribution."
  - "AI format and emotion tags cover 79 to 80 of the ads with delivery in the 90-day window, which is roughly 54% by count but 93.4% to 94.2% by spend. Count shares and spend shares therefore carry different denominators, and both are stated wherever they are used."
  - "No competitor, inspo or affinity library is tracked. A live `search_competitor_facebook_ads` call returned zero brands. Nothing here is benchmarked against the category."
  - "No customer review corpus and no post-purchase survey. Every customer verbatim in this doc comes from the brand's own Facebook ad comments and is labeled that way, never as a review corpus."
  - "No biweekly iterations report exists, so the audit stack is missing its iteration layer and this doc reconstructs iteration behavior from creation dates and creative fields instead."
  - "The account's month-by-month series does not exist before 2025-09-01, so roughly $104,000 of lifetime spend cannot be placed in a month."
  - "No ad naming convention was ever supplied. Ad, ad set and campaign names are used as inventory handles only, never as evidence of what a creative is or does."
---

# Ad account evaluation - Health For Moms

## Diagnosis

**This account has stopped making ads and started making click-buying devices, and it turned off the cheaper half of itself to do it.** That is the read the whole audit stack lands on, and the live pull on 2026-09-04 still supports it.

Three facts sit under that sentence. First, the trailing quarter is one idea. Over the 90 days to 2026-09-03 the account spent $100,065.31 for 4,421 leads at a $22.63 cost per lead, and ads tagged `POV` touched roughly 70% of it. **Verified**, live pull 2026-09-04. Second, that idea does its selling in the first two seconds of on-screen text and then has nothing left. Spend-weighted hold rate across the top ten ads, which carry 87.3% of the window's spend, is 3.83% against the 12% to 15% floor in `ad-metrics-glossary.md`, while hook rate runs 43.40%. **Verified** from the 90-day performance audit and reconfirmed on the live top-spender pull, where the workhorse holds 3.28% on a 45.36% hook rate. The account stops the scroll beautifully and holds almost nobody. Third, and this is the part the 90-day audits could not see, the account's cheaper half is dark. A lifetime pull filtered to image creative returns **308 ad-name groups, $168,907.73 of spend, 13,735 leads and a $12.30 cost per lead**, against video's $574,310.36 and 25,834 leads at $22.23. **Verified**, my own pull 2026-09-04. Statics took 22.7% of the money, delivered 34.7% of the leads, and cost 44.7% less per lead. Zero of them ran in the last 90 days.

Put those together and the flat cost per lead stops looking like stability. It was $22.65 in the prior quarter and $22.63 now, a two-cent move across a 73.5% spend collapse, a format inversion, an emotion swap and a funnel-posture flip. **Verified** across two matched pulls. A number that will not move through that much upheaval is not measuring the creative. It is measuring the offer. Confidence **strong**.

The one thing that has genuinely moved is the picture. August proved it cleanly: the identical POV husband text hook, word for word, bought a $23.37 lead on April's bedroom footage and a $13.24 lead on August's outdoor footage in the same month. **Verified** from the monthly performance report and from both ads' visual hook fields. Read through the differentiation hierarchy in `andromeda-v2.md`, that is a vehicle-and-hook change one rung below a format change, and it is the only lever this account has pulled in six months that produced a step change in cost.

So the working read a strategist should carry: **the line is not the liability, the sameness of the picture is, and the modality shutdown is bigger than either.** Confidence **strong** on the modality finding, **strong** on the attention finding, **mixed** on whether hold rate matters at all for a form fill, which is an open loop below rather than a settled call.

## Audit provenance

Eight audit artifacts and one sibling context doc feed this page. All were produced in the 2026-09-03 to 2026-09-04 cold-start build, so this is a t0 baseline with no prior read to check against. Every one is model-generated from Parker MCP pulls. **No human strategist has interpreted any of them**, and that matters for how much weight to put on the diagnosis.

| Audit | Date | Window read | Source surface | What it contributes here |
|---|---|---|---|---|
| 90-day creative strategy audit, the anchor | 2026-09-03 | 2026-06-05 to 2026-09-02 | Live Meta pull, 136 ads, full media analysis on the top 10, 92 ad comments, brand context | The diagnosis, the top-ten deep dives, format, emotion, desire and awareness distributions |
| 90-day performance audit | 2026-09-03 | 2026-06-06 to 2026-09-03 against 2026-03-08 to 2026-06-05 | Two matched live pulls plus six monthly cuts | The spend collapse at flat CPL, the age and gender drift, the hold-rate collapse |
| 90-day diversity audit | 2026-09-03 | Same, matched prior window | AI format tags on 80 of 147 delivering ads | The format concentration, the six formats that vanished, the test slate |
| Quarterly whitespace analysis | 2026-09-04 | Lifetime, 1,557 ad-name groups | Lifetime pulls, 1,322-comment corpus | The statics correction, the per-persona lifetime spend map, the employer-plan finding |
| Monthly hook audit | 2026-09-03 | 2026-08-04 to 2026-09-02, video only | Top 20 video ads carrying 99.2% of video spend, nine full transcripts | The opener inventory, the intensity-versus-cost split, the weak-hook verdict |
| Monthly performance report | 2026-09-03 | August 2026 against July 2026 | Top 20 by spend carrying 99.36% of the month, four segment pulls, 59 comments | The footage-versus-copy proof, the destination break, the six reconstructed tests |
| Weekly performance snapshot | 2026-09-04 | 2026-08-29 to 2026-09-04 | Eleven live pulls, 25 comments | The starved format batch, the duplicate build week, the current risers |
| Monthly organic TikTok audit | 2026-09-04 | Fixed 23-video scrape | Parker TikTok mining library | Read only for the boundary: this is category feed, not brand organic |
| `marketing-calendar-and-campaigns.md` | 2026-09-04 | 21 months of creation history, 13 readable months | 22 live pulls plus web search | The Open Enrollment correction and the canonical quiz-destination correction |

Two corrections in that stack are canonical and are honoured throughout this doc.

**The Open Enrollment correction.** The 90-day performance audit states the account's history begins in early 2026 and contains no prior Open Enrollment. Both halves are wrong. Ads were created from **2024-12-05**, and month-by-month metrics are readable from **2025-09-01**, which covers the full 2025-11-01 window. **Verified** by the calendar doc's direct pulls. That audit's open loop 7 is answered, not open, and it does not reappear below.

**The quiz-destination correction.** The figures "903 link clicks against 234 landing page views" and a "$75.72 cost per lead" are **not the quiz**. They are two destinations summed. I re-ran the split myself on 2026-09-04 at ad level and it holds exactly. `go.healthformoms.co/save/` took $1,639.35 for 690 link clicks and **63 landing page views**, a 9.1% landing rate, 6 leads and a **$273.23 cost per lead**, with a click quality score of 9.13. The same creative file on `www.healthformoms.co/save/` took $404.23 for 213 clicks and 171 landing page views, an 80.3% landing rate, 21 leads and a **$19.25 cost per lead**, click quality 80.28. The parent ad on `www.` is healthy at $17,723.91 lifetime, 86.1% landing rate and a $27.91 cost per lead. **Verified**, adIds lookup 2026-09-04.

Worth naming plainly, because it will bite the next reader too: a `groupBy: name` pull returns that whole family as one row showing 903 clicks, 234 landing page views, a $75.75 cost per lead and a `landing_url` of `quiz.healthformoms.com`. The tool renders the newest variant's URL on a row whose metrics sum four variants across three destinations. That is exactly how the original error was made. **Verified** by running both the grouped and the ad-level pull side by side on the same day. **`quiz.healthformoms.com` is a brand-new test at $138.27 lifetime across 26 ads, all created 2026-09-02 or 09-03, and must be treated as unmeasured, never as a leak.**

## Account history and current state

**The shape of the whole thing.** Lifetime, the account has spent **$743,218.09** for **39,569 leads** at a blended **$18.78** cost per lead, across 1,565 ad-name groups, with **zero purchases by design**. **Verified**, two lifetime pulls 2026-09-04. It runs on two standing campaigns rather than named seasonal pushes: a wide test campaign with more than a thousand ads and a tight scale campaign with about forty. It is an always-on acquisition machine. There is no retargeting story, no repeat buyer and no purchase event, so every dollar in it is acquisition.

**The arc, in four moves.** The account was born in December 2024. It ramped for Open Enrollment 2025 and the ramp was real: spend went $17,416 in September to $21,664 in October to $34,236 in November, with 38, 63 and 54 ads created across those months. November made the auction 31.6% more expensive on CPM and the buyer 41.3% more willing on CTR, so cost per lead moved only 6.6%, from $12.27 to $13.08, and November was 2025's biggest lead month. **Verified** from thirteen consecutive monthly pulls in the calendar doc. Then December turned: CPM hit $29.34, the most expensive month of the thirteen, and cost per lead rose 39.8% to $18.28 as the share of landing page views converting to leads fell from 17.1% to 14.2%.

The second move is the spring surge. March, April and May 2026 took $376,489, which is 58.9% of everything the readable series holds, and April alone at $156,716 was 4.6 times November. The account quadrupled February's spend in March and got *cheaper* leads while doing it, $23.39 down to $20.85. **Verified.** Nothing in the account or the chat history records why.

The third move is the collapse. Spend fell 73.5% quarter over quarter, from $374,507.92 to $99,266.98 as the performance audit measured it, and leads fell by exactly the same 73.5%, while cost per lead moved one cent. **Verified** across two matched pulls. Monthly, that reads $156,716 in April, $105,666 in May, $42,698 in June, $18,390 at the July trough, $42,749 in August. A fatigue-driven collapse pushes cost up as it falls. This one did not. It reads as a budget decision, not a performance failure. **Inferred**, confidence **strong** on the reasoning, and the reason itself is only knowable inside the business.

The fourth move is the rebuild, and it is where the account sits today. August went from 25 ads with delivery to 90. **125 ads were created between 2026-08-01 and 2026-09-04**, against 63 in October 2025, so the production machine is running hotter now than it was in the last Open Enrollment run-up. **Verified** from created-time pulls. The 117 ads created inside the 90-day window spent 26.6% of the money and returned leads at $20.26, while the 30 carryover ads spent 73.4% and returned them at $23.65.

**Where it stands right now.** The trailing seven days to 2026-09-03 ran **$17,696.22 for 692 leads at a $25.57 cost per lead**, on a $23.45 CPM and a 1.94% CTR, across 77 ad-name groups. **Verified**, live pull 2026-09-04. That headline number sits in the brand's own "not good" band, and part of it is real: the incumbent is finally aging. `Moms43 - 4 - V3`, live since 2026-04-15, took $3,543.83 last week for 109 leads at a **$32.51 cost per lead** on a $27.32 CPM, against its $22.28 across the full quarter. Its hook rate is unchanged at 46.11%. Nothing about the creative got worse. It just costs more now, which is what `ad-account-analysis.md` describes when CPM climbs while attention holds steady. **Inferred**, because frequency is not returned for this account and would be the metric that confirms it.

Meanwhile the August cohort is carrying the load. `moms-63 3e` is now the account's top spender at $3,638.53 for 214 leads at a **$17.00 cost per lead** on a $19.32 CPM, the cheapest impressions of any real spender. `moms-53 3`, the state-list ad, ran $1,709.12 at $18.78 with a **3.17% CTR and a $1.01 cost per link click**, both the best in the account. **Verified**, live pull. So the account's own newer, cheaper work is now the biggest line item, which is the first time that has been true all quarter.

**Delivery.** Over the 90 days: **95.3% female**, **81.2% aged 25 to 44**, 12.7% aged 45 to 54, **99.5% mobile**, and 60.3% Facebook to 39.1% Instagram. **Verified**, live pull 2026-09-04. Male share has risen in every one of the last six months, from 1.9% in March to 4.6% in August. Six consecutive months moving one way is a trend rather than noise, though at 4.2% it is still small.

## Key findings from the audits

**One. The format menu got shorter while the brand said it wanted the opposite.** The account ran 20 distinct formats in the prior quarter and 15 in this one. `Authority Figure`, `Street Interview`, `Infomercial / VSL`, `Humour`, `Offer Based` and `B-roll mashup + Voiceover` all went to zero. `Stitch Hooks` fell from $32,885.20 to $8.14. One format arrived, a single claymation ad worth $381.82. **Verified** by matched tag pulls across both windows. The brand's own words at intake were *"Right now we're mainly on iterations of our state angle that you will see in the account doing well. But not a ton of creative diversity."* **Stated.** Since it said that, diversity went down. Confidence **strong**.

**Two. The formats that hold attention are the ones getting no money.** `POV` runs a spend-weighted hold rate of 3.21% and touches roughly 70% of spend. `Graphic Video` holds 13.59%, `Educational` 12.61%, the unnamed `Other` bucket 11.49% and `Skit` 11.08%. Those four together touched 3.7% of the money. **Verified**, spend-weighted from ad-level video metrics. Every format at or near the craft floor is starved, and the three that take 88.8% of the money all sit under 6.4%. Confidence **strong** on the pattern, **mixed** on what it means, because the same audits show those high-hold formats also carry the *most expensive* leads: `Educational` at $32.00, `Graphic Video` at $31.82, `Other` at $33.62 against an account blend of $22.63. All three sit under $2,100 of spend, thin enough that a handful of leads swings the number.

**Three. Intensity buys the stop and calm buys the lead.** This is the sharpest single pattern in the stack and it arrives from three independent directions. The crying-mom set launched 2026-08-13 posted the best attention numbers in the account's history, a 57.02% hook rate and a 13.66% hold rate with an 8.08-second average play time on `moms54-3`, and produced leads at **$29.78 to $38.09**. The calm openers in the same month produced them at **$13.24 to $16.01**. **Verified** from all six ad records. The hook audit reaches the same split sorting by opener temperature. And the category's own organic feed says it a third time: **not one of the nineteen relevant videos in the TikTok mining library opens on crying**, and the strongest ones open calm and let the fact carry the shock. Read through `killer-performance-ads.md`, this is a stage-of-awareness failure rather than a craft failure. A mother landed in high-intensity distress is not in the mood to fill out a form about her ZIP code, and the conversion mechanic here is a solution-aware move. The CPM confirms it from the auction side: $36.75 and $37.83 on the two crying ads against $18.34 on the calm outdoor walk. Meta charged a premium to put grief in front of moms and the moms did not convert on it. **Inferred**, confidence **mixed**, since the crying set sits in a paused ad set at lower spend.

**Four. The picture is the variable, not the copy.** Six ads sharing the POV husband text hook carried $25,348.18 in August, 59.3% of the month. On the old reading that is message concentration. On the evidence it is an image portfolio question, because two of those six look nothing like the April original and delivered leads at $13.24 and $14.46 against the original's $23.37 with identical words. **Verified** from the visual hook fields read against period metrics. `andromeda-v2.md` explains why: Meta scans visual composition, people in frame, setting, camera angle and scene structure in the first three seconds, and a different text overlay on the same visual is a false differentiator that gets grouped into the same entity. The account has been running a messaging test inside a system that mostly grades pictures. **Inferred** from three independent same-month comparisons, confidence **strong**, and it cannot be verified because Meta does not expose entity grouping.

**Five. New files get built and then starved.** Fifteen satirical skit files went live on 2026-08-31, the largest format change since claymation died in July, and drew **$4.23 across 163 impressions in five days**. In the same week, three duplicates of already-proven ads took $2,080.15 pointed at the broken destination. The same winner-takes-all split shows up in three separate drops inside three weeks: the Moms53 drop put seven files up and one took 99.75% of the batch, the Moms65 drop put eleven up and one took 93.4%. **Verified** by ad-set-scoped lifetime pulls. Read through the breakdown effect in `ad-account-analysis.md`, this is Meta pacing budget toward the pocket it predicts will stay cheapest, which is exactly what the system is designed to do. The consequence is that every format test this brand runs dies before it can be measured.

**Six. Nobody qualified has ever been on camera.** Across 147 ads with delivery, every face is a mother talking about her own bill. `Authority Figure` ran four times last quarter for $8,884.74 and zero times this quarter. **Verified.** Meanwhile the brand's own context notes people search *"is Health for Moms legit"*, the comment corpus carries "don't believe this" and "Not recommend" twice, and a self-identified licensed health insurance advisor publicly told viewers *"never put your info online unless you want 100 calls a day about health insurance."* **Verified** verbatims from the ad comment pull. A peer saying "this worked for me" cannot answer a legitimacy question. The one half-test that exists is instructive: `MOMS30 - 1 - V20` put a pediatrician in a lab coat on screen, returned 381 leads at **$19.44**, and the doctor never speaks. The entire transcript is one narrator line. That is an unfinished test, not a failed one.

**Seven. The state gate is the mechanism, and it is also the friction.** All ten of the quarter's top-spend ads carry the approved-states list. The brand named it as its proven lever: *"State angle has worked very well if you see the account."* **Stated.** The one ad that puts the list in the **first frame**, `moms-53 3`, holds the account's highest CTR at 3.15% and cheapest click at $0.69 to $1.01 depending on the window. Every other ad reveals the list somewhere between eleven and thirty-three seconds, where the average viewer has already left at three to four seconds. **Verified.** Qualifying early did not cost this account volume. It bought better volume. The cost is public: *"Why is this being shown in IL if it's not on the list???😭🤦🏼‍♀️"*, *"Ofc Georgia ain't on there 🤣"*, *"What a joke!! They don't have quote for me In tx."* **Verified** verbatims. Texas appears on the state card in the top-spending ad, so either the lists differ between ads or the qualifier does something the card does not say.

**Eight. The account is buying a click on a promise the funnel then walks back.** Ninety-two comments landed in the 90-day window. Fifty of the 92 are a bare "Help" or "Info." Of the 38 substantive ones, the largest single cluster, ten of 38, is people finding out after clicking that they do not qualify, on grounds no ad mentions: *"It only works if you don't have any preexisting conditions. You gotta be perfectly healthy to qualify it looks like."* and *"Preexisting health condition of cancer disqualified me"* and *"But if you make under 30k a year you don't qualify smh."* **Verified** verbatims. The legal disclaimer that says "paid actor" and "not an insurance company" lands at forty-seven seconds in an ad whose average viewer leaves at 4.04. Against golden rule four in `killer-performance-ads.md`, zero confusion, this account has a real gap, and one comment says it best: *"I thought it was a Disney world membership."*

**Nine. The statics shutdown, which reframes all eight findings above.** Three separate 90-day audits describe this account as having never run a static. That is true of the trailing quarter and false of the account's life. **308 static ad-name groups, $168,907.73, 13,735 leads, $12.30 per lead.** **Verified**, my own pull 2026-09-04. The three biggest are `B1 samar- Copy` at $54,224.86 for 4,441 leads at **$12.21**, `B1 - Copy 7` at $30,339.32 for 2,584 leads at **$11.74** carrying the headline *"Left my big insurance company for a mom-focused one. 24% cheaper and I choose my own doctor 😌"*, and `B1 samar- Copy 1` at $14,633.08 for 1,231 leads at **$11.89** carrying *"Didn't know I could ditch my job's health plan… until I did."* None has run in months. What those headlines have in common is that each names a specific person in a specific moment, which is exactly what the current video does not do. The account did not just switch formats. It switched from talking to somebody specific to talking to nobody in particular, and it paid 44.7% more per lead to do it. Confidence **strong**.

## What came from Parker versus the brand or human audit

**What the brand stated directly, at intake or in its own context document.** These are the brand's claims, authoritative on intent and unverified on fact. The north star is *"CPL is important to scale but then we look at the lead quality as well before really scaling."* The cost-per-lead tiers are under $15 fantastic, $15 to $20 good, $20 to $25 meh, over $25 not good. The stated goal is "SCALE BABY!" with efficiency before volume. The stated creative problem is too little diversity beyond state-angle iterations. The stated video preference is *"We want to focus mostly on video ads. MAYBE some image ads are fine to find angles."* The stated proven lever is the state angle. The compliance rules are non-negotiable: no government or ACA references, no scare tactics, the villain is always the system rather than a named company, and a doctor character requires a real licensed physician. The stated calendar has one date on it, Open Enrollment November 1, planned two months ahead. The stated production volume is one to five net-new concepts and one to five iterations a month, with casting named as the top bottleneck.

**Where the brand's account contradicts the brand's own statement, and the conflict is the finding.** Three places. The brand said it wants more creative diversity and the format count fell from 20 to 15 in the three months since. The brand permitted statics for angle discovery and not one ran in 90 days, while its own static library holds the cheapest leads it has ever bought. The brand names November 1 as its most important date, and November 2025 took 5.4% of the readable thirteen months while March through May 2026 took 58.9%. **Verified** in all three cases. None of these is the brand being wrong about itself in a way it should be embarrassed by. All three are gaps between the plan and the spend that nobody had checked until now.

**What Parker inferred and no human has confirmed.** That the spend collapse was a budget decision rather than a performance failure, inferred from flat cost per lead through a 73.5% fall. That the four ads sharing the POV husband hook are very likely one entity wearing four creative IDs, inferred from shared text hooks and near-identical opening frames read against `andromeda-v2.md`, because Meta does not expose entity grouping. That the anger lane was abandoned by drift rather than by decision, inferred from nothing in the brand context or the four chat threads recording a call to kill it. That the crying openers fail on awareness-stage mismatch, inferred from the creative read against the CPM gap. Every one of these is reasoning, not fact.

**What a human strategist has interpreted.** Nothing. **No human has reviewed any audit in this stack.** The whole diagnosis is model-generated from Parker pulls plus the brand's own intake. Two cross-document errors have already been caught inside this build, the quiz-destination figures and the Open Enrollment history, and both were caught by a later prompt reading a live source rather than by review. That is the honest confidence ceiling on this page.

**What only the brand can answer.** What happens to a lead after it reaches the partner agency. Why the team stopped making statics. Why the scam-angle creative was switched off. Why spend fell 73.5% from April to July. Whether a licensed partner advisor can be filmed. Each of these is marked at the loop level below where it belongs.

## Audit movement since last read

**There is no prior read. This is the t0 baseline**, and it should be treated as the thing the next quarter is checked against rather than as a movement report. Where the audits reconstruct trajectory, they did it by pulling the prior 90-day window directly rather than by carrying an earlier strategist's read forward, so there is no prior diagnosis to agree or disagree with.

What did move, inside the stack itself, is worth recording because the next reader needs to know which layer wins.

**The statics finding overturned a premise three audits shared.** The 90-day creative strategy, performance and diversity audits all describe an account that has never run a static, and all three built recommendations on top of that. The quarterly whitespace analysis, run one day later against a lifetime rather than a 90-day window, found 308 static groups and $168,907.73 of spend. I re-verified it independently on 2026-09-04. **The lifetime read governs.** The 90-day audits are describing a shutdown, not an absence, and every "the brand has never tried statics" line in this brain should now read "the brand stopped running statics."

**The hold-rate theory got contradicted by the account inside four weeks.** The 90-day audits carried hold rate forward as the metric to fix. August then produced a $13.24 lead on a 2.38% hold rate and a $29.78 lead on a 13.65% hold rate, in the same month, in the same account. **Verified** across the top 20 by spend covering 99.36% of the month. That does not settle the question, and the honest state is that the general craft standard and this account's own numbers disagree. It sits in the loops below rather than being resolved by picking a side.

**One thing the account was asked to fix got worse instead.** The monthly performance report, generated 2026-09-03, told the team to fix the `go.healthformoms.co` redirect that week and to treat every ad routed through it as unscored rather than as a loser. In the week that followed, spend on that destination **more than doubled**, from $1,136.37 to $2,574.92, and three fresh duplicates of proven winners were launched straight onto it. **Verified** from matched destination pulls in the weekly snapshot. That is an execution gap and it stays visible here until it closes.

**One recommendation half-landed.** The monthly report asked for a footage sprint and a real format test before November. The footage sprint arrived: three of the four clean risers last week carry the identical POV husband hook over genuinely different pictures. The format test arrived and then got $4.23. Half of what was asked for shipped, and the half that shipped cannot be judged on 163 impressions.

**One test was retired before it settled.** The claymation set held 13.59%, 12.58% and 11.15%, the only creative in the account at or near the craft floor, and was killed on $516.86 and about four weeks. **Verified** by pulling all four files in July and finding none delivering in August. Format is the top rung of the differentiation hierarchy in `andromeda-v2.md`, and animation was the largest format change this account has ever made. Recorded as inconclusive, not as a failure.

## What later creative work should remember

**Change the picture, not the line.** This account's only proven step change in cost came from putting genuinely different footage under copy that already converts, and it was worth 43% on cost per lead in a same-month comparison. A different text overlay on the same visual is a false differentiator that Meta groups into the same entity. When a brief says "iterate," it has to mean a different person, a different setting and a different camera position in the first three seconds, not a new overlay on the same clip.

**Qualify in the first three seconds or do not qualify at all.** The average viewer leaves at 3.2 to 4.4 seconds. Every qualifier this account owns, the state list, the disclaimer, the eligibility rules, currently lands after she has gone. The one ad that puts the state list in the opening frame has the account's cheapest clicks and highest CTR. Anything a mother needs to know before she clicks has to be visible in the first frame.

**Two gates, and Parker can only see one.** Cost per lead is gate one. Lead quality is gate two and it lives with the partner agencies. Only 42 `Call` events fired against 4,336 leads in the window, so even the pixel's shadow of gate two is too thin to read. **Never call an ad a winner on cost per lead alone.** The correct phrase is a candidate that passed gate one, with gate two named as the open question, every single time.

**Never report ROAS, average order value, purchase value or add-to-cart for this brand.** The account has zero purchase events by design. It is a match-and-consult referral to partner insurance agencies, not a direct sale. Judge on cost per lead, lead volume, CPM, CTR, hook rate and hold rate. Quoting a return figure here is a fabrication, not a conservative estimate.

**Statics are proven inventory here, not an untested idea.** Any plan that treats a headline static as a new bet is starting from the wrong premise. They ran for months, they carry the cheapest leads in the account's history, and a headline plus a photograph needs none of the four upstream bottlenecks the brand named. Before the November ramp, that is the difference between five swings and twenty.

**Calm delivery, shocking fact.** The account's own numbers and an unrelated category feed agree that the emotion belongs in the fact rather than in the face. High-intensity distress on a cold audience wins the stop and loses the lead. If the harder story is worth telling, move the intensity to the three-to-five-second mark where `killer-performance-ads.md` puts the best benefit or the re-hook, and open calm.

**Casting is the untouched lever.** Every face in 147 ads is a mother talking about her own bill. That is one proof shape repeated 147 times in a category where the buyer is actively searching whether the brand is legitimate. The compliance rule blocks a fake doctor. It does not block a real licensed partner advisor, who is already inside the funnel and whom the brand already describes as *"like your Mom BFFs."*

**Concentration is a delivery risk, not only a creative one.** Roughly 70% of the quarter's spend touched one format container and four ads sharing one text hook carried 60.5%. Under the entity-ID rules that is very likely fewer distinct ads than the count suggests, which caps incremental reach and pushes frequency onto the same pool of mothers. The fix is difference, not volume.

## Open loops

**1. The cheapest leads this account ever bought came from the format it stopped making.**
Statics carry 22.7% of lifetime spend and 34.7% of lifetime leads at $12.30 against video's $22.23, and zero ran in the last 90 days. The two cheapest ads at real scale in the account's history are both statics that name a specific person in a specific moment, and both are dark.
*Pull: Gap.* It fired when a filtered lifetime pull returned 308 static ad-name groups worth $168,907.73 inside an account that three separate 90-day audits describe as having never run a static.
**Question: What made the team stop making statics?**
Four of the strongest moves available before November assume statics are on the table, and if something was learned that took them off it, that reason is a hard constraint nobody has written down. **This one only the brand can answer.**
*Territory: Product.*

**2. The account builds format variety and then does not spend on it.**
Fifteen satirical skit files launched 2026-08-31 and drew $4.23 across 163 impressions in five days, while three duplicates of existing winners took $2,080.15 in the same week. The same winner-takes-all split shows up in three separate drops inside three weeks, at 99.75%, 93.4% and effectively 100%.
*Pull: Surprise.* An account whose own diagnosis is that it lacks creative diversity built a batch of diversity and then gave it almost nothing, three times in a row.
**Question: What decides which new files in this account get delivery in their first week?**
Every format test this brand runs before November dies unmeasured if the answer is budget structure rather than performance, and that makes it a media-buying problem wearing a creative problem's clothes.
*Territory: Messaging.*

**3. Watching longer costs more here, and the craft says it should cost less.**
The account's cheapest lead comes from an ad holding 2.39% of viewers with a 3.38-second average play time, and its best-holding ads sit in the worst cost band, at $29.78 to $38.09. The craft floor is 12% to 15%. In August the ads that held people longer cost more per lead, not less, across the top 20 by spend covering 99.36% of the month.
*Pull: Tension.* The general method and this account's own numbers cannot both be right about what attention is worth here.
**Question: How much of this account's lead volume comes from people who watched past three seconds?**
If the answer is almost none, then the body of every ad matters far less than the industry default assumes, and the whole production budget should move to first frames.
*Territory: Product.*

**4. The creative is picking the audience, and nobody planned that.**
Three ads with no targeting difference between them produced three completely different age distributions. The self-employed static put 54.4% of its spend on women over 45, the skit family put 40.2% there, and the silent-clinician ad went the other way with 52.7% on women aged 25 to 34, against an account average of 21.2% over 45.
*Pull: Surprise.* The format and the copy were never designed as a targeting tool and they appear to be acting as one anyway.
**Question: How much of this account's audience mix is being set by the words and pictures in the creative rather than by the targeting?**
The brand says it wants to reach moms of all ages with kids of all ages, and if a sentence is the lever that reaches a forty-eight-year-old, then the persona problem and the brief problem are the same problem.
*Territory: Personas.*

**5. Nobody with credentials has ever appeared in this account.**
Across 147 ads with delivery, every face is a mother talking about her own bill. Authority creative ran four times last quarter and zero times this quarter. In the same window the comment section produced "don't believe this," "Not recommend" twice, and a licensed advisor publicly warning viewers not to submit their information. The one half-test, a pediatrician on screen who never speaks, returned leads at $19.44.
*Pull: Gap.* There is a trust question the brand knows it has, and not one ad in the account is built to answer it.
**Question: Who do mothers actually trust to tell them the truth about health insurance?**
The answer decides whether the next production budget buys a different casting call or a different proof, and the brand names casting as its top bottleneck either way.
*Territory: Creators and talent.*

## Appendix - Parker media links

Links and paths preserved exactly as returned by the Parker MCP.

**M001 — `Moms43 - 4 - V3`.** The incumbent. $43,119.77 over the 90 days for 1,935 leads at $22.28, hook rate 45.36%, hold rate 3.28%, average play time 4.04 seconds. Lifetime $57,506.21 for 2,668 leads at $21.55. Last 7 days $3,543.83 for 109 leads at $32.51 on a $27.32 CPM. Carries 116 page likes against 1,987,158 impressions, 327 shares and 385 saves. Created 2026-04-15. Discussed in the diagnosis, the current-state read and findings four and eight.
Facebook ad id: 120241073380060519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

**M002 — `moms-63 3e`.** The current top spender. $5,448.56 over the 90 days at $15.44, and $3,638.53 last week for 214 leads at $17.00 on a $19.32 CPM, the cheapest impressions of any real spender. The POV husband line over outdoor mother-and-son footage. Created 2026-08-14. Discussed in the diagnosis and finding four.
Facebook ad id: 120247093478820519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4
Landing page: https://www.healthformoms.co/save/

**M003 — `moms-63 2b`.** The account's cheapest lead at scale, $5,529.74 over the 90 days for 417 leads at $13.26. Same text hook as M001, different picture. Created 2026-08-14. The other half of the footage-versus-copy comparison in finding four.
Facebook ad id: 120247093361410519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
Landing page: https://www.healthformoms.co/save/

**M004 — `moms-53 3`.** The state list in the first frame. $2,041.29 over the 90 days at $16.07 with a 3.15% CTR and a $0.69 cost per link click, both best in the account. Created 2026-08-25. Discussed in finding seven and carries the Illinois, Georgia and Texas comments.
Facebook ad id: 120247254787160519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4
Landing page: https://www.healthformoms.co/save/

**M005 — `Moms43 - 5 - V1`.** The best-holding ad at real scale, 7.59% over the 90 days on $10,170.58 at $23.71, and 7.96% last week on a $40.14 CPM at $30.20. The screenshot-outrage overlay. Created 2026-06-01.
Facebook ad id: 120243987355020519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120243987355020519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0fe2980848d12fe1c6fd107a759e68fe37d8776c34235b5fab3c15e751af171d.mp4
Landing page: https://www.healthformoms.co/save/

**M006 — `Moms Nahuel WV#1 - V9 - Copy`, the broken-destination variant.** $1,639.35 lifetime, 690 link clicks, 63 landing page views, 9.1% landing rate, 6 leads, $273.23 cost per lead, click quality 9.13. Created 2026-08-17. The canonical `go.` case in the audit-provenance section.
Facebook ad id: 120247145872230519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872230519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/645496c411d82a546a3e2deada69459c716615ad09f635ca0b978625c2778b37.mp4
Landing page: https://go.healthformoms.co/save/

**M007 — `Moms Nahuel WV#1 - V9 - Copy`, the working-destination variant.** Identical video file. $404.23 lifetime, 213 link clicks, 171 landing page views, 80.3% landing rate, 21 leads, $19.25 cost per lead, click quality 80.28. Created 2026-08-11. The control that proves the break is plumbing, not creative.
Facebook ad id: 120247022199760519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247022199760519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Landing page: https://www.healthformoms.co/save/

**M008 — `Moms Nahuel WV#1 - V9 - Copy`, the two quiz variants.** $0.94 on 63 impressions and $0.60 on 17 impressions, both created 2026-09-02. Unmeasured.
Facebook ad ids: 120247367204750519 and 120247373812940519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247367204750519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Landing page: https://quiz.healthformoms.com/#/indvfam

**M009 — `MOMS38 - 1 - V1`.** The scam-hook ad. $54,173.20 in the prior window at a 17.29% hold rate, 7.08-second average play time and a $20.15 cost per lead. Zero spend this quarter. The abandoned lane.
Facebook ad id: 120239479305920519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239479305920519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/50a0309be06d87e55299b9e00d7962b88516c847dec96e80cfd47e6ba5959b66.mp4
Landing page: https://www.healthformoms.co/save/

**M010 — `B1 samar- Copy`.** The largest static in the account's history, $54,224.86 lifetime across 39 variants for 4,441 leads at $12.21, on a $16.18 CPM. Created 2025-07-17. Dark.
Facebook ad id: 120228910482200519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120228910482200519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/59bf52c09c6081e3dfc63e0b17e649c989b490ad5b03079e469d1dc258e2cc0f.jpg
Landing page: https://www.healthformoms.co/save/

**M011 — `B1 - Copy 7`.** The switching static. $30,339.32 lifetime across 5 variants for 2,584 leads at $11.74. Headline *"Left my big insurance company for a mom-focused one. 24% cheaper and I choose my own doctor 😌"*. Created 2025-02-26. Dark.
Facebook ad id: 120216241083030519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120216241083030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/7e3133fccf8b205622146f7297669b76296123fb46177e5262ee89f0040ca8ba.jpg
Landing page: https://www.healthformoms.co/save/

**M012 — `B1 samar- Copy 1`.** The employer-plan static. $14,633.08 lifetime for 1,231 leads at $11.89 on a $15.05 CPM. Headline *"Didn't know I could ditch my job's health plan… until I did."* Created 2025-07-17. Dark.
Facebook ad id: 120227092759640519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227092759640519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b219b0aa7f7e7ed8d83fa471803f4b6c96ad98b2de118b2a8e68038439e759a9.jpg
Landing page: https://www.healthformoms.co/save/

**M013 — `moms54-3`.** The distress lane at its strongest and most expensive. 57.02% hook rate, 13.66% hold rate, 8.08-second average play time, $29.78 cost per lead on $1,283.69. Created 2026-08-13.
Facebook ad id: 120247063711860519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063711860519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/5a62b11062812d9509cb2cd8c95e89777a15d1a6ac1cdb1f6e9a92eb77f93a9d.mp4
Landing page: https://www.healthformoms.co/save/

**M014 — `Moms46 - V1`.** The claymation file, 13.59% hold rate and 6.77-second average play time on $381.82. Retired before it settled.
Facebook ad id: 120246046671140519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120246046671140519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0e843f33de6045345de8bafc06819312831ea5db2037b5a0670dc09af3412597.mp4
Landing page: https://www.healthformoms.co/save/

**M015 — `moms 68 1#`.** The starved format batch. $0.85 and 32 impressions across its first five days. Woman in a black leather jacket, text hook *"This is why health insurance in America is a scam..."*. Created 2026-08-31. Loop two.
Facebook ad id: 120247340952300519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247340952300519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/7aa5cf3b3cd5d470e40e939f3ab051cd97d6c2ae5d4dcac6ca317f9fe5dda470.mp4
Landing page: https://www.healthformoms.co/save/

**M016 — `moms-65 1a`.** The riser whose cost improved as it scaled, $1,289.09 last week for 58 leads at $22.23 against $28.85 the week before. Stylish mom at a modern black front door. Created 2026-08-27.
Facebook ad id: 120247285907980519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247285907980519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/bb071de9e8d0e46ca498a10528b066d07bf324999cb3e1b0d11d83c83592cc67.mp4
Landing page: https://www.healthformoms.co/save/

**M017 — Facebook ad comments.** 92 comments in the 90-day window, 1,322 lifetime, read in full through Parker MCP `search_facebook_ad_comments_sql` by the upstream audits. The source of every customer verbatim on this page, used in place of a review corpus per the substitution rule in `running-notes/missing-context.md`. No dashboard link exists for a comment pull; it is reproduced by querying brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`.

**M018 — Brand context document.** Retrieved through Parker MCP `get_brand_persona` for brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`. The source of the cost-per-lead tiers, the compliance rules, the five stated ICPs and the stated testing history. No public link; reproduced by that call.

---

This is everything I know about Andromeda v2.
