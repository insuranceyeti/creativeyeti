---
brand: health-for-moms
doc: customer-journey-and-persona-discovery
generated_on: 2026-09-03
refresh_by: 2027-03-02
quarter: Q3 2026, reflecting creative live through 2026-09-03 and comments posted 2025-01-08 through 2026-09-03
sources:
  - "Facebook and Instagram ad comments, Meta ad account HealthForMoms, act 484897827497337, via Parker MCP `search_facebook_ad_comments_sql` and `search_facebook_ad_comments_semantic`. Corpus is 1,322 comments, 100% of what Parker holds, on 112 ad ids and 79 ad names, dated 2025-01-08 to 2026-09-03. Eleven substring counts and four semantic sweeps were run fresh for this doc."
  - "Meta ad account `HealthForMoms`, act 484897827497337, via Parker MCP `search_facebook_ads_sql`. Lifetime cut across 1,557 ad-name groups, $743,218.09 spend, 39,569 leads, $18.78 CPL. Full scripts pulled fresh on the referral family and on the family that names the viewer's hesitation out loud."
  - "`source-pulls/ad-account.md`, the completed persona source pull, 2026-09-03. 13 ads read at full media depth with transcript, creative analysis, creator demographic and per-ad delivery. Used here as the full-media read behind creative claims."
  - "`source-pulls/ad-comments.md`, the completed comment source pull, 2026-09-03. All 1,322 comments read, full creative read on the 20 ads carrying 997 of them."
  - "Brand context document via Parker MCP `get_brand_persona`, sections 1 through 6 and 12 through 14, read in full for the brand's stated journey, tipping points, entry points, objections and customer language."
  - "Parker TikTok mining library via `search_tiktok_videos`. 23 videos, 19 scored Relevant. Five read at full report depth including transcript, creator description and hook analysis."
  - "Parker chat history via `search_chat_history`. Four threads, one web and three Slack, all dated 2026-09-03. Two Slack threads read in full for what the team said about its own buyer."
  - "`running-notes/missing-context.md`, `running-notes/brand-rules.md`, `running-notes/success-definition.md`, Phase 0, 2026-09-03."
substitution_rule_applied: "Customer reviews are dark for this brand, confirmed again in this run with a live pull returning totalReviews 0. Per the team's own instruction in Slack on 2026-09-03, review evidence is substituted with Facebook ad comments, the category TikTok library and the brand context document, and every substituted source is labelled where it is used. Nothing here is presented as this brand's own review corpus."
data_limitations:
  - "No customer reviews. A live `search_customer_reviews_sql` pull on 2026-09-03 returned totalReviews 0. There is no first-party buyer source of any kind for this brand, which under the persona method caps every identity read here at thin to mixed and means no journey claim can be checked against a confirmed buyer."
  - "No post-purchase surveys. Zero responses, no survey platform connected, confirmed in Phase 0. This is the single strongest journey source the method names and it does not exist here."
  - "No purchase event exists in the account. There is no revenue, no ROAS, no AOV and no purchase value, and none is reported anywhere in this doc. Every efficiency figure is CPL and lead volume, per `running-notes/brand-rules.md`."
  - "Lead quality is invisible to Parker. The real second gate on a winner lives with the partner agencies. Every CPL here is the cost of a phone number, not the cost of a customer."
  - "The brand's own website could not be read. `https://www.healthformoms.co/save/` was blocked by the network egress proxy in this run, so the FAQ comparison this prompt asks for is built from the brand context document's stated objection list rather than from the live FAQ page. This is a run gap, not a finding."
  - "Comment authorship is unreadable. `author_name` and `permalink_url` are null on all 1,322 rows, so every count is a count of comments and never a count of people, and no commenter can be traced to a lead."
  - "The comment corpus is skewed. Roughly 60% of it sits on the `MOMS38 - 1` family and 38% was posted in April 2026, so every rate quoted is a rate inside that skew."
  - "No competitor ad library is tracked in the Parker app, so no category baseline exists for any of these rates."
  - "The TikTok library is a curated mining set built from insurance keywords, not a random sample of the category. It shows what the category talks about, not how often."
  - "Northbeam is not connected. All attribution is Meta-reported on the org default window."
---

# Customer journey and persona discovery — Health For Moms

## How buying actually happens here

Nobody buys anything from Health For Moms. That is the first thing to hold, because every field below reads differently once you do.

This is a matching business. The brand's own context document describes a three-step service: answer a few questions, speak with a partner agent who is "like your Mom BFFs - friendly and approachable," get a better plan. That is `stated`. What the account shows is `verified`: 39,569 leads and zero purchases across $743,218.09 of lifetime spend, pulled fresh on 2026-09-03. So the thing the creative sells is not a health plan. It is a thirty-second qualification check, paid for with a phone number.

That splits the journey into two halves, and Parker can only see one of them.

The first half is fast, cheap and almost entirely curiosity. Every funded script in the account runs the same shape. Name the money pain, promise a $0 deductible, put a full-screen list of 32 to 34 approved states on the screen so she stops and hunts for hers, then say it takes thirty seconds. `moms-53 3`, pulled in full for this doc, is four lines long: "I'm so thankful for the mom that told me about this," then the state gate, then "It takes you 30 seconds, it's a brand new website," then "fill it out and see if you qualify." That is not a considered purchase. It is a scratch-off ticket with a state list on it.

The second half is the opposite. It is a phone call with a licensed agent about a medically underwritten private plan for a family, and it is a slow, high-distrust, high-stakes decision that can be killed by a pre-existing condition, a pregnancy, a state, or a price nobody has named yet. Parker cannot see one minute of it. The account's own `invitee_meeting_scheduled` conversion returned no data at all in the 90-day window, and only 42 `Call` events fired against 4,336 leads, per `source-pulls/ad-account.md`.

**The read, marked `inferred`, confidence strong:** the creative's job here is not to make her want insurance. She already wants it and mostly already has it. The job is to make handing over a phone number feel safe and cheap enough to be worth doing on a scroll. That reframes what a barrier even is for this brand. The barrier is not belief in the product, because there is no product on screen. The barrier is what she thinks happens next, and the loudest single voice in 1,322 comments is a woman telling other women what happened to her phone number.

Read against the TEEP model in `emotional-delivery-and-timing.md`, the account has a mismatch it is paying for. The funded creative is written for **Evaluation**, the phase where she is resolving one specific objection and deciding. "You may qualify," "worst case, you check and stick with what you have," "click below and see what you qualify for." But the audience answering in the comments is sitting hard in **Trigger**, the phase where a need has just become conscious and she is still making sense of it. She does not answer the offer. She answers the number. Someone says her deductible is $6,000 and 160 comments across 17 ads come back with their own figure, the highest-liked being "This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family. It's insane," posted 2026-03-22 with 47 likes. That is a woman processing a feeling, not comparing plans.

There is one funded ad in the account written for the phase she is actually in, and it is the newest and among the cheapest. `moms-63 3e`, created 2026-08-14, opens with "I almost scrolled past this because I thought, 'I already have health insurance, this doesn't apply to me,'" and closes with "Worst case, you check and stick with what you have. Best case, you realize you've been paying way more than you needed to." It has spent $5,240.28 for 339 leads at a **$15.46 CPL** against a $22.67 account average for the 90-day window. One ad is not proof. It is the strongest single piece of evidence in this doc that naming the hesitation out loud beats adding pressure, which is exactly what the emotional delivery method predicts for Evaluation-phase creative.

A caution to carry into everything below, from `persona-research-and-creative-strategy-process.md`: a low CPL means the phone number was cheap. It does not mean the woman on the other end answers the phone. Under this brand's own two-gate definition of a winner, every ad named here has passed gate one and none of them has been tested against gate two.

## Shape of the journey

