---
brand: health-for-moms
doc: biweekly-iterations-report
report_date: 2026-09-04
generated_on: 2026-09-04
refresh_by: 2026-09-18
date_range: 2026-08-22 to 2026-09-04
prior_report_lineage: "none. This is the first bi-weekly iterations report for this brand, the t0 baseline. There is no prior report to take in as context and no prior round of recommendations whose outcomes could be carried forward. Every iteration history below was reconstructed from the account itself rather than read from a log."
data_sources_read: [live Meta ads manager via Parker MCP search_facebook_ads_sql on account HealthForMoms act 484897827497337 (16 pulls run 2026-09-04, including a four-ad adIds lookup with transcripts, two text-hook family cuts, and two ad-set family cuts), Parker MCP search_facebook_ad_comments_sql (25 comments since 2026-08-22), audits/2026-09/weekly-performance-snapshot.md, audits/2026-09/monthly-performance-report.md, sub-context-docs/marketing-calendar-and-campaigns.md, running-notes/brand-rules.md, running-notes/success-definition.md, running-notes/missing-context.md]
knowledge_docs_read: [parker-system/creative-strategy-context/selecting-ads-to-iterate-on.md, parker-system/creative-strategy-context/iterations.md, parker-system/creative-strategy-context/ad-account-analysis.md, parker-system/creative-strategy-context/ad-metrics-glossary.md, parker-system/creative-strategy-context/killer-performance-ads.md, parker-system/creative-strategy-context/andromeda-v2.md]
ads_selected_for_iteration: [moms-63 3e, moms-53 3, moms-65 1a, Moms43 - 4 - V3]
context_docs_loaded: yes
data_limitations:
  - "No iteration history log exists for this brand. briefs/ is empty and nothing in running-notes/ records what has been tried or what outcome the team assigned to it. Every iteration history below was reconstructed from the account: shared media hashes, shared text hooks, shared creation timestamps and ad-set groupings. The lineage is verified from the account; the outcome the team assigned to each variant is not recorded anywhere and is therefore read from spend and cost per lead rather than from a decision. Marked inferred wherever that distinction matters."
  - "No prior bi-weekly report exists, so no recommendation from a previous round can be scored here. The success criteria set below are the first ones on record for this brand, and the 2026-09-18 report is the first that will be able to judge anything."
  - "Lifetime metrics lag the period series in this account's snapshot. moms-53 3 returns $1,955.60 lifetime against $2,097.43 for the trailing fourteen days, and moms-65 1a returns $1,283.97 against $1,376.63. Where the two disagree the period figure is used and the gap is named."
  - "Reach and frequency are not returned for this account. Every fatigue read below rests on CPM moving against a flat hook rate, which ad-account-analysis.md accepts as the shape of a used-up audience but which frequency would confirm. Marked inferred, not verified."
  - "Placement-level breakdown is not exposed for this account. Platform splits between Facebook and Instagram are available and used; Feed versus Reels versus Stories is not."
  - "Meta does not expose entity-ID grouping. Every claim below about which files Meta likely treats as one ad is inferred from the visual hook, text hook and first-three-seconds description read against andromeda-v2.md, never read directly."
  - "Video transcripts carry spoken lines with timestamps but do not describe what is on screen second by second. Where a recommendation names a visual beat, it is built from the visual_hook field plus the transcript timing, not from a frame-level review."
  - "Lead quality is invisible to Parker. It sits with the partner insurance agencies. Every ad below has cleared gate one only, and no recommendation here should be read as clearance to scale."
  - "Northbeam is not connected. All figures are Meta-reported on the Meta default attribution window."
  - "No ad naming convention was supplied. Names and ad-set names are used to group and date variants only, never as evidence of what a creative is or does. Every creative claim rests on the text hook, verbal hook, visual hook, angle and transcript fields."
---

# Bi-weekly iterations report — Health For Moms — 2026-09-04

The window is 2026-08-22 to 2026-09-04, and the first thing to say about it is that the account is in better shape than its headline number suggests. Blended cost per lead across the fortnight reads high because ads pointed at `go.healthformoms.co/save/` are still running and still converting about seven percent of the clicks they buy. Stripped out, the account spent **$24,644.97 clean and bought leads at roughly $22**. Four ads carry **$15,340.24 of that, or 62.2%**, and they returned **712 leads at a $21.55 cost per lead**. Those four are the report. Three of them are high-risers by the definition in `selecting-ads-to-iterate-on.md`, and the fourth is the incumbent that has been running since April and is now the most expensive lead in the account. Everything below is gate one only: the brand's own definition of a winner is cost per lead first and then lead quality, and lead quality lives with the partner agencies where Parker cannot see it. Nothing here is a clearance to scale.

Four ads did not make the cut and it is worth saying why. **moms55-1** rose from $7.75 to $704.90 and is genuinely interesting, but it has seven days of run time and 2.9% of the window's clean spend, which is exactly the "insignificant spend and short run-time" case the selection doc tells you to leave alone for now. **moms-63 2b** fell 65% in spend, but it fell because its own ad-set sibling rose, so the breakdown effect explains it and there is no separate ad to iterate. **Moms43 - 5 - V1** spends real money at a $31.07 cost per lead on a $41.45 CPM, and it is fatiguing the same way the incumbent is, but it is a smaller version of the same problem and the same fixes apply. **moms 68**, the fifteen-file satirical batch launched 2026-08-31, is the most creatively interesting thing in the account and cannot be iterated on at all, because it has spent $4.23 and never been tested. That last one is an open loop, not an iteration.

One pattern runs under all four entries and it is the most useful thing this report found. **Every round of iteration this account has run that changed the footage beat the original. Every round that kept the footage matched it.** That is not a theory borrowed from a method doc; it is this account's own history, and it is laid out ad by ad below.

---

## moms-63 3e

### The ad

Media: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4`

Ad name **moms-63 3e**, facebook_ad_id 120247093478820519, ad set Moms63, campaign USHA - ABO - TEST - MOMS. Launched **2026-08-14**, so **21 days running**. Over the fortnight it took **$5,093.33** for **309 leads at a $16.48 cost per lead**, on a **42.87% hook rate**, a **2.91% hold rate**, a **1.63% CTR** and an **$18.77 CPM**, the cheapest impressions of any big spender in the account. Cost per link click $1.51, landing page views 2,894 from 3,364 link clicks, an 86.0% landing rate. Lifetime it has taken **$5,240.28 for 339 leads at $15.46**. Week over week it went from $1,372.61 to $3,720.72, up 171%, the largest spend gain in the account. Format is a produced lifestyle video with a female voiceover. Persona target is the account's core buyer, a mother aged 25 to 44 on mobile, which carries 82.1% of the account's age spend this week. Per-ad demographic splits were not pulled for this file, so the persona read is the account's, not this ad's. Destination `https://www.healthformoms.co/save/`, the working one.