**The single call, marked `inferred`, confidence strong.** The click takes almost no thought and the purchase behind it takes a great deal, and the account is built almost entirely for the click. What the creative has to do is win a two-second qualification scan and then survive a trust check she runs somewhere the brand does not control.

Here is the walk that produced that call. I ranked the account by lifetime spend and read the funded creative, then I read all 1,322 comments' worth of behavior through the fresh counts I ran for this doc, then I checked both against what the brand says its journey looks like. Three things lined up and one broke.

**What lined up.** The funnel is short by construction. The brand's context document says what converts skeptics is "Low friction. 'Just answer a few questions' — no commitment, no credit card, no long form," which is `stated`. The scripts say the same thing in the same words, "It takes you 30 seconds," which is `verified` across every transcript in `source-pulls/ad-account.md` and both scripts I pulled fresh. And the delivery matches a scroll-speed decision: 99.3% of lifetime spend lands on mobile.

**What broke.** A short funnel is not the same as a short journey. Between the form and any actual coverage sits a medical underwriting screen, and the public evidence that women hit it is everywhere. 42 of 1,322 comments use the word "qualify," which is 3.2% of the corpus, and the shape of those comments is a journey ending, not starting. "Was so excited about this but as soon as i said diabetic i didnt qualify," posted 2025-07-07 on `B2 - 10TH JUNE - Copy 16`. "April Crawford I was told I don't qualify 🤷," posted 2026-04-02 on `MOMS38 - 1 - V1`. "I took the short survey twice and slightly changed up my answers and it still didn't work out for me. Bummer," posted 2026-09-01 on `Moms43 - 4 - V3`, two days before this doc was written.

So the honest shape is a funnel that is thirty seconds wide at the top and has a hard gate a few clicks in, and a large share of the women the ads recruit meet the gate rather than the offer. How large is the one number nobody outside the brand can produce. It is an open loop below.

**Where the journey differs by buyer state.** The sources show at least five paths, and they do not need the same creative. Each is marked with what it rests on.

**One. The insured mom who suspects she is overpaying.** `inferred`, confidence strong, and this is the path 67.8% of the last 90 days of spend is built for, per `source-pulls/ad-account.md`. Her journey is genuinely short. She is not researching, she is reacting, and the movement she needs is small: permission to doubt a plan she already has. `moms-63 3e` names that movement in one line.

**Two. The mom whose employer picks her plan.** `inferred`, confidence mixed. She can be reached by the ad and cannot act on it, and she says so plainly. "Mine is $6k per person too but since it's thru my job I don't really have a choice," 2026-03-17 on `MOMS39 - 2 - V2`. "The hospital I work for only provides the option to use their insurance company. Last year it was over 18k," 2026-03-28 on `MOMS38 - 1 - V3`. Her journey has a step before all the others: learning that declining employer coverage is even allowed. In this corpus a stranger teaches her that, not the brand. "if it's an employer insurance, you don't have to sign up with that employer insurance you can decline the coverage and go out and find your own insurance carrier," 2026-05-05 on `MOMS38 - 1 - V2`.

**Three. The mom in the income gap with no plan at all.** `inferred`, confidence mixed, and this is a long, considered, months-long journey. She is the brand's stated Courtney profile, and one comment says it better than the profile does: "There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy," 2025-08-09 on `B1 samar- Copy`. The account gives this path about 0.14% of lifetime spend, per `source-pulls/ad-account.md`.

**Four. The chronic-condition family.** `inferred`, confidence strong on intensity and thin on volume. Her journey is the longest and most emotional in the corpus and it does not end at this product, because underwriting screens her out. 55 comments across 17 ads say so, and diabetes is named 11 times.

**Five. The mom leaving the category entirely.** `verified` across two independent surfaces, and the path this doc has read the least. She is not choosing between plans. She is choosing between insurance and no insurance. In the comments it looks like this: "I would rather have no insurance you would get better self-pay rates then you do with 'having coverage,'" 2026-03-26 on `MOMS38 - 1 - V2` with 14 likes. In the category TikTok library it is enormous. A doctor calling hospitals for cash prices on a delivery has 6.2 million plays, 661,800 likes and 208,000 shares. A former nurse explaining that her family of four has been uninsured for three years and joined a health-share group has 872,100 plays. A phone video panning down a hospital bill that went from $55,623.00 charged to $1,404.00 owed as a cash payer has 213,100 plays. That is the same argument the brand's own "Health Insurance is a scam" hook makes, and it ends somewhere else.

**What this demands of the creative, marked `inferred`.** One shape does not serve all five. The funded path needs a doubt and a thirty-second check. The captive needs permission. The mom who earns too much for help and too little to pay full price needs a comparison she can finish alone. The chronic-condition family needs the brand to stop recruiting a pain it cannot treat. And the defector needs a reason to stay in the category at all, which nothing in the account currently gives her.

## Where buyers come from

The prior behavior being replaced is the comparison the creative is actually fighting, and here it is not one thing.

**Replacing an employer plan is the dominant case.** `verified` from the creative, `inferred` on its share. Not one of the 13 scripts read at full media depth in `source-pulls/ad-account.md` asks whether the viewer has insurance. Every one assumes she does and reframes it as a bad deal. The comments confirm the audience arrives insured: 160 of 1,322 comments self-report their own deductible or premium, which is 12.1% of the corpus, counted across 17 different ads in `source-pulls/ad-comments.md`, and they are reporting on plans they hold today.

The account's cheapest evidence for this switch is a static from 2025 that nobody is talking about now. `B1 - Copy 7` carries the headline "Left my big insurance company for a mom-focused one. 24% cheaper and I choose my own doctor 😌" and ran $30,339.32 for 2,584 leads at an **$11.74 CPL**. That is a switching story told in the first person, in the customer's own frame, and it is the cheapest lead in the top ten lifetime spenders. It is not running now.

**Replacing nothing is the second case.** `inferred`, confidence mixed. The uninsured mom exists in the library and not in the budget. The 2025 video ending on "If you feel like you've fallen through the cracks, this is the bridge" received $67.51 of spend, and a static headlined "I'm a single mom, and I didn't know my insurance was failing us... 😭" ran a $15.07 CPL on $1,009.79 and is paused, both per `source-pulls/ad-account.md`.

**Replacing insurance with cash is the third, and it is the one the brand is not counting.** `verified` across ad comments and the category feed, as walked above. Two things make it matter more than its size. It is the direct competitor to the whole category, and the brand's own strongest hook argues its case for it. When your best-performing ad opens "Health Insurance is a scam 🙄" you have agreed with her out loud before you ask her to buy insurance.

**And the fourth case is not a switch at all.** The captive cannot switch, and the ad's premise assumes she can.

**What this means for the comparison the creative has to win, marked `inferred`.** The brand's context document frames the alternative set as marketplaces, employer plans and big carriers. That is `stated` and it is incomplete. In the public conversation this brand pays to create, the live alternatives are her employer's one option, doing nothing, and leaving insurance behind for cash pay and health shares. Rival agents work that last lane inside her comment section: 39 comments across 10 ads pitch a competing offer, including Direct Primary Care and health shares, per `source-pulls/ad-comments.md`.

## Discovery and word-of-mouth dynamics

**Paid social is the discovery channel. Not the main one. Effectively the only funded one.** `verified`. $743,218.09 of lifetime Meta spend against 39,569 leads, and the brand's own document names paid social as "the primary acquisition channel."

Then there is the thing that is not there.

**The brand's word-of-mouth story is a script, not an observed behavior.** This is the sharpest finding in the doc and it is built on an absence, so here is the full walk. The brand's context document names peer recommendation as a tipping point that "can collapse the decision timeline from weeks to minutes," and its own guidelines script the arc: "Then I found HealthforMoms" or "my neighbor told me about." The account acts on it. `moms-53 3` opens "I'm so thankful for the mom that told me about this," and a sibling POV line reads "POV: You shared Health for Moms in the group chat and now three friends have better insurance because of you. Legend behavior.💕"