The ad opens silent. A well-dressed mother and her young son walk hand in hand outdoors near a house, warm daylight, the camera holding them in easy motion, and across the frame sits the text hook the account has run since April: *"POV: Telling your husband you found better health insurance, saved $400 a month, AND the deductible is zero. Wife of the year energy. 💗"*. Music only. Nobody speaks for eleven seconds. Then a woman's voice arrives mid-thought, as if she has been talking to a friend: *"I almost scrolled past this because I thought, 'I already have health insurance, this doesn't apply to me.'"* At 0:17 she corrects herself, *"But then I realized, having health insurance doesn't necessarily mean you have the best option available to you,"* and at 0:22 she names the pain in the audience's own terms, *"Especially if you're paying every month and still have a deductible that's thousands of dollars."* At 0:27 comes the turn, two words: *"So I checked."* From 0:28 she lays out the qualifier and the offer, a mom in one of these states, a $0 deductible, better premium rates, thirty seconds to look. And then at 0:40 the ad does the smartest thing in it: *"Worst case, you check and stick with what you have. Best case, you realize you've been paying way more than you needed to."* A narrator closes at 0:50 with the brand name and "save up to 30%."

### Why this ad is worth iterating on

This is a **high-riser** in the exact sense `selecting-ads-to-iterate-on.md` defines it. The doc describes a creative that "immediately showed exponential growth" with media buyers allocating large amounts quickly and the creative standing the test, and says that when you see this pattern, "which will be visible even after 3 days of being live, you should immediately be looking for ways to iterate on it." moms-63 3e went from $1,372.61 to $3,720.72 in a week, a 171% increase, and became the largest single clean line item in the account while its cost per lead moved only from $14.92 to $17.15, staying inside the brand's own "good" band of $15 to $20. It is also the top spender, which is the doc's first test: Meta's own system has predicted this is the most potent ad in the account right now, and the doc is explicit that spend is the signal because of how the breakdown effect works.

It passes the second test too, run time in the context of spend. Twenty-one days is young, but the doc is clear that run time only matters against factual performance, and this one has taken $5,093.33 in a fortnight without its efficiency breaking. And it clears the promotional caveat cleanly, because the account runs no discounts and this is not a promo ad, so there is no risk of iterating on a spike that dies when an offer ends.

The bottleneck is not hard to find and it is startling once you see it. Per the diagnostic in `iterations.md`, the main constraint here is hold rate, and specifically what the hold rate is hiding. Hold rate is **2.91%**, average play time is **4.03 seconds**, and only **6.57% of three-second viewers reach fifteen seconds**. The first spoken word in this ad lands at **0:11**. So the entire persuasive argument, including the risk reversal at 0:40 that is the single best line in the file, is being delivered to roughly six percent of the people who stopped scrolling. That is the pattern `iterations.md` calls "strong CTR but low hold rate," where "the hook is doing its job but something after it is losing them," and it tells you to look at "pacing, length, the transition from hook to body, and whether the product introduction comes too late." Here the product introduction and the argument both come very late indeed. The working elements to protect are the visual hook, which is producing a 42.87% hook rate against the 30% floor in `ad-account-analysis.md`, the cheapest CPM in the account at $18.77, and the text hook itself, which across twelve ads carrying it has produced $86,135.90 of lifetime spend at a $19.77 cost per lead. The element to iterate is everything between second zero and second eleven.

### Iteration history

This file is round three of a four-round program, all of it reconstructed from the account because no iteration log exists. *Verified* from shared media hashes, shared text hooks and matched creation timestamps; the outcome assigned to each round is *inferred* from spend and cost per lead, since no decision was ever written down.

1. **2026-03-18 — the originals.** MOMS37 - 12 - V5 and MOMS37 - 13 - V5, two ads sharing one video file, a mother lying in bed with her baby under a white duvet, carrying this exact text hook. $558.90 at a **$6.58 cost per lead** and $562.42 at a **$7.50 cost per lead**. These remain the cheapest leads this hook has ever produced. Both now sit in a paused ad set.
2. **2026-04-06, relaunched 2026-04-15 — round one, three variants on the same bed footage.** Moms43 - 4 - V1, V2 and V3. V3 took **$57,506.21 at $21.55**, V1 took **$12,153.59 at $21.32**, V2 took **$1,852.41 at $14.59**. V1 and V2 are now paused. The outcome worth noticing: the variant with the best cost per lead got a fifteenth of the budget of the one with the worst, and all three landed within a few dollars of each other because none of them changed what the viewer sees.
3. **2026-08-14 — round two, new footage under the same words. This ad.** moms-63 1e, 2b and 3e launched together. 2b took **$5,529.30 at $13.26**, 3e took **$5,240.28 at $15.46**, and 1e took **$0.03 on two impressions**. Both files that got delivery beat the April incumbent by six to eight dollars a lead.
4. **2026-08-27 — round three.** moms-65 1a, covered in its own entry below, at $1,283.97 and a $21.40 cost per lead and still improving.
5. **2026-09-03 — round four, in flight.** The moms62 drop, eight files, $155.68 for 9 leads at a $17.30 cost per lead on three days of delivery. Too young to call.
6. **2026-08-31 and 2026-09-02 — not iterations.** This exact file was duplicated twice and re-pointed at `go.healthformoms.co/save/` and then `quiz.healthformoms.com/#/indvfam`. The copies took $537.23 for 8 leads at $67.15. These are destination tests wearing an iteration's clothes and they tell you nothing about the creative.

What the history says for this round: hook headline changes have never been tried on this file, footage changes have been tried twice and worked both times, and nothing has ever been done about the eleven silent seconds.

### Recommended iterations

**Cold Open — pull the risk reversal to second zero.** This is the Cold Open pattern from the Video: Pacing Iterations menu in `iterations.md`, described there as cutting the intro entirely and dropping the viewer straight into the most compelling moment, and it is the right call because the diagnosis says the intro is losing viewers and the strong content starts too late. Take the exact six seconds from 0:40 to 0:46, *"Worst case, you check and stick with what you have. Best case, you realize you've been paying way more than you needed to,"* and place it at 0:00 over the same walking footage, keeping the POV text hook on screen. At 0:06 cut to what is currently the 0:11 line, *"I almost scrolled past this because I thought, 'I already have health insurance, this doesn't apply to me,'"* which now plays as her explaining what led her to check, and let the rest of the ad run unchanged from there. The transition works because the risk reversal is a question and the scroll-past line is the answer, so the viewer hears a reason to keep watching before she hears anything about insurance. This is also an open-loop hook in the sense the hook doctrine describes, an unresolved statement that the body then resolves. **Success criterion for the 2026-09-18 report:** hold rate above 5.0% and fifteen-second retention above 10.0% at $2,000 or more of spend, with cost per lead holding under $20.

**Burned-In Headline carrying the check-it-yourself promise.** This is the Burned-In Headline pattern from the Edit Iterations menu, and it is the deliberate quick win `iterations.md` asks you to include: very low effort, no reshoot, no new footage. Add a persistent text bar across the top of the frame from 0:03 to the end reading the worst-case, best-case idea in the customer's own compressed words. It sits above the existing POV text hook rather than replacing it, so the proven line stays intact and the new bar answers the "why keep watching" question for the ninety-four percent who never reach 0:40. The reason to run this alongside the Cold Open rather than instead of it is that they are separate variables and `iterations.md` is explicit that isolating variables is how you learn which change drove the result. **Success criterion:** CTR above 2.0% against the current 1.63%, at $1,500 or more of spend.