So I went looking for it in the only unprompted surface this brand has. Across all 1,322 comments, the word "friend" appears in **3**, which is 0.23% of the corpus, and not one of the three is a referral to this brand. One is about flying to Colombia for cheaper dental care, one is about a friend medevaced from the Bahamas with a seven-figure bill, one reports a friend's $18,000 deductible. A semantic sweep for referral language, run at a 0.4 similarity floor against the full corpus, returned **zero results**. The word "recommend" appears in 5 comments, and three of those are "Not recommend" or "I DO NOT RECOMMEND."

`inferred`, confidence mixed. Mixed rather than strong because a comment section is a poor place to observe a private conversation, and because absence of evidence in one surface is weaker than presence. But the claim being tested is not "does anyone ever tell a friend." It is "is word of mouth a real acquisition channel for this brand today," and in fourteen months of the only public conversation the brand has, it leaves no trace at all.

**What happens instead of word of mouth is a peer verification hunt, and it happens in the comments.** This is the most useful discovery behavior in the doc, and it is `verified`, because I read the threads end to end.

On 2026-03-20, under `MOMS38 - 1 - V1`, a woman wrote: "Anyone actually have this and have insight?" It drew **15 likes and 6 replies**, which makes it one of the most-liked comments in the entire corpus. Here is what the thread answered her with, in order. "April Crawford wondering the same. I filled out something like this years ago- and got spam phone calls every 10 minutes for months!" "That's exactly what will happen here. Their website says they are a third party agency to connect you to agents. You'll get hundreds of calls and the plans aren't great." Then one genuinely positive answer: "I was connected to a very helpful agent. They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful." Then "April Crawford I was told I don't qualify 🤷" and "Jamie Abernethy Same."

It happened again five months later. "Has anyone had success with this?" on 2026-08-19 under `Moms43 - 4 - V3`, answered on 2026-09-01 with "I didn't. I took the short survey twice and slightly changed up my answers and it still didn't work out for me. Bummer."

`inferred`, confidence strong: the brand has no review page, no post-purchase survey, and a search result that invites doubt, so the verification step in this journey has relocated into the ad's own comment section, where strangers answer it and the brand does not. That is a discovery dynamic and a conversion barrier at the same time.

**How this connects to the brand's attribution gap.** Performance is read in Meta Ads Manager only, with no third-party attribution, per `running-notes/success-definition.md`. That is fine for a business whose discovery is one paid channel. It becomes a problem the moment word of mouth or search actually starts working, because neither would show up. There is one measurable leak worth naming now: ads pointing at the quiz destination show 903 link clicks against 234 landing page views on the `Moms Nahuel WV#1` group, per `source-pulls/ad-account.md`. That is a page or tracking fault sitting between the click and the form, and it inflates that group's CPL.

**No retail or shelf discovery exists.** This is a service. The field does not apply.

## Trigger events

These are moments, not people. Every one of them can sit on any of the five paths above, and the same woman can be triggered by several of them across years. They are ranked by how widely they recur across different ads in the comment corpus, since spread beats raw count.

**One. Finding out the number.** The most common trigger in the corpus and the one the account is built on. 160 comments across 17 ads disclose a deductible or premium unprompted. The state it produces is not shopping, it is grievance. "$6000???? Huh mine is $18000 .....where can I get the $6k," 2026-03-26. "6k....try 13k!" 2026-04-02. Confidence strong on recurrence, mixed on meaning, because a woman who quotes her deductible has not necessarily started looking for another one.

**Two. The deductible reset.** A calendar trigger that fires in December and January. "After my deductible, I pay 25% of all costs 'til I meet my max out of pocket, and then everything is finally taken care. And then it's the end of the year, and we start all over. I literally hate NYE for this reason!" 2026-04-04 on `MOMS38 - 1 - V3`, 6 likes. Confidence mixed, since the evidence for a seasonal spike is described rather than measured.

**Three. A procedure already on the calendar.** The highest-intent moment in the corpus. "This is what I'm afraid of. Just found out I desperately need a hysterectomy. My husband is looking into insurance for me so that I can get it done," 2026-04-14. "how can I get that because I pay $1000 a month for my insurance and tomorrow I have surgery," 2026-05-04. Small in volume, extreme in urgency, and worth naming because the second comment shows a husband running the search, which the brand's own document predicts.

**Four. The claim fight.** A denial or a two-hour phone call is what produces the only real recognition in this corpus, covered under what people love below.

**Five. A benefits change in the household.** The brand names this first among its tipping points. The comments carry it lightly: "I'm heading in to work so couldn't really look at this. And with bring a new rehiring I'm able to enroll into insurance. Not sure if I want to," 2026-04-30.

**Six. The bill that arrives after the emergency.** Strong in the category feed, present in the comments. The TikTok library's political ad from 2026-08-31 opens "My son started to have really bad headaches and then fainted. We ended up in the ER... And even with health insurance, these bills just keep coming."

**Seven. Open enrollment, and the lockout that precedes it.** The brand calls November 1 "the single most important date on the marketing calendar," which is `stated`. What the comments add is that the trigger fires in both directions: it also tells her to stop. "yes there is. You have to sign up during open enrollment, not whenever you need it," 2026-04-25. "Does this work in Louisiana? Because they wouldnt let me apply for good insurance here until November," 2026-05-27. There was no open enrollment creative in the 90-day window ending 2026-09-02, per `source-pulls/ad-account.md`, and the brand's own stated planning lead time is two months, which puts the start line at September 1.

**Not observed: peer recommendation as a trigger.** The brand names it as one of six tipping points. It does not appear in the corpus at all. See the discovery section.

## What has to happen before purchase

Two movements, and the account is good at one of them.

**Movement one: from "I already have insurance, this isn't for me" to "having insurance is not the same as having the right one."** This is the conversion movement the funded creative is actually built for, and the brand does it well. It is `verified` in the transcripts. `MOMS39 - 2 - V2` says it as a spoken line: "This is why you can't simply just say oh I have insurance I'm covered." `moms-63 3e` says it as a confession, which is stronger, because it lets her be the one who almost scrolled past. That ad's $15.46 CPL is the best evidence in the account that the confession beats the correction.

**Movement two: from "what happens to my phone number" to "this is safe."** The account does not make this movement anywhere I could find, and the evidence that it is required is the strongest single-comment evidence in the corpus.

The third-most-liked comment out of 1,322 is this, posted 2026-03-16 on `MOMS38 - 1 - V3` with **33 likes**: "Filled it out and have been getting calls everyday from all sorts of companies which are mostly India based. Also, the harassment from whomever keeps calling me about Medicare (India again). This is the ONLY form I've filled out since getting my new phone number 3 months ago so it came from this site!"

It is not alone, and the shape of it changed over time. In 2025 it is a report from someone who did it. "I filled this out because it literally says we won't be contacted by random agents. That's a lie. I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies," 2025-11-28. By 2026 it is fear from someone who has not. "I don't wanna put my information and get called by hundreds of people though..," 2026-03-11. "Really wish you could see plans without adding all your personal information to get even more telemarketing calls than we already do," 2026-03-13. Fifteen comments across ten ads carry this objection, per `source-pulls/ad-comments.md`, and my own count found four separate comments using the word "filled," three of which are complaints about what followed.

`inferred`, confidence strong on the barrier and thin on its cost, because nothing reachable connects a comment to a lost lead. But the logic is hard to argue with. The only thing the ad asks her to give is the exact thing the loudest voice in her comment section warns her about, and the brand's own promise of a pressure-free "Mom BFF" agent is being quoted back at it as a broken one.

**A third movement exists for the captive and it is pure information.** She has to learn she is allowed to leave. One stranger did that job in a reply. No ad does it.

**What the sources do not support:** an education arc about what insurance is, or a long trust-building sequence before the ask. The audience knows the category cold. Parker's own awareness tags put 56.2% of spend on Solution Aware and 37.1% on Problem Aware with essentially nothing Unaware, per `source-pulls/ad-account.md`, and 103 comments correct the ad's own use of the word deductible. Explaining the category to this audience would be doing the wrong thing well.

## Biggest myths

Myths exist here, and they are not the main blocker. Both parts of that sentence matter.

**Myth one, real and load-bearing: "I have insurance, so I'm covered."** A confidently held wrong belief, held by people paying premiums every month. The brand's own document names it: "Most think they're covered when they aren't." The winning scripts attack it directly. This is the one myth the creative is actually built to break, and it is doing that job. `verified` in the creative, `stated` by the brand, and corroborated in comments where women discover mid-thread that their deductible is not what they thought.

**Myth two, real and unaddressed: "I'm stuck with what my employer offers."** Held sincerely and repeated across many ads. It is a myth rather than an objection because it is factually wrong and a single sentence overturns it. The brand has never said that sentence in an ad I could find.

**Myth three, running in reverse: the brand's own hook carries the mistake.** 103 comments across 13 ads say the ad describes an out-of-pocket maximum, not a deductible, and self-identified brokers, agents and medical billers are among them. "That's not a deductible. What she just described is an out of pocket maximum," 2026-05-04. This is the inverse of a myth-busting job. The audience is correcting the brand, in public, under its highest-spend creative.

**And now the more relevant blockers, because myth-busting is not what is holding this journey up.** Marked `inferred`, confidence strong, ordered by how widely each recurs across different ads.

**Trust in what happens after the click.** Covered above. This is the real one.

**Eligibility, which is not a belief at all but a gate.** 42 comments use "qualify," 55 across 17 ads name a pre-existing condition denial, 42 across 15 ads name the pregnancy exclusion. A blocker that is true cannot be reframed away.

**Legitimacy.** Small in count and heavy in weight. Four comments use "legit," and the most-liked of them, with 14 likes on 2025-01-13, is a pasted summary of Reddit threads concluding the brand is "generally considered not legitimate and likely a scam." That is `stated` by a commenter about a third-party forum, not verified by me, and Reddit has not been pulled for this brand yet. It still tells you what a woman finds when she checks.

**Price, which the ad never names.** Seven comments ask "how much." "But you don't say how much is the monthly cost😮‍💨," 2026-04-03. "How much is the monthly I can afford a lot," 2026-07-04. That second one is a buying signal with nowhere to go.

## Recurring pre-purchase questions

The comment corpus is meaningfully a question surface. **166 of 1,322 comments contain a question mark, which is 12.6%.** That is the denominator for everything below. All counts are comments, never people, because authorship is null on every row.

Ranked by spread across different ads, which is the durability test this single-source corpus can actually support:

1. **"Do I qualify?"** 42 comments, 3.2% of the corpus. The most consequential question, because it is answered by a screen rather than by copy.
2. **"What about dads, husbands, sons?"** 16 comments across 12 ads. Mostly asked by women on behalf of a man, which is itself a signal about who does the household's insurance work.
3. **"My kids are grown. Am I still a mom to you?"** 16 comments across 7 ads, asked politely, and never answered on the thread.
4. **"Will you sell my number?"** 15 comments across 10 ads, the highest-liked question in the set.
5. **"Is my state on the list?" and its angry twin, "why am I seeing this if my state isn't?"** Roughly 10 comments across 6 ads. The gate that creates the click also creates this.
6. **"How much is it?"** 7 comments. Nobody is told.
7. **"Has anyone actually tried this?"** 3 comments, and the smallest count on this list carries the most weight because of where the likes are. One drew 15 likes and 6 replies. This is the social-proof question, and the brand loses it by default.
8. **"Is this legit?"** 4 comments using the word, sitting alongside 45 that use "scam," most of which are aimed at the category rather than at this brand.

**Against the brand's own FAQ.** I could not read the live site in this run, so this comparison uses the objection list in the brand context document, which names five: is this legit, I don't want to be sold to, I don't have time, my state probably isn't included, I should wait for open enrollment. Three of the eight questions the audience actually asks most widely are absent from that list: eligibility, who counts as a mom, and what happens to my phone number. `verified` as a gap between two documents I read directly, and the open loops below carry the part of it Parker cannot settle.

**The purchase is not question-light.** It looks question-light because the click is cheap. The questions are all still there, they have simply moved past the form where the brand cannot see them.

## What people love

This section is nearly empty, and the emptiness is the finding.

In 1,322 comments spanning fourteen months, **exactly two report a good experience with this brand's actual service**, and both come from women who were told no.

"Best advice I have gotten from an insurance agent! She didn't have anything that fit but pointed me in the right direction!" 2026-04-17 on `Moms Nahuel WV#1 - V9`, 2 likes.

"I was connected to a very helpful agent. They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful." 2026-04-01 on `MOMS38 - 1 - V1`, 1 like.

`stated`, confidence thin on two comments out of 1,322. Thin is not the same as unimportant. Both people were rejected and both left praise anyway, which is unusual, and both are praising a person rather than a plan. The brand positions its partner agents as "Mom BFFs" who are friendly and pressure-free. These two comments are the only public evidence anywhere that the positioning lands, and they are evidence about the agent, not the product.

**What is brand-specific love versus category love.** There is not enough here to separate them. Category love shows up plenty: women describing a plan they are happy with, none of it this brand's. "My employer finally started offering a copay plan with no deductible. Its a God send," 2026-05-10. Any rival would get credit for that.

**No sign that anyone wishes they had bought sooner.** The brand's context document lists "I wish I'd known about this sooner" as its conversion language. I searched the full corpus for "wish" and found 4 comments. None is that sentence. One is about a lawsuit, one wants to see plans without giving a phone number, one wants an insurance company for men, one is a woman with a chronic illness telling the ad's speaker to stop complaining about a $6,000 deductible.

`inferred`, confidence mixed given the surface's bias toward the unhappy: this brand currently has no post-purchase love to amplify, and that is a real constraint on acquisition creative, because the standard move of turning delight into proof has nothing to draw from. The nearest usable proof asset it does have is two rejected women who thanked the agent anyway.

## Brand-self-echo watch

Two echoes, one small and one large. The large one matters a great deal for the persona work about to be built on top of this.

**The small one: a sentence pattern the brand handed the audience.** The ad `MOMS39 - 2 - V2` overlays a tweet ending "Make that make sense...." and commenters then write "Health care for moms but you don't qualify if your pregnant? Make that make sense." That is the brand's phrasing coming back, and per `customer-review-mining-method.md` it should be tagged low confidence wherever it surfaces in the voice bank. Read: the brand supplied the frame, so this is echo, not customer voice.

**The large one: the brand's stated customer language is not observed customer language.** Section 4 of the brand context document lists what customers supposedly say. Three of its listed conversion lines are "I wish I'd known about this sooner," "My friend told me about this and I'm so glad she did," and "I finally understand my insurance." I searched the only unprompted corpus this brand has for all three shapes. "Wish" appears in 4 comments and never in that form. "Friend" appears in 3 and never as a referral. A semantic sweep for referral language returned zero.

**The call, marked `inferred`, confidence strong.** This is not the good version of the echo, where a brand's messaging is so strong that customers adopt its frame. This is the second version, where the brand is mostly hearing itself. The section is written in the conditional in places, "the outcome language the brand cultivates and that customers ideally echo," which is honest, but it is filed under "Customer Language" and the next reader will treat it as voice of customer. It is not. It is brand copy with no source and no date attached to a single line of it.