**Video to Static on the state-list moment.** This is the Format Iterations pattern Video to Static, and the signal-change ladder in `iterations.md` calls format the loudest lever available, the one to reach for when you want fresh distribution. The case here is unusually strong and it is not generic. This account currently runs no statics at all in its live top twenty, and per `marketing-calendar-and-campaigns.md` the cheapest era in the account's history was the SAMAR static run from 2025-07-17, 87 ads at a **$12.34 cost per lead** against the $22.95 the current video era averages. The account abandoned its cheapest format and has not tested it since the winter. Do not compress this whole video into a card. Take the single strongest claim, the $0 deductible plus the state qualifier, pair it with a still frame of the mother and son walking, and set the headline in the voiceover's own register rather than in ad copy. **Success criterion:** any static built from this concept clearing a $20 cost per lead on 50 or more leads.

**Human Desire Swap from social approval to protection.** This is the Human Desire Swap from the Messaging Iterations menu, which `iterations.md` lists among its historically highest-confidence iterations and describes as keeping product, format and structure intact while changing the emotional engine. Read through the Life Force 8 frame in `killer-performance-ads.md`, the current hook runs on Social Approval and on being superior: the win is her husband's reaction, "wife of the year energy." The account has never tested the same offer built on Care and Protection of Loved Ones, which is the drive the brand's own positioning rests on. There is evidence this matters. The most-liked comment in the window, tied at one like, sits under this casting family and reads *"I'm sure the mom that can afford matching outfits prob just pays in cash 🤦‍♀️"*. A mother who reads the family as wealthy does not see herself in a status win. Rewrite the text hook so the payoff is the child being covered rather than the husband being impressed, keep the footage, keep the voiceover, change nothing else. **Success criterion:** cost per lead at or under $16.48 at $1,500 or more of spend, plus fewer affordability objections in the comment thread than the two logged in this window.

---

## moms-53 3

### The ad

Media: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4`

Ad name **moms-53 3**, facebook_ad_id 120247254787160519, ad set Moms53, campaign USHA - ABO - TEST - MOMS. Launched **2026-08-25**, so **10 days running**. Over the fortnight it took **$2,097.43** for **128 leads at a $16.39 cost per lead**, on a **35.44% hook rate**, a **3.88% hold rate**, a **3.13% CTR** and a **$21.85 CPM**. Cost per link click **$0.97** and cost per click $0.70, both the best in the account by a wide margin. Landing page views 1,640 from 2,153 link clicks, a **76.2% landing rate**, which is meaningfully below the account's 85.4% clean rate. Week over week it went from $465.61 to $1,631.82, up 250%, while cost per lead went from $10.58 to $19.43. Lifetime reads $1,955.60, which is lower than the fortnight because the lifetime snapshot lags. Format is a short direct-to-camera UGC testimonial. Destination `https://www.healthformoms.co/save/`.

A woman in a grey tank top stands in front of a white screen filled with a long list of US state names under the heading *"Approved State List ✔️"*, and she speaks straight into the lens, warm and slightly breathless, like someone passing on a tip: *"I'm so thankful for the mom that told me about this."* That is second zero. At 0:02 she qualifies the room in one long sentence: *"If you're a mom and you live in one of these states and you're tired of paying high deductibles, high premiums for health insurance for your family, listen up."* At 0:09 she gives the mechanic, *"It takes you 30 seconds, it's a brand new website,"* and from 0:12 she closes: as long as you live in one of those states, click below, fill it out, see if you qualify for lower premiums and a $0 deductible. The whole thing is about twenty seconds. There is no music bed carrying an empty opening, no produced voiceover, no lifestyle footage. It is one person, one screen of text, one recommendation.

### Why this ad is worth iterating on

This clears the **high-riser** bar the same way moms-63 3e does, but harder and faster: 250% spend growth week over week on ten days of life. It also carries the account's single most distinctive performance signal, and `selecting-ads-to-iterate-on.md` has a specific guideline for exactly this. Its second additional guideline says that when you see uncommon hooks that are prominent in the account but not industry standard, you should recognise them as good and use them further in the iterating process, and it gives the example of a creator introducing herself, normally a weak opener, working anyway. That is precisely what is happening here. A wall of state names is not a hook anyone would design from a taxonomy, and it is producing a **3.13% CTR** against the account's 1.94% and a **$0.97 cost per link click** against $1.75. The brand told us this angle is its best, verbatim in the brand context document: *"State angle has worked very well if you see the account. Emotional and direct response."* The account now agrees with them on clicks.

There is a second and much rarer reason to iterate here. This ad holds attention in a way nothing else in the account does. **6.65% of its three-second viewers watch to 100%**, against 0.74% on moms-63 3e and 0.86% on the incumbent. Its 25% completion rate is **69.87%**. In an account whose spend-weighted hold rate is 3.78% against a 12% to 15% floor, this is the only file that has ever earned a real watch, and the reason is structural: it is short and the argument starts immediately. That is an asset the account does not otherwise have, and per `iterations.md`, the working elements you protect are the ones the data says are performing. Protect the length, the direct-to-camera framing and the mom-to-mom register.

Two bottlenecks. First, **efficiency is decaying under scale**: cost per lead went from $10.58 to $19.43 as spend tripled, which is the "good metrics but not scaling further" pattern shading into the "CPA rising over time" pattern in `iterations.md`. Second, and more actionable, this ad **loses clicks between the click and the page**. Its landing rate is 76.2% against 85.4% for the rest of the clean account, on the same working destination, which means the gap is not the page, it is who is clicking. It is buying the cheapest clicks in the account and a larger-than-normal share of them evaporate before arrival. Read against the hook doctrine's first core principle, *"prioritize relevance over raw attention. Wrong audience attention is wasted spend,"* and against the click-pre-qualification idea in `visuals.md`, that reads as a qualification problem in the opener. The comment thread says the same thing out loud. In this window three separate commenters named a state the product cannot serve: *"Why is this being shown in IL if it's not on the list???😭🤦🏼‍♀️"* on 2026-09-02, *"Ofc Georgia ain't on there 🤣"* on 2026-08-29, and *"What a joke!! They don't have quote for me In tx"* on 2026-08-31.

### Iteration history

**This file has never been iterated on. It is on its first cycle.** But it did not launch alone, and what happened to its siblings is the most important context for what to do next. *Verified* from an ad-set-scoped lifetime pull run 2026-09-04.

1. **2026-08-25 — the Moms53 drop, seven files, one timestamp.** All seven were created at 09:59:43 on the same day into the same ad set. moms-53 3 took **$1,955.60 of the batch's $1,960.50, which is 99.75% of it.** The other six split **$4.90** between them.
2. **moms-53 1, $0.12, and moms-53 4, $0.33.** Both carry the *identical* verbal hook to the winner, *"I'm so thankful for the mom that told me about this,"* on different footage: a woman in a tie-dye tank in a bedroom, and the same creator in a room with mirrors and plants. This matters enormously. **A creator-and-setting reshoot on this exact script has already been attempted, twice, and neither variant ever got enough delivery to be tested.** Recommending "reshoot the script with a new creator" as a fresh file in the same ad set would be re-running a test that has already failed to run.
3. **moms-53 5, $2.06, and moms-53 6, $1.95.** Both pivot to the deductible-anger angle, one as a split-screen reaction video, one direct to camera, under *"Health Insurance is a scam."* Also starved.
4. **moms-53 2, $0.33, and moms-53 7, $0.11.** A blonde woman in a pink cardigan under *"I wish this was a joke... (health insurance)"* and one file with no described opener. Also starved.