The consequence is specific and worth stating plainly. If the persona work and the voice-of-customer work draw from that section, this brand will end up with a customer who talks like its own landing page. The real corpus talks nothing like that. It says "make that make sense," "this is not real life, y'all," "I want the 1990's back," and "I'll trade you and take your 6k." Route this to the persona pipeline and to `voice-of-customer` as a flag, not as a source.

## Persona signals to validate later

Signals only. None of these is a persona, none gets a name, an age or a story here, and the final word on every one of them belongs to `personas-profile.md` and its source pulls, which triangulate identity across more surfaces than a comment section.

**Signal: the older woman who watches the grievance ads.** Source: per-ad delivery data across nine ads in `source-pulls/ad-account.md`. Ads opening on a distressed face deliver 30% to 38% of spend to women 45 and over; warm aspirational openers deliver 7% to 12%. She also watches three to five times longer. Already a live loop in the ad-account pull.

**Signal: the mom whose employer picks her plan.** Source: ad comments, recurring across multiple ads. What makes it a signal rather than an overlay is that her whole situation, not just a behavior, is different. Validate against lead-level data the brand holds.

**Signal: the woman doing the household's insurance work for a man.** Source: 16 comments across 12 ads asking about dads, husbands and sons, plus "With income restrictions? Also I'm a mom but I carry the insurance for my whole family, including dad," 2026-04-23. This is a signal about the decision-maker's scope, not about a new buyer.

**Signal: the after-stage mom.** Source: 16 comments across 7 ads from women whose children are grown or in college, plus a 64-year-old asking about herself alone. "What if I'm a mom, but my son is in college 🤔 i pay more $ to take care of him now than ever before ijs," 2026-03-28.

**Signal: the industry insider inside the audience.** Source: 103 comments across 13 ads correcting the deductible language, many self-identifying as brokers, agents or billers. Not a buyer. A read on how sophisticated the delivered audience is.

**Signal: the mom who left the category.** Source: ad comments plus the category TikTok library, two independent surfaces. The strongest cross-source signal in this doc, and the one with no persona work attached to it anywhere yet.

**Signal from the team itself, and it needs handling carefully.** In Slack on 2026-09-03, the team said of an earlier ICP set: "Some of those ICPs are very wrong." They then approved a corrected framing and added, verbatim: "That sounds about right genrally those 3. I'm sure we can go granular as we go correct? BEcause honestly single moms are fine just as long as we also use lingo about them not being broke if that makes sense." The corrected framing described in that thread is a woman 28 to 50, married or partnered, one to three kids, household income $50,000 to $150,000 or more, with no pregnancy-only targeting.

This is `stated`, it is the team's own word, and it sits in tension with the brand context document Parker holds today, which still carries a profile of a single mother with a $900 emergency fund and a profile of a 41-year-old seven months postpartum. The names differ between the two sets, so the rejected profiles are not literally the current ones, but the shapes overlap. Do not resolve this here. Route it to the persona work with both sources attached, and note that the team's "not broke" rule is a real constraint on how the money trigger gets written.

**Not personas, and worth naming so nobody promotes them later.** Per `persona-research-and-creative-strategy-process.md`, these are overlays that cut across every identity above: the deductible reset, the scheduled procedure, open enrollment timing, the phone-call avoidance, the post-form burn, geographic exclusion. Every one of them can sit on any buyer here. A trigger is a moment, not a person.

## Open loops

**1. Word of mouth is in the script and nowhere else.**

The brand names peer recommendation as a tipping point that can collapse the decision from weeks to minutes, and the account has scripted it twice. In fourteen months and 1,322 comments, three mention a friend, none refers anyone to this brand, and a semantic sweep for referral language returns nothing at all.

*Pull: Gap.* There is a whole discovery channel the brand talks about as if it exists, and the only unprompted surface Parker can read shows no trace of it.

*Question:* Where does a mom who heard about Health For Moms from another mom actually show up?

*Why it is a loop:* if referral is real but invisible, the brand is under-crediting a channel it could feed deliberately. If it is not real, then discovery is one hundred percent paid, and every CPM increase before November lands directly on the business with nothing to cushion it.

*Territory: Product.*

**2. She goes looking for proof, and finds strangers.**

"Anyone actually have this and have insight?" drew 15 likes and 6 replies, and the answers she got were two spam warnings, one "I was told I don't qualify," a "Same," and one woman who was politely turned away and thanked the agent anyway. It happened again in August. The brand has no reviews, no survey, and a search result that a commenter used to call it a scam.

*Pull: Resonance.* Watching a woman ask a comment section to vouch for a brand, and watching the comment section answer, is the clearest picture in this whole doc of the moment the decision is actually made.

*Question:* What does a mom find when she goes looking for proof that this is real before she gives her number?

*Why it is a loop:* the verification step is happening in a place the brand does not own and currently loses. If Parker knew what she finds and where she looks, the fix might be a review surface, a moderation habit, or a line in the creative, and those are very different amounts of work.

*Territory: Messaging.*

**3. Nobody knows how many women hit the gate.**

42 comments use "qualify," 55 across 17 ads describe a pre-existing condition denial, 42 across 15 ads describe the pregnancy exclusion, and one woman on 2026-09-01 says she took the survey twice with different answers and still did not get through.

*Pull: Tension.* The account is graded on cost per lead while a large and unmeasured share of the traffic it buys appears to be screened out after the click, and both of those cannot be the real picture at once.

*Question:* What share of the women who start the qualification flow are screened out, and for what reasons?

*Why it is a loop:* if a large share is screened out, the cheapest fix in the business is upstream of creative, in who the ads invite in the first place, and no amount of hook testing touches it. Only the brand's own funnel data can settle it.

*Territory: Product.* **Routed to the brand.**

**4. The biggest date on the calendar has no journey attached to it.**

The brand calls November 1 the single most important date it has and plans creative two months ahead, which put the start line at September 1. There was no open enrollment creative in the 90 days ending September 2. Meanwhile the comments show women telling each other to wait for November, and being told by their state that they must.

*Pull: Surprise.* A brand that names one date as its whole calendar arrived at that date's planning deadline with nothing in the window built for it.

*Question:* How is a mom's decision different during open enrollment than during the rest of the year?

*Why it is a loop:* the brand is about to spend into its biggest moment using creative written for the other eleven months. If the buyer's urgency, her questions, or even who she is shifts during that window, the current library is the wrong library, and Parker has no read on the shift at all.

*Territory: Messaging.*

**5. Nobody says what it costs, so both the wrong moms and the right ones keep raising their hands.**

The creative never names a price. Seven comments ask "how much," including "How much is the monthly I can afford a lot" on 2026-07-04, which is a buying signal with nowhere to go. At the other end, a woman wrote on 2026-04-09: "So because I make under $30,000 and am under 63.. no othe questions that fit as to why I can't get coverage.. I'm a single mom not making enough to afford insurance so who's this plan for if not moms like me?" Meanwhile the team said in Slack on 2026-09-03 that single moms are fine "just as long as we also use lingo about them not being broke."

*Pull: Tension.* The team's own rule says this buyer is not broke, and the ads carry no signal at all about money, so the women arriving include both the one who cannot afford the plan and the one who could afford much more.

*Question:* How much money does a mom need to have for this offer to actually work for her?

*Why it is a loop:* it is the line between a lead that becomes a customer and a lead that wastes an agent's afternoon, and right now the creative draws no line anywhere. Knowing the floor would change who the ads invite, how the money trigger is written, and whether naming a price earlier would cost volume or buy quality. Part of the answer sits in the brand's own closed-lead data.

*Territory: Personas.* **Partly routed to the brand.**

*Creators and talent produced no new loop in this pass. The live questions about who is on camera are already open in `source-pulls/ad-account.md` and `source-pulls/ad-comments.md`, and nothing in the journey read sharpened them. The territory is left empty rather than filled.*

## Appendix - customer language repository

Every quote is preserved exactly as written, including spelling and punctuation. Source surface and date lead each entry. All Facebook and Instagram ad comments come from Meta ad account `HealthForMoms`, act 484897827497337, pulled via Parker MCP on 2026-09-03 from a corpus of 1,322 comments dated 2025-01-08 to 2026-09-03. Author names are null on every row in this corpus, so no quote can be attributed to a person. Customer reviews and post-purchase surveys do not exist for this brand, so no quote here comes from a confirmed buyer.

### Trigger — finding out the number

- Ad comment, `MOMS38 - 1 - V1`, 2026-03-22, 47 likes, the most-liked comment in the corpus: "This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family. It's insane. I have 2 members of the family with chronic diseases. This absolutely insane. I want the 1990's back."
- Ad comment, `MOMS38 - 1 - V1`, 2026-03-27, 13 likes: "Wow only 6? Must be nice"
- Ad comment, `MOMS38 - 1 - V1`, 2026-03-26: "$6000???? Huh mine is $18000 .....where can I get the $6k"
- Ad comment, `MOMS38 - 1 - V1`, 2026-03-31: "I'll trade you and take your 6k…."
- Ad comment, `MOMS38 - 1 - V1`, 2026-04-02: "6k....try 13k!"
- Ad comment, `MOMS38 - 1 - V3`, 2026-03-17: "A friend's deductible is like 18,000 for family of 4."
- Ad comment, `MOMS38 - 1 - V2`, 2026-04-10: "Ive never had insurance through work and i just found out what tf a deductible is(mines $12,000) and now i have a 2000$ hospital bill that if id had known id have just suffered."

### Trigger — the deductible reset and the calendar

- Ad comment, `MOMS38 - 1 - V3`, 2026-04-04, 6 likes: "After my deductible, I pay 25% of all costs 'til I meet my max out of pocket, and then everything is finally taken care. And then it's the end of the year, and we start all over. I literally hate NYE for this reason!"
- Ad comment, `MOMS38 - 1 - V8`, 2026-03-26, 2 likes: "Mine is $8,000 and I hit it in the beginning of march 🤣😭"
- Ad comment, `MOMS38 - 1 - V3`, 2026-04-25: "yes there is. You have to sign up during open enrollment, not whenever you need it."
- Ad comment, `Moms43 - 4 - V3`, 2026-05-27: "Does this work in Louisiana? Because they wouldnt let me apply for good insurance here until November."

### Trigger — a procedure already scheduled

- Ad comment, `MOMS38 - 1 - V2`, 2026-04-14, 1 like: "This is what I'm afraid of. Just found out I desperately need a hysterectomy. My husband is looking into insurance for me so that I can get it done."
- Ad comment, `MOMS39 - 2 - V2`, 2026-05-04: "how can I get that because I pay $1000 a month for my insurance and tomorrow I have surgery"
- Ad comment, `MOMS38 - 1 - V10`, 2026-04-02: "Our deductible is $10,500 😭 And I have to have surgery in June"

### Prior behavior — the employer plan she cannot leave

- Ad comment, `MOMS38 - 1 - V3`, 2026-03-30: "nope.  My job picks the plan that they offer."
- Ad comment, `MOMS39 - 2 - V2`, 2026-03-17: "Mine is $6k per person too but since it's thru my job I don't really have a choice"
- Ad comment, `MOMS38 - 1 - V3`, 2026-03-28: "The hospital I work for only provides the option to use their insurance company. Last year it was over 18k"
- Ad comment, `MOMS38 - 1 - V2`, 2026-03-27: "Mine is $9,200/individual, $17,500/family and that's the only plan my employer offers 😬"
- Ad comment, `MOMS38 - 1 - V3`, 2026-05-03: "Yep…I work for an insurance company and they now outsource our insurance and our deductible is 4k with no copays"
- Ad comment, `MOMS38 - 1 - V2`, 2026-05-05, the permission line the brand never says: "Y'all have the wrong insurance and if you're deductible, is that high.\n\nYou realize you're not stuck with that insurance?\nYou can find another insurance that has cheaper premiums and has a lower deductible out-of-pocket amounts.\n\nAnd if it's an employer insurance, you don't have to sign up with that employer insurance you can decline the coverage and go out and find your own insurance carrier."

### Prior behavior — the income gap and self-employment

- Ad comment, `B1 samar- Copy`, 2025-08-09: "There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy."
- Ad comment, `MOMS39 - 2 - V2`, 2026-04-02, 7 likes: "Well you being a teacher is why. I'm self employed and can't find anything that doesn't have at least $5k deductible"
- Ad comment, `MOMS39 - 2 - V2`, 2026-03-22: "Literally why I refuse to.get insurance as a self-employed person"
- Ad comment, `MOMS38 - 1 - V2`, 2026-04-09: "So because I make under $30,000 and am under 63.. no othe questions that fit as to why I can't get coverage.. I'm a single mom not making enough to afford insurance so who's this plan for if not moms like me? Doesn't seem legit"

### Prior behavior — leaving insurance for cash pay

- Ad comment, `MOMS38 - 1 - V2`, 2026-03-26, 14 likes: "I would rather have no insurance you would get better self-pay rates then you do with \"having coverage\""
- Ad comment, `MOMS38 - 1 - V8`, 2026-03-21: "I stopped paying for health insurance. Its actually WAY cheaper to not have insurance. We have saved thousands and that includes xrays treatments routine visits"
- Ad comment, `MOMS38 - 1 - V1`, 2026-03-15, 2 likes: "Put your money that you WOULD be paying an insurance into a high yeail savings accound (EASY) and then pay cash which will be way cheaper btw, and if you need a payment plan, make one..  done"
- TikTok, @kaseyjaneanderson, video posted 2026-03-13, 872,100 plays, 75,400 likes, transcript excerpt: "We have not had health insurance for three years. This is the reason why I can be a stay-at-home mom... And we couldn't afford private benefits. So we're uninsured. And it's been the best decision we've ever made."
- TikTok, @readra21, video posted 2025-11-15, 213,100 plays, transcript in full: "You ever wonder why we don't want insurance? Here's our bill prior. And here's our bill cash pay. This is why the insurance companies need to be out."

### Hesitation — what happens to my phone number

- Ad comment, `MOMS38 - 1 - V3`, 2026-03-16, 33 likes, the third-most-liked comment in the corpus: "Filled it out and have been getting calls everyday from all sorts of companies which are mostly India based.  Also, the harassment from whomever keeps calling me about Medicare (India again).  This is the ONLY form I've filled out since getting my new phone number 3 months ago so it came from this site!"
- Ad comment, `B1 samar- Copy`, 2025-11-28: "I filled this out because it literally says we won't be contacted by random agents. That's a lie. I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies."
- Ad comment, `B2 - 10TH JUNE - Copy 16`, 2025-10-06: "They just sell your info. I did the form, and immediately got multiple calls and texts from different, unrelated insurance agents."
- Ad comment, `B1 samar- Copy`, 2025-09-17, 1 like: "Do not give them your info. They send it to multiple different private insurance agents and you'll get a million texts and calls."
- Ad comment, `MOMS38 - 1 - V1`, 2026-03-29, 5 likes: "April Crawford wondering the same. I filled out something like this years ago- and got spam phone calls every 10 minutes for months!"
- Ad comment, `OMC - C11 - 2b`, 2026-03-13: "Really wish you could see plans without adding all your personal information to get even more telemarketing calls than we already do."
- Ad comment, `MOMS38 - 1 - V8`, 2026-03-11, 2 likes: "I don't wanna put my information and get called by hundreds of people though.."

### Hesitation — is this real, and did it work for anyone