The honest read of this history is that the batch did not test seven ideas. It tested one, because Meta picked a winner inside the first hours and the breakdown effect did the rest. Six real creative bets in this drop remain genuinely unknown.

### Recommended iterations

**Qualifier-first hook — put the state requirement in the first two seconds, spoken and legible.** This is a Demographic Hook iteration from the twenty hook formats in `iterations.md`, the format built to make it instantly obvious who the ad is for, and it targets the landing-rate bottleneck rather than the hook-rate one. Today the state requirement is on screen from 0:00 as a wall of small text but it is not spoken until 0:02 and it is buried mid-sentence inside a long qualifying clause. Recut so the very first spoken words name the constraint plainly, something in her own register that leads with the state list rather than with her gratitude, and hold the list at a size that is readable on a phone before the sentence ends. Then cut straight into the existing 0:00 line, *"I'm so thankful for the mom that told me about this,"* at roughly 0:03, so the gratitude becomes the payoff rather than the setup. This deliberately trades some raw click volume for relevance, which is the trade the hook doctrine says to make. **Success criterion for the 2026-09-18 report:** landing rate above 85% and cost per lead at or under $17.00 at $2,000 or more of spend. Cheaper clicks are not the goal; more of them arriving is.

**Length Extension carrying the pre-existing-conditions proof.** This is the Length Extension pattern from the Video: Length Iterations menu, described as expanding a short winner with more proof, story or detail, and `iterations.md` says it is the right call when a short ad is winning and you have additional proof to add. This ad is the only file in the account that has earned the attention to carry proof, at 6.65% completion. And the proof it needs is named for us by the customers. On 2026-09-02 a commenter wrote *"Preexisting health condition of cancer disqualified me."* On 2026-08-31 another asked *"Is this insurance or something like a Christian health share?"* On 2026-09-01, *"But if you make under 30k a year you don't qualify smh."* The monthly report named this objection as the highest-value new script in the queue and it is still unwritten. Add ten seconds after the current 0:12 close, in the same one-take register, that answers what the plan is and who it is actually for, and then repeat the CTA. Against golden rule four in `killer-performance-ads.md`, zero confusion, this is the account's clearest failure and its cheapest fix. **Success criterion:** completion rate holding at or above 5.0% on the longer cut, cost per lead at or under $20.00 at $1,500 or more of spend, and a visible drop in category-confusion comments.

**Comment Reply format built on a real objection.** This is the Comment Reply pattern from the Format Iterations menu, and the Comment Response hook, which is format one of the twenty and which the hook doctrine names as the right choice for a solution-aware audience carrying objections. This brand's audience is squarely solution-aware: they already have insurance and already believe it is failing them. Open on a screenshot of a real comment from this account's own thread, the pre-existing-conditions one, and have the same creator answer it directly to camera. The reason to run this as a separate file rather than folding it into the extension above is that it is a different job. The extension adds proof to a working ad; this one leads with the objection and is a genuinely different first three seconds, which per `andromeda-v2.md` is what it takes to be treated as a new ad rather than grouped with the original. **Success criterion:** cost per lead at or under $20.00 on 50 or more leads, and a hook rate at or above 35% to show the objection opener stops the same people the state list does.

**A delivery note that applies to all three.** Do not launch these into the Moms53 ad set. The history above shows six files in that set never got out of the gate. Give each iteration its own ad set with its own budget, or the test will not happen.

---

## moms-65 1a

### The ad

Media: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/bb071de9e8d0e46ca498a10528b066d07bf324999cb3e1b0d11d83c83592cc67.mp4`

Ad name **moms-65 1a**, facebook_ad_id 120247285907980519, ad set Moms65 + Moms 68, campaign USHA - ABO - TEST - MOMS. Launched **2026-08-27**, so **8 days running**. Over the fortnight it took **$1,376.63** for **63 leads at a $21.85 cost per lead**, on a **32.69% hook rate**, a **4.29% hold rate**, a **1.64% CTR** and a **$26.20 CPM**. Week over week it went from $201.98 to $1,174.65, up **482%**, the largest proportional gain of any established ad, and its cost per lead **improved** over the same step from $28.85 to $20.98. It is the only riser in the account whose efficiency got better as it scaled. Its batch delivers **63.0% on Instagram** against the account's 38.8%, and skews **51.0% aged 35 to 44** against the account's 44.6%. Destination `https://www.healthformoms.co/save/`.

The opening frame is aspirational and quiet: a stylish mom in good clothes holds a young boy's hand and walks in front of a modern house with a large black door, the same POV husband text hook running across the frame with a different heart emoji. Like moms-63 3e, it says nothing for a long time. At **0:10** a woman's voice arrives with the best single line in this batch: *"When did family health deductibles start looking like a down payment on a car?"* She keeps going without waiting for an answer: *"Seriously though, we pay this huge monthly bill, but the second one of our kids needs urgent care, I'm still swiping my card for thousands of dollars before the plan actually pays a dime."* At 0:25 she lands it in two words, *"It's ridiculous,"* and at 0:26 turns to the solution, checking Health for Moms, the state qualifier, a private plan with a near-zero deductible and lower monthly payments. At 0:38, *"If your state is in the list on the screen, tap below,"* and a professional narrator closes at 0:45.

### Why this ad is worth iterating on

On the selection doc's primary test, spend trend in the context of the account, this is the clearest case in the report. `selecting-ads-to-iterate-on.md` walks through three account examples and in every one the ads chosen are the ones whose spend is increasing week over week, with the Brand C case specifically naming an ad "running for 7 days, spend doubled on 7-day basis" as a clear iterate-on candidate. moms-65 1a is that case with a bigger multiple: eight days old, spend up 482%, **and** cost per lead improving 27% over the same step. An ad that gets cheaper as Meta pushes more money into it is the account telling you it has found headroom, and the doc's high-riser section says that when you see this pattern you should immediately be looking for ways to iterate on it.

It also passes the account-trends read the doc asks for before any iteration is made. Among the common traits of this account's top performers, this one shares the proven text hook, the produced-lifestyle format and the mother-and-child-outdoors visual grammar. Where it diverges is the thing worth extending: it is reaching a different audience than the rest of the account. **63.0% Instagram against 38.8% account-wide**, and a heavier 35-to-44 skew. Read through `ad-account-analysis.md`, heavy Instagram delivery signals a younger, more visually driven audience sitting higher in the funnel, which means this file is doing incremental reach rather than re-serving the same pool the incumbent has been hitting since April. That is exactly the "unlock new audiences" goal `iterations.md` names as one of the two strategic reasons any iteration exists.