- Ad comment, `MOMS38 - 1 - V1`, 2026-03-20, 15 likes and 6 replies: "Anyone actually have this and have insight?"
- Ad comment, `MOMS38 - 1 - V1`, 2026-04-01, 2 likes, a reply on that thread: "That's exactly what will happen here. Their website says they are a third party agency to connect you to agents.  You'll get hundreds of calls and the plans aren't great. Website says they don't guarantee coverage or plans. \nThey are hoping you sign up for a \"cheaper\" plan on paper but really it doesn't cover anything."
- Ad comment, `Moms43 - 4 - V3`, 2026-08-19, 1 like and 2 replies: "Has anyone had success with this?"
- Ad comment, `Moms43 - 4 - V3`, 2026-09-01, the reply to it: "Cassie Smithson I didn't. I took the short survey twice and slightly changed up my answers and it still didn't work out for me. Bummer"
- Ad comment, `MOMS38 - 1 - V1`, 2026-04-04: "Have anyone tried this?"
- Ad comment, `Moms43 - 4 - V3`, 2026-08-15: "Has anyone tried this? I pay quite a bit for an employee plan with a very high deductible. Is this worth it and is it widely accepted?"
- Ad comment, `B1 samar- Copy`, 2025-07-24, 1 like: "A Google search doesn't pull anything about this. Is it legit?"
- Ad comment, `Moms43 - 4 - V1`, 2026-04-27: "Is this legit?"
- Ad comment, `IMG 6`, 2025-01-13, 14 likes, the Reddit summary paste, opening line only, full text in `source-pulls/ad-comments.md`: "According to discussions on Reddit, \"Health for Moms\" insurance is generally considered not legitimate and likely a scam, as many users report extremely limited coverage, difficulty cancelling policies, and concerns about the company's practices not aligning with standard health insurance expectations"

### Screened out — where the journey ends for many

- Ad comment, `B2 - 10TH JUNE - Copy 16`, 2025-07-07, 1 like: "Was so excited about this but as soon as i said diabetic i didnt qualify"
- Ad comment, `B2 - 10TH JUNE - Copy 16`, 2025-07-01, 3 likes: "If you are currently pregnant, you dont qualify. Its underwritten, if you have health concerns, be warned"
- Ad comment, `Moms43 - 4 - V3`, 2026-08-13, 2 likes: "It only works if you don't have any preexisting conditions. You gotta be perfectly healthy to qualify it looks like"
- Ad comment, `MOMS38 - 1 - V1`, 2026-04-02, 1 like: "April Crawford I was told I don't qualify 🤷"
- Ad comment, `B1 samar- Copy`, 2025-08-05: "Dont qualify. T1D."
- Ad comment, `moms-63 3e`, 2026-09-02: "Preexisting health condition of cancer disqualified me"
- Ad comment, `MOMS30 - 1 - V20`, 2026-02-03: "Health for Moms, but only if your babies are out of the womb. I was denied for being pregnant. Scam."
- Ad comment, `B2 - 10TH JUNE - Copy 16`, 2025-07-16: "Another predatory health insurance company. If you are truly for moms why do you disqualify pregnant women and those with preexisting conditions. Ridiculous!"

### Pre-purchase questions — price, eligibility, and who counts as a mom

- Ad comment, `MOMS38 - 1 - V8`, 2026-04-03: "But you don't say how much is the monthly cost😮‍💨"
- Ad comment, `Moms43 - 4 - V3`, 2026-07-04: "How much is the monthly I can afford a lot"
- Ad comment, `MOMS38 - 1 - V10`, 2026-05-04: "So how much is your monthly payment?"
- Ad comment, `Moms43 - 4 - V3`, 2026-05-11: "So I tried to sign up. Is this just for mom only? It says no options for mom + family. Or mom + dependent children. Clarify?"
- Ad comment, `MOMS 28 - N3 - Body 3 - Hook5`, 2025-12-18: "So I filled out form, watched video.  How can I see the plans online so I can compare?"
- Ad comment, `MOMS38 - 1 - V3`, 2026-03-23: "What if I have an insurance plan that is too expensive but want to change it? Can I apply?"
- Ad comment, `MOMS38 - 1 - V9`, 2026-03-28, 2 likes: "What if I'm a mom, but my son is in college 🤔 i pay more $ to take care of him now than ever before ijs"
- Ad comment, `MOMS38 - 1 - V2`, 2026-04-23: "With income restrictions? Also I'm a mom but I carry the insurance for my whole family, including dad. Can he get on this magical plan?"
- Ad comment, `moms-53 3`, 2026-09-02: "Why is this being shown in IL if it's not on the list???😭🤦🏼‍♀️"

### Post-purchase — the only two good experiences in the corpus

- Ad comment, `Moms Nahuel WV#1 - V9`, 2026-04-17, 2 likes: "Best advice I have gotten from an insurance agent! She didn't have anything that fit but pointed me in the right direction!"
- Ad comment, `MOMS38 - 1 - V1`, 2026-04-01, 1 like: "I was connected to a very helpful agent. They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful."

### Post-purchase — the bad ones

- Ad comment, `MOMS30 - 1 - V20`, 2026-02-04, 4 likes: "I got pushed around and given to a side insurance company. I had already done all of that and then some and tried this, so no I DO NOT RECOMMEND!"
- Ad comment, `MOMS31 - N1 - 1B`, 2026-01-28: "It listed no selling my number to scammers but it's been just a few hours and I've had multiple numbers contact me with different agency type names"
- Ad comment, ad name not captured on the semantic row, 2026-01-27: "Nice try lol I tried to get health insurance through this place and it was over $500/month. And they used hours of my time in order to tell me!"

### Recognition — what the audience says is about them

- Ad comment, `MOMS38 - 2 - V1`, 2026-04-03, 4 likes: "\"It's out of network\"  \"But it's in the same building!\"  \"In a different hallway\"  🤣🤣🤣🤣🤣 whoever came up with this ad deserves a raise!! Love this!"
- Ad comment, `MOMS38 - 2 - V1`, 2026-04-06: "TRUTH! A SAD TRUTH."
- Ad comment, `MOMS38 - 2 - V4`, 2026-03-23: "Had a similar conversation recently with my soon to be former insurance company."
- Ad comment, `MOMS38 - 2 - V1`, 2026-04-06: "At the Mayo Clinic for my husband right now.  Absolutely dealing with this."

### Category voice — how moms outside this brand talk about the same problem

- TikTok, @drashleehendry, posted 2025-11-12, 6,200,000 plays, 661,800 likes, 208,000 shares, opening line: "This is Dr. Ashley Hendry. I was calling to get a quote for a self-pay patient to see what the global vaginal delivery fee would be."
- TikTok, @paumod, posted 2026-01-08, 916,200 plays, opening line: "If you're watching this and you're pregnant, don't shop for anything until you call your health insurance if you have it obviously."
- TikTok, @salina_sunshine, posted 2026-08-31, 235,800 plays, opening line: "My son started to have really bad headaches and then fainted. We ended up in the ER and then had to see several specialists and do more testing. And even with health insurance, these bills just keep coming."

### The brand's own creative, for comparison with the voice above

- Ad script, `moms-53 3`, created 2026-08-25, pulled 2026-09-03, in full: "I'm so thankful for the mom that told me about this. / If you're a mom and you live in one of these states and you're tired of paying high deductibles, high premiums for health insurance for your family, listen up. / It takes you 30 seconds, it's a brand new website. / As long as you live in one of those states, you can click down here below, fill it out and see if you qualify for lower premiums and a $0 deductible."
- Ad script excerpt, `moms-63 3e`, created 2026-08-14, pulled 2026-09-03: "I almost scrolled past this because I thought, 'I already have health insurance, this doesn't apply to me.' ... So I checked. ... Worst case, you check and stick with what you have. Best case, you realize you've been paying way more than you needed to."
- Static headline, `B1 - Copy 7`, created 2025-02-26: "Left my big insurance company for a mom-focused one. 24% cheaper and I choose my own doctor 😌"
- Text hook, `Moms43 - 4 - V3`, created 2026-04-06: "POV: Telling your husband you found better health insurance, saved $400 a month, AND the deductible is zero. Wife of the year energy. 💕"

### Team language, from Parker chat history

- Slack, Health For Moms channel, 2026-09-03: "Some of those ICPs are very wrong. I'm uploading branding guidelines into your Training. Do you want me to wait until you see those are want me to send that document here also?"
- Slack, Health For Moms channel, 2026-09-03: "That sounds about right genrally those 3. I'm sure we can go granular as we go correct?\n\nBEcause honestly single moms are fine just as long as we also use lingo about them not being broke if that makes sense"
- Slack, Health For Moms channel, 2026-09-03: "Sounds good we don't have reviews but you can pull from competitor reviews or health insurance Reddit etc"

### Lookup section — quotes with no source or date, not usable as evidence

These come from Section 4 of the brand context document, which is titled "Customer Language." Not one line carries a source, a surface or a date, and none of them appears in the 1,322-comment corpus in any form. They are listed here so a later reader can see exactly what was excluded and why, and they must not be treated as voice of customer. What is missing: source surface, date, and any evidence that a customer said them.

- "I wish I'd known about this sooner"
- "My friend told me about this and I'm so glad she did"
- "I can't believe how much I was overpaying"
- "I finally understand my insurance"
- "My family is covered, no matter what"
- "I made a smart choice"
- "No more worrying every time my kid gets sick"
- "It was so easy — I just answered a few questions"
- "They actually explained things in a way I could understand"
- "Nobody pressured me — they just showed me my options"
- "I don't even know what my plan covers"
- "I'm scared one ER visit will wipe us out"
- "They don't give a rat's butt about people like me"
- "We are super middle class — how are we stuck with everything?"

## Appendix - Parker media links

### Own ads, playable media and Parker dashboard links

`Moms43 - 4 - V3`, the account's top-spending video, created 2026-04-06:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`MOMS38 - 1 - V1`, the grievance winner and the ad carrying the thread where women asked each other whether this is real:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/50a0309be06d87e55299b9e00d7962b88516c847dec96e80cfd47e6ba5959b66.mp4
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239934711290519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`MOMS38 - 1 - V2`:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/69af0d6f1d49f1bb1d77aab8a83c89100912a7bb4f0c7a12c5f177edb41c4e93.mp4
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239934711130519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`MOMS38 - 1 - V3`, the ad carrying the comment about daily calls that drew 33 likes:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/34abf0402e049c2957caeafa6a203a955020b08a7b48b7547bb5867a59a033eb.mp4
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239934711030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`MOMS39 - 2 - V2`, the $6,000 deductible tweet ad:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b5709e2fc3c51b32fc818394fcc0d33d94206dccad0c923f953671d48875d937.mp4
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239934711200519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`Moms43 - 4 - V4`, same hook as the top spender, different opening visual:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/985c6a8045a5bcfb5e7450ad0f3a00ca783b996f4ba3633337e8c84e1aac8a39.mp4
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380050519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`MOMS34 - N1 - 3a`, the peace-of-mind montage:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1c501ac53c00f4e6b9f3ee87626968c02aa9861c6958bcf6c338644cbaf1fa8d.mp4
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238774764390519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`moms-53 3`, the peer-referral script, created 2026-08-25:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`moms-53 5`, the same referral line preceded by the deductible complaint:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1f24bccea594c5e32b7748c684f40efa1c93d4c963b440171bf7eb37e26ffc04.mp4
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254793290519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`moms-63 3e`, the script that names the hesitation, and the cheapest funded video in the account:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`moms-63 3b`, the same script with a different opener:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/d18d8bec80b278476603cb815c109469b13b58151c8137f01fda7de626650752.mp4
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093452350519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`B1 samar- Copy`, the largest lifetime spender and the ad carrying most of the 2025 comment history:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/59bf52c09c6081e3dfc63e0b17e649c989b490ad5b03079e469d1dc258e2cc0f.jpg
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120228910482200519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`B1 - Copy 7`, the static that tells a switching story, at an $11.74 lifetime CPL:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/7e3133fccf8b205622146f7297669b76296123fb46177e5262ee89f0040ca8ba.jpg
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120216241083030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

`B2 - 10TH JUNE - Copy 16`, the static carrying several comments from women who were screened out:
- https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/2196cede33edbb670d810d017aa0c57568dc50db2e8c71b7b7a608410b0c0aae.jpg
- https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120224684049380519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

### Landing destinations named in the account

- https://www.healthformoms.co/save/
- https://quiz.healthformoms.com/#/indvfam

### Category TikTok, from the Parker mining library

Dr. Ashlee Hendry, cash-pay pregnancy pricing, 6,200,000 plays:
- https://www.tiktok.com/@drashleehendry/video/7571648042147908894
- https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7571648042147908894_1788468281/7571648042147908894_join_me_as_i_call_around_and_get_self_pay_pricing_.mp4
- https://app.heyparker.ai/dashboard/inspiration?video_report=a15b7ef7-b29d-467f-8498-893c832bf05a&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

@paumod, what insurance covers for maternity, 916,200 plays:
- https://www.tiktok.com/@paumod/video/7593050209676987662
- https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7593050209676987662_1777257347/7593050209676987662_if_you_have_health_insurance_they_may_cover_matern.mp4
- https://app.heyparker.ai/dashboard/inspiration?video_report=94e28178-adf8-4ee5-9de1-a274f54dddf7&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

@kaseyjaneanderson, three years uninsured by choice, 872,100 plays:
- https://www.tiktok.com/@kaseyjaneanderson/video/7616717859724545311
- https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7616717859724545311_1779072506/7616717859724545311_ive_wanted_to_make_this_video_for_so_long_but_was_.mp4
- https://app.heyparker.ai/dashboard/inspiration?video_report=731bd1a3-8c13-4faa-8c54-ccdce1503972&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

@salina_sunshine, the ER bill and the cost of living, 235,800 plays:
- https://www.tiktok.com/@salina_sunshine/video/7680344555161521421
- https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7680344555161521421_1788468674/7680344555161521421_how_are_we_supposed_to_keep_up_with_all_of_these_c.mp4
- https://app.heyparker.ai/dashboard/inspiration?video_report=82407e0c-f8d6-43a4-b320-88f48775a5ba&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

@readra21, the cash-pay bill reveal, 213,100 plays:
- https://www.tiktok.com/@readra21/video/7572985864435879181
- https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7572985864435879181_1788468482/7572985864435879181_selfpaynoinsurance_emergencyroom.mp4
- https://app.heyparker.ai/dashboard/inspiration?video_report=d4293d9f-8006-49df-9a76-a9abff310d2b&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

@amandatalksalot, budgeting for a baby including the insurance line, 14,400 plays:
- https://www.tiktok.com/@amandatalksalot/video/7538841869065768247
- https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7538841869065768247_1788469125/7538841869065768247_dont_let_my_numbers_scare_you_go_through_your_expe.mp4
- https://app.heyparker.ai/dashboard/inspiration?video_report=8311a25c-dbdd-48b4-8ae9-b0da327be0ac&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

### Source documents read for this pass

- `source-pulls/ad-account.md`
- `source-pulls/ad-comments.md`
- `running-notes/missing-context.md`
- `running-notes/brand-rules.md`
- `running-notes/success-definition.md`

Comment permalinks are null on all 1,322 rows in this corpus, so no individual comment can be linked. Every comment quoted above is retrievable by its ad name and date through Parker MCP `search_facebook_ad_comments_sql`.