The bottlenecks are two and they are related. First, the same silent runway: **the first spoken word lands at 0:10** and average play time is **3.41 seconds**, the shortest of any riser. The car-payment line, which is a genuinely strong Comparison Hook by the taxonomy in `iterations.md`, is buried under ten seconds of music. Second, this is the **most expensive impression set of the four candidates at a $26.20 CPM**, and its hook rate of 32.69% is the lowest of the risers, only just clear of the 30% floor. Those two facts fit together: a weaker first frame gets a worse auction price. The working elements to protect are the trajectory, the Instagram reach and the spoken script, which is the sharpest writing in the account. The element to iterate is the first ten seconds.

### Iteration history

**This file has never been iterated on directly.** It is itself round three of the POV husband program described in the moms-63 3e entry. But like moms-53 3, it launched inside a batch, and the batch history changes what to recommend. *Verified* from a name-scoped lifetime pull run 2026-09-04.

1. **2026-08-27 — the Moms65 drop, eleven files.** moms-65 1a took **$1,283.97 of the batch's $1,375.03, which is 93.4%.** The remaining ten split about $91.
2. **moms-65 1e, $7.24, and moms-65 1b, $4.45.** Both carry the **identical verbal hook** to the winner, *"When did family health deductibles start looking like a down payment on a car?"*, on completely different footage: a woman folding baby clothes on a bed with a tweet overlay, and a woman in a bedroom beside a large grey teddy bear. So the account has already built the version of this ad where the strong line opens the file, and it has never been given enough budget to find out whether it works. That is the single cheapest test available in this report, because the asset already exists.
3. **moms-65 1c, $46.13 for 3 leads at $15.38.** A different angle entirely, a close-up to camera opening *"I'm getting an MRI and the price if I use insurance is $4600."* The best cost per lead in the batch on far too little spend to call, and a cash-price comparison angle the account has never run at scale.
4. **moms-65 2a, $14.07, and 2b, $5.70.** A tattooed mother on a nursery floor holding a Paw Patrol book, and a similar domestic setting with Hello Kitty books, both on the deductible-anger script. This is the relatable end of the casting axis and it has never been tested.
5. **moms-65 2f, $6.55, and 2d, $2.78.** A kitchen-set outrage piece and the monkey-bars crying opener, both starved.

The pattern is identical to the Moms53 drop, three weeks apart, in a different ad set.

### Recommended iterations

**Cold Open on the car-payment line, using the footage that already exists.** This is Cold Open from the Video: Pacing menu, and it is the highest-confidence, lowest-effort recommendation in this entire report because **no production is required**. moms-65 1e already opens on that exact spoken line over different footage and has $7.24 of delivery. Two moves: relaunch 1e into its own ad set with real budget, and separately recut 1a so the 0:10 line becomes 0:00 over the walking footage, cutting to the existing 0:14 continuation, *"Seriously though, we pay this huge monthly bill..."*, at roughly 0:04. The transition is seamless because those two lines are already consecutive in the same take. The reason to do both rather than either is that they isolate different variables: one tests the line as an opener on new footage, the other tests it on the footage Meta has already chosen to spend on. **Success criterion for the 2026-09-18 report:** hook rate above 38% and average play time above 4.5 seconds at $1,500 or more of spend, with cost per lead at or under $22.

**Aspirational versus relatable creator, on the same script.** This is the Aspirational vs. Relatable Creator pattern from the Audience Iterations menu, which `iterations.md` describes as testing someone the audience wants to be against someone the audience sees themselves as. The evidence is not a hunch. The joint most-liked comment in this window reads *"I'm sure the mom that can afford matching outfits prob just pays in cash 🤦‍♀️"*, sitting under this casting family, and it is a mother saying the ad is not for someone like her. The stylish mom at the modern black door is the aspirational pole and the account has run it three times. The relatable pole exists already in the same batch, unspent: moms-65 2a, a tattooed mother sitting on a nursery floor among children's books. Reshoot the car-payment script with that creator in that setting, keep the text hook, keep the length. Per the optimization hierarchy in `iterations.md`, avatar is the last lever you pull, and this account has now exhausted angle and is starting on format, so the timing is right rather than premature. **Success criterion:** cost per lead at or under $21.85 at $1,500 or more of spend, and a Facebook share of delivery above 50%, which would tell us the relatable casting reached a different pool rather than the same one.

**Negative versus positive framing on the text hook.** This is the Negative vs. Positive Framing pattern from the Messaging Iterations menu, low effort, described as testing loss aversion against gain framing for the same fact. The current text hook is pure gain: you saved $400 and your husband is impressed. The spoken script directly underneath it is pure loss: you are swiping your card for thousands before the plan pays a dime. The ad is running two opposite psychological frames stacked on top of each other, and only the gain frame has ever been tested as a hook in this account. Write the loss version of the text hook in the creator's own words from the transcript, keep every frame of footage and every second of audio identical, and run it as its own file. This is the cheapest possible test of whether the account's most-used line is actually the right one. **Success criterion:** cost per lead at or under $21.85 and hook rate at or above 32.69% at $1,000 or more of spend. If loss framing matches gain framing on cost, the account has a second proven hook family for the first time since April.

---

## Moms43 - 4 - V3

### The ad

Media: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4`

Ad name **Moms43 - 4 - V3**, facebook_ad_id 120241073380060519, ad set Moms43 - 4 (State Moment), campaign USHA - ABO - SCALE - MOMS, the only ad in this report living in the scale campaign. Launched **2026-04-15**, so **142 days running**. Over the fortnight it took **$6,772.85** for **212 leads at a $31.95 cost per lead**, which is **27.5% of the account's clean spend** and the largest single line item by some distance. Hook rate **45.97%**, hold rate 3.59%, CTR 1.84%, CPM **$26.05**, cost per link click $2.65. Lifetime it has taken **$55,794.26 for 2,549 leads at a $21.89 cost per lead**, on a lifetime hook rate of 45.76%, a lifetime hold rate of 3.81% and a lifetime CPM of **$21.63**. Week over week spend fell 12.2%, from $3,606.71 to $3,166.14. No landing_url is returned; the working destination is inferred from an 88.1% landing rate.

The ad opens on stillness. A mother and her baby lie together in bed, white bedding, soft beige light, both looking calmly into the camera, and a woman sings gently over the top: *"These memories will stay with me."* The POV husband text hook sits across the frame. Nothing else happens. The singing runs, the shot holds, and the first spoken word of the argument does not arrive until **0:18**, when a different voice cuts in with, *"Listen, this is why you can't simply just say, 'Oh, I have insurance, I'm covered.'"* At 0:23, *"No. You need health insurance that has a zero dollar deductible without spending thousands."* At 0:28 comes the qualifier, *"And you can only get that if you are a mom and you live in one of these states,"* and from 0:35 the close: click below, use this new website, better rates, thirty seconds. A female voiceover ends it at 0:46 with *"Finally, insurance that actually feels like it has our back."*

### Why this ad is worth iterating on, and the test it fails

Be straight about this one. **On the selection doc's primary test, this ad does not qualify.** `selecting-ads-to-iterate-on.md` is explicit across all three of its worked examples that the ads you choose are the ones whose spend is climbing, and it says of the Brand A case that an ad "maintaining fairly high spend levels" but "dropping in spend WoW" should not be prioritised, whether the cause is fatigue or seasonality. This ad's spend fell 12.2% week over week and its cost per lead is the worst of any big spender in the account. By the letter of the doc, it is the ad you leave alone.

It is in this report on the doc's two other criteria, and the case has to be made rather than assumed. The first is **spend volume in the context of the whole account**, which the doc names as one of the two absolute precursors. At **27.5% of clean spend** this is where more than a quarter of the brand's money currently goes, and the brand's stated objective is efficiency before volume. An account cannot fix its cost per lead while ignoring its biggest line item. The second is **run time read against factual performance**, which the doc frames memorably: an ad running a long time on flat contribution is like an employee doing the bare minimum for ten years, and you would not promote it. At 142 days this is by far the oldest thing carrying real budget.

What makes it an iteration target rather than a kill is the specific shape of the decline, and the shape says the creative is not the problem. **Hook rate is essentially unchanged**, 45.97% over the fortnight against 45.76% lifetime, so the first frame still stops exactly as many people as it ever did. Hold rate is also unchanged at 3.59% against 3.81% lifetime. What moved is price: **CPM is $26.05 against a lifetime $21.63, up 20.4%**, and cost per lead is $31.95 against a lifetime $21.89, up 46%. That is the pattern `ad-account-analysis.md` describes when it says a rising CPM means you are paying more to reach the same pool, and the pattern `iterations.md` labels plainly: "CPA rising over time: this is typically audience fatigue. The same people are seeing the same creative too many times. You need fresh elements like new creator archetypes, format changes, or messaging angles to reach new pockets of audience." Frequency would confirm it and this account does not return frequency, so this stays **inferred**. But the trajectory over five months is hard to read any other way: this hook produced a **$6.58 cost per lead in March** on its original footage, **$21.55 lifetime** on this file, and **$31.95 in the last fortnight**. The words are not tired. The picture is, and the audience that likes that picture has been fully bought.

### Iteration history

This is the most-iterated asset in the account, four rounds across five months, and its history is the strongest evidence in this report. *Verified* from a text-hook family pull returning twelve named ads carrying this exact line, $86,135.90 of lifetime spend and 4,357 leads at a blended $19.77. The outcomes are *inferred* from spend and cost per lead, because no decision log exists.

1. **2026-03-18 — the originals, and the cheapest leads this hook ever bought.** MOMS37 - 12 - V5 at $558.90 and a **$6.58 cost per lead**, MOMS37 - 13 - V5 at $562.42 and a **$7.50 cost per lead**, both on one shared video file of a mother in bed with her baby. Both now in a paused ad set. Nobody appears to have asked why the cheapest version was retired.
2. **2026-04-06, relaunched 2026-04-15 — round one, three variants, same footage.** V1 at $12,153.59 and $21.32, V2 at $1,852.41 and **$14.59**, V3 at $57,506.21 and $21.55. V1 and V2 now paused. **Outcome: the round changed the text and the edit but not the picture, and all three converged around $21, roughly triple the March cost.** V2 had the best cost per lead in the round and received three percent of the round's budget. Read against `andromeda-v2.md`, three variants sharing one visual composition in the first three seconds is the textbook case of a false differentiator, and the flat results across the three are what that looks like in a report.
3. **2026-08-14 — round two, new footage, same words.** moms-63 2b at **$13.26**, moms-63 3e at **$15.46**, moms-63 1e at $0.03 and two impressions. **Outcome: both files that got delivery cut the cost per lead by $6 to $8 against the incumbent running the identical text in the same month.**
4. **2026-08-27 — round three.** moms-65 1a at $21.40 and improving, covered above. **Outcome: still scaling.**
5. **2026-09-03 — round four, in flight.** moms62, eight files, $17.30 on three days. Too young.
6. **2026-08-31 and 2026-09-02 — destination duplicates, not iterations.** Copies of rounds two's winners re-pointed at the broken and the untested destinations, $865.39 and $537.23 at $144.23 and $67.15 per lead. Unscored.

Four rounds, one lesson, repeated twice: **changing the words did nothing and changing the picture worked both times it was tried.** No round has ever changed the format. No round has ever touched the eighteen silent seconds.

### Recommended iterations

**Cold Open — cut the eighteen-second musical intro.** Cold Open from the Video: Pacing menu. This is the most extreme version of the problem that runs through this whole report and it is worth stating as a number: average play time on this ad is **4.20 seconds** and the first word of the argument arrives at **0:18**, while only 10.08% of its three-second viewers reach the quarter mark and 2.60% reach the halfway mark. Read between those two points, well over ninety percent of the people who stop for this ad never hear a single word of what it is selling. They see a mother, a baby and a promise about $400, and they leave. Cut straight to the 0:18 line, *"Listen, this is why you can't simply just say, 'Oh, I have insurance, I'm covered,'"* keep the bed footage under it as b-roll, and keep the sung line as a two-second cold open rather than an eighteen-second one. The body from 0:23 onward runs untouched. Given the ad's spend level, `iterations.md` warns that large-spend ads usually need bigger swings than small tweaks, which is why this sits alongside the format change below rather than standing alone. **Success criterion for the 2026-09-18 report:** hold rate above 6.0% and cost per lead at or under $25.00 at $3,000 or more of spend.

**Format swap — build this message as a static.** Video to Static from the Format Iterations menu, and the format lever is the top rung of both the signal-change ladder in `iterations.md` and the differentiation hierarchy in `andromeda-v2.md`. Three arguments converge on it. This asset has had four rounds of iteration and not one of them changed the format, so the loudest available lever is untouched. The audience for this visual is priced up, and format is the change most likely to buy genuinely new reach rather than the same pool at a higher CPM. And the account has direct evidence that statics work for it: per `marketing-calendar-and-campaigns.md` the SAMAR static era from 2025-07-17 ran 87 ads for $75,890.55 at a **$12.34 cost per lead**, the cheapest era in the account's history, with a workhorse static headlined *"Didn't know I could ditch my job's health plan… until I did."* The account walked away from its cheapest format and has not tested one since. Do not compress this video into a card. Take the one claim that has carried $86,135.90 of spend, the $400 saving with a zero deductible, and build it as a first-person testimonial card in the SAMAR register. **Success criterion:** a static from this concept clearing a **$22.00 cost per lead on 100 or more leads**, which would beat the incumbent video's lifetime figure and settle whether the format is worth a real round.

**Frankenstein stitch — the state-list opener onto this body.** This is the Frankenstein stitching pattern, which `iterations.md` lists among its historically highest-confidence iterations and calls one of the lowest-risk moves available, because every component has already been validated on its own. The account has two separately proven assets that have never met. The state-list screen from moms-53 3 is producing the best CTR and the cheapest clicks in the account at $0.97. The body of Moms43 - 4 - V3 has converted 2,549 leads over five months. Take the first three seconds of moms-53 3, the woman in the grey tank in front of the wall of state names saying *"I'm so thankful for the mom that told me about this,"* and cut at 0:03 into this ad's 0:18 line, *"Listen, this is why you can't simply just say, 'Oh, I have insurance, I'm covered.'"* The stitch flows because both are direct address and the second line reads as her continuing the recommendation, and the energy matches: neither is high-production and neither is emotionally heightened. It also does the pre-qualification job in the first frame, which is the other thing this ad needs. Per `andromeda-v2.md` this is a genuinely different first three seconds, so Meta should treat it as new rather than grouping it with the incumbent. **Success criterion:** cost per lead at or under $22.00 at $2,000 or more of spend, plus a CTR above 2.5% to confirm the state opener carried its click behaviour across.

---

## Open loops

**1. Three separate drops, three weeks apart, and each one funded a single file.**
The Moms53 drop of 2026-08-25 put seven files up at one timestamp and moms-53 3 took 99.75% of the batch's spend. The Moms65 drop of 2026-08-27 put eleven up and moms-65 1a took 93.4%. The moms 68 drop of 2026-08-31 put fifteen up and the whole batch drew $4.23 across 163 impressions. In every case the starved files include real creative bets on angles the account has never tested at scale, like the $4,600 MRI cash-price comparison at a $15.38 cost per lead on $46.13.
*Pull: Pattern.* The same winner-takes-all split showed up in three independent drops inside seven days of each other, which stopped looking like chance somewhere around the second one.
**Question: What would it take for a second file in one of this account's drops to get a fair test?**
The whole iteration program in this report assumes a recommended variant will actually receive delivery. If batches keep collapsing onto one file within hours, then every recommendation here produces one test rather than three, and the constraint on this brand's learning rate is the ad-set structure rather than the creative.
*Territory: Messaging.*

**2. The words have been iterated four times and the format has never been iterated once.**
Across five months this account has run four rounds on its most-used text hook. Two rounds changed the copy and the edit and landed within a few dollars of each other. Two rounds changed the footage and both cut the cost per lead by six to eight dollars. Nothing has ever changed the format. Meanwhile the cheapest era in the account's history, at a $12.34 cost per lead, was a static era that ended in the winter and has never been revisited.
*Pull: Gap.* The lever the method docs and this account's own history both point at hardest is the one lever nobody has pulled.
**Question: What happens to this account's cost per lead when its proven message runs as a static?**
If statics land anywhere near their 2025 numbers, the September and October rounds should be rebalanced toward them before Open Enrollment rather than after it, and the production bottlenecks the brand named in casting and scripting matter far less than they currently seem to.
*Territory: Messaging.*

**3. Every ad in this report keeps its argument behind a wall of silence.**
The first spoken word lands at 0:11 on moms-63 3e, 0:10 on moms-65 1a and 0:18 on Moms43 - 4 - V3. Average play times are 4.03, 3.41 and 4.20 seconds. The one file that opens talking, moms-53 3, has the account's best deep retention by a factor of nine and its cheapest clicks. That is four data points pointing the same way and not one of them was designed as a test.
*Pull: Surprise.* An account whose whole diagnosis is that it cannot hold anyone has been opening its biggest ads with ten to eighteen seconds of music.
**Question: How much of this account's hold-rate problem is the creative and how much is just the silence at the front?**
If the silent runway is the cause, the fix costs nothing and applies to the entire library at once, which would be the cheapest performance gain available to this brand before November.
*Territory: Messaging.*

**4. Nobody knows what a lead from a $16 ad is worth against a lead from a $32 ad.**
The four ads in this report range from a $16.39 cost per lead to a $31.95 one, and every recommendation above is written to move spend from the expensive end toward the cheap end. Parker can see the cost of all 712 leads in this window and can see nothing about any of them after the handoff.
*Pull: Gap.* There is a two-times spread in cost sitting in plain view and the single piece of information that would say whether it is a real spread lives entirely outside Meta.
**Question: How do the leads from the August creative compare with the leads from the April creative once the partner agencies have worked them?**
This is gate two on every recommendation in this report. Without it the whole iteration program rests on half of the brand's own definition of a winner. **This one only the brand can answer.**
*Territory: Product.*

## Appendix - Parker media links

Every ad discussed in the body, indexed so a strategist can reopen the media without searching. Links and paths preserved exactly as returned by the Parker MCP.

**M001: moms-63 3e.** Selected for iteration. $5,093.33 over the fortnight for 309 leads at $16.48, 42.87% hook rate, $18.77 CPM. The POV husband line over outdoor mother-and-son footage, first spoken word at 0:11. Created 2026-08-14.
Facebook ad id: 120247093478820519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4
Landing page: https://www.healthformoms.co/save/

**M002: moms-53 3.** Selected for iteration. $2,097.43 for 128 leads at $16.39, a 3.13% CTR and a $0.97 cost per link click, both best in the account, and 6.65% completion. The "Approved State List ✔️" opener. Created 2026-08-25.
Facebook ad id: 120247254787160519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4
Landing page: https://www.healthformoms.co/save/

**M003: moms-65 1a.** Selected for iteration. $1,376.63 for 63 leads at $21.85, spend up 482% with cost per lead improving from $28.85. Stylish mom at a modern black door, car-payment line at 0:10. Created 2026-08-27.
Facebook ad id: 120247285907980519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247285907980519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/bb071de9e8d0e46ca498a10528b066d07bf324999cb3e1b0d11d83c83592cc67.mp4
Landing page: https://www.healthformoms.co/save/

**M004: Moms43 - 4 - V3.** Selected for iteration. $6,772.85 for 212 leads at $31.95 over the fortnight against $55,794.26 lifetime at $21.89. 142 days running, hook rate flat, CPM up 20.4%. Mother and baby on white bedding, sung intro, first spoken word at 0:18. Created 2026-04-15. No landing_url returned; working destination inferred from an 88.1% landing rate.
Facebook ad id: 120241073380060519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

**M005: moms-63 2b.** Iteration history, round two. $5,529.30 lifetime at a $13.26 cost per lead, the cheapest lead the POV hook has produced since March. Sibling of M001. Created 2026-08-14.
Facebook ad id: 120247093361410519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
Landing page: https://www.healthformoms.co/save/

**M006: MOMS37 - 13 - V5.** Iteration history, the original. Created 2026-03-18, $562.42 at a $7.50 cost per lead, 49.87% hook rate. Mother in bed with baby, the first file to carry the POV husband text hook.
Facebook ad id: 120239743452890519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239743452890519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0219cba7b09365039fa6d105f8ed805a7486783dffa637b03135c3c96d56fbd9.mp4
Landing page: https://www.healthformoms.co/save/

**M007: MOMS37 - 12 - V5.** Iteration history, the original's twin on the same video file. Created 2026-03-18, $558.90 at a **$6.58 cost per lead**, the cheapest this hook has ever been.
Facebook ad id: 120239743397990519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239743397990519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0219cba7b09365039fa6d105f8ed805a7486783dffa637b03135c3c96d56fbd9.mp4
Landing page: https://www.healthformoms.co/save/

**M008: Moms43 - 4 - V2.** Iteration history, round one. Created 2026-04-06, $1,852.41 at a **$14.59 cost per lead**, the best in its round and now paused on three percent of the round's budget. Same bed footage as M004.
Facebook ad id: 120241073380070519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380070519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/3212df8ea94c10b250d5e8bf953eb9390c5c8d2760b843b70544a0809c2b06d5.mp4

**M009: Moms43 - 4 - V1.** Iteration history, round one. Created 2026-04-06, $12,153.59 at $21.32, now paused.
Facebook ad id: 120241073380110519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380110519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/f18c5a15a13e4412e35f654034f63f147ca73e40b35538419d22500d143b670d.mp4

**M010: moms-65 1e.** Iteration history, and the ready-made asset behind the first moms-65 recommendation. Created 2026-08-27, **$7.24 total**. Opens on the spoken line "When did family health deductibles start looking like a down payment on a car?" over a woman folding baby clothes with a tweet overlay. Never tested.
Facebook ad id: 120247286043630519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247286043630519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/3c4d9062e9f2b9db931824df3769448d036a275e02185cb57295ee32dc33b479.mp4
Landing page: https://www.healthformoms.co/save/

**M011: moms-65 2a.** Iteration history, and the relatable-casting asset behind the second moms-65 recommendation. Created 2026-08-27, $14.07. A tattooed mother sitting on a nursery floor among children's books holding a Paw Patrol book. Never tested.
Facebook ad id: 120247286221890519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247286221890519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/a5ca131fbd3583ed0b83710ee9fe04492d44f415fadaba9e9bc2af3bb98929cc.mp4
Landing page: https://www.healthformoms.co/save/

**M012: moms-65 1c.** Iteration history, and the starved angle named in open loop 1. Created 2026-08-27, $46.13 for 3 leads at $15.38. Opens "I'm getting an MRI and the price if I use insurance is $4600." The cash-price comparison angle, never run at scale.
Facebook ad id: 120247286033490519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247286033490519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e8dacd6894b005061a1465804ff64b8de78c0951ba1491738780d9afe0bbd5ba.mp4
Landing page: https://www.healthformoms.co/save/

**M013: moms-53 4.** Iteration history. Created 2026-08-25, **$0.33**. Carries the identical verbal hook to M002, "I'm so thankful for the mom that told me about this," on a different creator and setting. The creator reshoot that never got delivery.
Facebook ad id: 120247254790580519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254790580519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1f3734eb32be5ab50d05d9c0b6e4c7bef37c069276817d0c4e36c7efd532a6a3.mp4
Landing page: https://www.healthformoms.co/save/

**M014: moms-53 1.** Iteration history. Created 2026-08-25, **$0.12**. Same verbal hook again, a woman in a tie-dye tank in a bedroom, text hook "2026 health insurance hack for moms."
Facebook ad id: 120247254735370519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254735370519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/001844f832ea96737713810b8b9a4b9086aeec8061cf87a415e830196b78e070.mp4
Landing page: https://www.healthformoms.co/save/

**M015: moms-53 5.** Iteration history. Created 2026-08-25, $2.06. A split-screen reaction format, black-and-white reaction face over a woman venting, under "Health Insurance is a scam 🙄 $6,000." The only split-screen vehicle in the drop, untested.
Facebook ad id: 120247254793290519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254793290519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1f24bccea594c5e32b7748c684f40efa1c93d4c963b440171bf7eb37e26ffc04.mp4
Landing page: https://www.healthformoms.co/save/

**M016: moms-63 2b - Copy.** Iteration history, the destination duplicate. Created 2026-08-31, re-pointed 2026-09-02, $865.39 for 6 leads at $144.23 across the broken and quiz destinations. Unscored, named to keep it out of the creative read.
Facebook ad id: 120247373812970519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247373812970519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
Landing page: https://quiz.healthformoms.com/#/indvfam

**M017: moms 68 1#.** Named in the intro as the batch that cannot be iterated on because it was never tested. Created 2026-08-31, $0.85 and 32 impressions. The satirical skit format, woman in a black leather jacket, "This is why health insurance in America is a scam..."
Facebook ad id: 120247340952300519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247340952300519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/7aa5cf3b3cd5d470e40e939f3ab051cd97d6c2ae5d4dcac6ca317f9fe5dda470.mp4
Landing page: https://www.healthformoms.co/save/

**M018: moms55-1.** Named in the intro among the ads not selected. $704.90 for 31 leads at $22.74 on seven days. Woman in orange-tinted sunglasses doing insurance math in the school pickup line. Created 2026-08-28.
Facebook ad id: 120247304910390519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247304910390519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b3ef51c46ea047450eeba20ec707c5b9022d136aa15f90b609da424269526a11.mp4
Landing page: https://www.healthformoms.co/save/

**M019: B1 samar- Copy.** The static-era reference behind the Video to Static recommendations, carried forward from `marketing-calendar-and-campaigns.md`. Created 2025-07-17, $35,219.98 lifetime for 3,046 leads at an **$11.56 cost per lead**. Headline "Didn't know I could ditch my job's health plan… until I did."
Facebook ad id: 120227092765930519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227092765930519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b219b0aa7f7e7ed8d83fa471803f4b6c96ad98b2de118b2a8e68038439e759a9.jpg
Landing page: https://www.healthformoms.co/save/

**Funnel destinations appearing in this window**

- https://www.healthformoms.co/save/
- https://go.healthformoms.co/save/
- https://quiz.healthformoms.com/#/indvfam
- https://quiz.healthformoms.com/2

---

**Brand Context Applied:**

- **What I used:** The brand's two-gate winner definition and its verbatim intake line that cost per lead matters for scale but lead quality is checked before really scaling, so nothing here is called a winner. Its own cost-per-lead tiers, under $15 fantastic through over $25 not good, as the bar every figure is graded against. Its stated best angle, the state mechanic, verbatim as *"State angle has worked very well if you see the account. Emotional and direct response."* Its own diagnosis of low creative diversity. Its stated production capacity of one to five net-new concepts and one to five iterations a month, which is why each entry carries three or four recommendations rather than ten. Its Open Enrollment date of November 1 with a two-month planning lead, now 58 days out. The live Meta account for every number, and the 25 Facebook ad comments from this window as the only voice-of-customer surface this brand has.
- **What I avoided:** ROAS, AOV, purchase value and add-to-cart appear nowhere, per the standing rule for this lead-generation account with zero purchase events. No ad is called a winner on cost per lead alone. No lead-quality claim is made anywhere, because Parker cannot see it. No specific metric improvement is predicted for any iteration; every recommendation names the bottleneck it targets and the criterion that would judge it, never an expected lift. No political or partisan framing was recommended, per the brand's stated guardrail. And no recommendation repeats a variant the account has already tried and starved, which is why the creator reshoot on moms-53 3 is written as a delivery fix rather than as a fresh file.
- **Why this fits:** The account is 58 days from the single most important date on its calendar, with a proven message, almost no format variety, and five months of its own evidence that changing the picture works and changing the words does not. These four ads carry 62.2% of the clean spend, so they are where a cost-per-lead fix actually moves the account. The recommendations aim the next fortnight at the three things the account has never tried on its best assets: opening with words instead of music, running the proven message as a static, and giving a second file in a drop enough budget to be tested at all.

This is based on everything I know about choosing which ads to iterate on.

This is based on everything I have learned about making iterations 2.0.

This is everything I know about Andromeda v2.
