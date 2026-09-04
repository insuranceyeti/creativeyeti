---
brand: health-for-moms
doc: ad-comments
generated_on: 2026-09-03
refresh_by: 2026-10-03
sources_read:
  - Facebook and Instagram ad comments, Meta ad account HealthForMoms, act 484897827497337, via Parker MCP search_facebook_ad_comments_sql, full corpus paginated in three pages of 500 on 2026-09-03
  - Parker MCP search_facebook_ad_comments_semantic, six themed passes, each reporting the same 1,322-comment corpus
  - Full creative pulled via Parker MCP search_facebook_ads_sql for 20 ads, with ad_analysis, ad_summary, creator_demographic, scripts, hooks and lifetime metrics
  - Brand context document via Parker MCP get_brand_persona, read for the five stated ICPs and the brand's own stated objection list
  - running-notes/missing-context.md, for the dark-surface rules this brand runs under
comments_read: 1,322 comments, which is 100% of the corpus Parker holds for this brand. They sit on 112 distinct ad IDs and 79 distinct ad names, dated 2025-01-08 through 2026-09-03. 1,023 are top-level and 299 are replies. Full creative was read on 20 ads that together carry 997 of the 1,322 comments, or 75%.
data_limitations:
  - author_name is null on all 1,322 rows and permalink_url is null on all 1,322 rows. There is no way to dedupe by person, count unique commenters, or read a name for any signal. Every "how many people" read in this doc is really "how many comments."
  - Customer reviews and post-purchase surveys are both empty for this brand, per running-notes/missing-context.md. That means nothing in this doc can be corroborated against a confirmed buyer. This is the single biggest limit on the whole read, and it caps confidence on every identity below.
  - No competitor ad comments are reachable. No rival brands are tracked in the Parker app, so there is no category baseline to say whether these objection rates are high, low, or normal for health insurance lead generation.
  - A commenter cannot be tied to a lead, a call, or a policy. Parker holds no join between a comment and the 4,336 leads the account produced in the last 90 days.
  - The demographic splits quoted below come from Meta spend-weighted delivery, not from the commenters. The two are different populations and are not interchangeable.
  - There is no get_current_time tool on this MCP surface. The dates above come from the session clock, which reads 2026-09-03 and matches the date stamped on the rest of this build.
  - refresh_by is set 30 days out rather than the 180-day persona-source cadence in parker-system/system/refresh-cadence.md. The prompt calls for a fast cadence because comments accrue daily while campaigns are live, and that trigger has fired: 10 new comments landed in the first three days of September 2026 alone.
---

# Ad comments — persona signal — Health For Moms

## How this read was built, and what it can and cannot carry

I pulled every comment Parker holds for this brand, not a sample. Three paginated calls of 500 returned 1,322 unique rows, and a fourth call at offset 1,322 returned zero, which confirms the corpus end. Six separate semantic passes each reported `totalCommentsAnalyzed: 1322`, so the two tools agree on the denominator. I read all 1,322 messages in full, not just the headlines, because the customer-review mining method warns that the usable line usually sits in the middle of a comment that reads as background at a glance. Then I pulled full media on the 20 ads carrying the most comments, so that every claim about who an ad was built to reach comes from the script, the visual hook, the creator description and the ad analysis, never from the ad name.

Two things shape how much weight any of this can hold.

First, a commenter is not a buyer. This corpus captures whoever the algorithm served, which for this account is a very wide net. Meta spend on the eight ads with the most comments ran 97% female, 48.4% aged 35 to 44, 23.8% aged 25 to 34, 99.7% mobile, and split 59.4% Facebook to 40.2% Instagram. That is a big, cheap, broad audience, and a comment section that size fills with people who will never buy.

Second, and more serious for this brand: there is nothing to check this against. Reviews are empty. Surveys are empty. The persona method ranks evidence with post-purchase survey data at the top and community comments near the bottom, and this brand has only the bottom tier. So the honest confidence ceiling on every identity below is **thin to mixed**, never verified, no matter how many times a phrase recurs. Recurrence inside one noisy source is still one source. I have said so on each read rather than rounding any of them up.

One more shape worth holding before the findings. The corpus is lopsided. 795 of 1,322 comments, or 60%, sit on a single creative family, `MOMS38 - 1`, and 506 of 1,322, or 38%, were posted in April 2026 alone. So a signal that looks huge may really be one ad in one month. I have carried the ad spread on every objection for exactly this reason: how many different ads a thing appears on is better evidence than how many times it appears.

## Identity signals observed

### The insured mom who is still broke

This is the dominant identity in the corpus and it is not the identity the creative was built for. 160 of 1,322 comments, or 12%, disclose the commenter's own deductible or premium in a self-report frame, and they appear across 17 different ads. These are not uninsured shoppers. They already pay for a plan. They are saying it does not work.

The evidence walk. The winning ad, `MOMS38 - 1 - V1`, opens on a woman filming herself, visibly annoyed, with the words "Health Insurance is a scam 🙄" over her head, saying "My deductible is $6,000. I have to spend $6,000 in medical expenses before everything is taken care of and there's no copays. But yet I pay for that insurance." What the comment section did with that number is the finding. It did not read as a pain point to be relieved. It read as an opening bid. "Wow only 6? Must be nice" drew 13 likes on 2026-03-27. "$6000???? Huh mine is $18000 .....where can I get the $6k" landed 2026-03-26. "I'll trade you and take your 6k…." landed 2026-03-31. "Mine is 18,000" landed 2026-04-05. "6k....try 13k!" landed 2026-04-02. The single most-liked comment in the entire 1,322-row corpus, with 47 likes, is this one from 2026-03-22 on `MOMS38 - 1 - V1`: "This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family. It's insane. I have 2 members of the family with chronic diseases. This absolutely insane. I want the 1990's back."

My read, marked inferred: this is a trigger-anchored identity in the sense the persona method means, and the trigger is the moment she found out the number. She is not shopping. She is grieving a bill and looking for someone to agree with her. In TEEP terms she is sitting hard in **Trigger**, the phase where a need has just become conscious, and the creative is written for **Evaluation**, where a specific plan is being compared. That mismatch is visible in the comments themselves: people answer the ad's number instead of answering the ad's offer. Confidence: mixed. The volume and the ad spread are real, but nothing confirms any of these commenters bought.

### The employer-plan captive

A distinct sub-identity inside the group above, and the one that quietly breaks the ad's premise. The creative assumes you can switch. A recurring set of commenters says plainly that they cannot.

Verbatims, each with its date and ad. "nope. My job picks the plan that they offer." on 2026-03-30, `MOMS38 - 1 - V3`. "Mine is $6k per person too but since it’s thru my job I don’t really have a choice" on 2026-03-17, `MOMS39 - 2 - V2`. "The hospital I work for only provides the option to use their insurance company. Last year it was over 18k" on 2026-03-28, `MOMS38 - 1 - V3`. "Mine is $9,200/individual, $17,500/family and that’s the only plan my employer offers 😬" on 2026-03-27, `MOMS38 - 1 - V2`. "Yep…I work for an insurance company and they now outsource our insurance and our deductible is 4k with no copays" on 2026-05-03, `MOMS38 - 1 - V3`.

My read, marked inferred: she is reachable by the ad and not reachable by the offer, at least not without a message that names the employer-plan trap directly. She has no idea she is allowed to decline employer coverage, and one commenter tells her so in the replies rather than the brand doing it: "if it’s an employer insurance, you don’t have to sign up with that employer insurance you can decline the coverage and go out and find your own insurance carrier" on 2026-05-05, `MOMS38 - 1 - V2`. Confidence: mixed on the identity, thin on the size, because there is no way to count how many of the 4,336 leads came from this state.

### The chronic-condition mom, loud and unservable

Small by volume, largest by emotional intensity, and the persona method says to keep those two rankings separate rather than flattening them into one. These commenters describe a medical reality, not a budget preference.

"Add having a son fighting cancer for 7+ years." on 2026-04-12, `MOMS38 - 1 - V3`. "My daughters 1 January claim was $364,000. She had half a million in claims over a week." on 2026-04-20, `MOMS38 - 1 - V9`. "This year it took 35 days to hit our 8k OOP. Next year it could take as few as 1 depending on how prescriptions hit. Child is on 1 med that is $3600 per fill. I am on a combo of meds that are $2,600, 1,800, and $3,200." on 2026-03-31, `MOMS39 - 2 - V2`. "girl, we pay $2,200 a month and its a battle for them to cover anything. I have MS so I NEED to be covered for my treatments" on 2026-03-23, `MOMS38 - 1 - V1`, with 4 likes. "I have to pay 16000 before they cover anything and my husband pays over 300/wk for our insirance. Im in cancer remission...have to have CT scans every 6mo and physical checks in between...so by December just hit it...oh but its Jan. Now so it starts over...and they still never cover anything.... insurance is the biggest scam 😒" on 2026-03-24, `MOMS38 - 1 - V3`.

My read, marked inferred: this is the highest-intensity identity in the corpus and the product's medical underwriting screens her out. That collision is covered in the objection section below and it is the single sharpest tension the comments surface. Confidence: strong on the intensity, thin on the volume, since roughly 20 comments carry it.

### The self-employed mom in the income gap

Matches the brand's own ICP "Courtney" closely enough to be worth naming as corroboration of a stated persona rather than a new one. "Well you being a teacher is why. I’m self employed and can’t find anything that doesn’t have at least $5k deductible" on 2026-04-02, `MOMS39 - 2 - V2`, with 7 likes. "Literally why I refuse to.get insurance as a self-employed person" on 2026-03-22, same ad. "There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy." on 2025-08-09, `B1 samar- Copy`. "I don't have any pre-existing conditions, so I don't think that was it. Probably more likely that they don't cover in my area. Or my income doesn't fall into the sweet spot. I don't make very much, just more than medicaid allows (which is far below poverty level)." on 2025-08-03, `B1 samar- Copy`.

Worth noting that the ad built expressly for this identity is `B1 samar- Copy`, whose script says "Everyone told me get Obamacare, apply for Medicaid. What they didn't say - those don't work if you're in the middle. I make too much for Medicare, but not enough to drop $600 a month on a plan I barely use." That ad carries the lowest cost per lead of the eight ads with the most comments, at $14.12. The identity and the message line up. Confidence: mixed, and it is the one identity here that a stated ICP and the comment evidence both point at.

### The insurance insider, correcting the ad in public

The most surprising identity in the corpus, and the one nobody would have predicted from the targeting. 103 of 1,322 comments, or 8%, across 13 ads, argue with the ad's use of the word deductible. Many identify themselves.

"As a licensed insurance broker this is VERY misleading in the beginning. The first half is talking about a medical maximum out of pocket. A deductible is something you pay before your insurance kicks in with co insurance." on 2026-04-07, `MOMS38 - 1 - V1`. "Deductible is different than maximum out of pocket 😃 -an insurance agent" on 2026-05-01, same ad. "I’m a licensed insurance brokers." on 2026-03-31, `MOMS38 - 1 - V5`. "As someone that bills medical claims to insurances, and adores my offices patients, I find it all nauseating." on 2026-03-25, `MOMS38 - 1 - V1`. "That's not a deductible. What she just described is an out of pocket maximum." on 2026-05-04, `MOMS38 - 1 - V2`, followed by a full four-paragraph explanation. And one commenter naming the damage directly on 2026-04-03, `MOMS38 - 1 - V3`: "THANK YOU  I was so annoyed that she was talking about how shit is covered in full once ded is met because unless it's the same amount as OOPM, that's incorrect."

My read, marked inferred: the hook's central claim is technically wrong, the audience contains enough industry people to notice, and the correction is now the second-largest conversation under the brand's best-performing creative. This is not a persona to target. It is a credibility leak sitting on the account's highest-spend ad, and it is real signal about the sophistication of the audience Meta is finding. Confidence: strong that the pattern exists, since 103 comments across 13 ads is wide spread on a 1,322 denominator. Data-limited on whether it costs anything, because nothing here connects a correction to a lead.

### The rival agent farming the comment section

39 comments across at least 10 ads pitch a competing offer under the brand's own creative. Some are polished and repeated verbatim, which suggests a small number of operators working the account.

"Heather, you can pair Direct Primary Care with a low premium health plan and have a comprehensive health plan...Check mapper.dpcfrontier.com for a location near you. And then you can pair DPC with an unbundled health plan like this hybrid that is a month-to-month renewing plan, to meet major medical at 100% after IUA: www.blueoceanemployerbenefits.com/individual-plans" on 2026-04-07, `MOMS38 - 1 - V1`. That same operator's script appears at least eight more times under the same ad on the same day, addressed to different women by name. Others are blunter. "You can get a health insurance without paying premiums $0/month (depending on your eligibility) as well as $0 deductible. Pm me if you need health insurance." on 2026-04-07, `MOMS38 - 1 - V2`. "my team can assist you if and when you need it. I think it's odd to market to moms but not offer anything dor maternity...682-307-0039 Health Insurance Confidant Consulting" on 2025-07-25, `B1 samar- Copy`. "As a licensed health insurance advisor, never put your info online unless you want 100 calls a day about health insurance. Also you dont have to be a single mom to find a zero deductible plan...DM and I can help you look at the plans available in your state and find fits your needs best." on 2026-07-16, `Moms43 - 4 - V3`, with 1 like.

My read, marked inferred: the brand is paying to create demand and a competitor is intercepting part of it in the comments, for free, using the brand's own credibility problem as the wedge. 17 of the 39 sit on `MOMS38 - 1 - V1`, the account's single highest-spend ad at $54,173 lifetime.

### The anti-category self-insurer

33 comments across 10 ads argue that the right move is to drop insurance and pay cash. This person will never buy, but she is loud and she is persuasive to the people around her. "I stopped paying for health insurance. Its actually WAY cheaper to not have insurance. We have saved thousands and that includes xrays treatments routine visits" on 2026-03-21, `MOMS38 - 1 - V8`. "Put your money that you WOULD be paying an insurance into a high yeail savings accound (EASY) and then pay cash which will be way cheaper btw, and if you need a payment plan, make one.. done" on 2026-03-15, `MOMS38 - 1 - V1`, with 2 likes. "I would rather have no insurance you would get better self-pay rates then you do with \"having coverage\"" on 2026-03-26, `MOMS38 - 1 - V2`, with 14 likes.

My read, marked inferred: this is not a persona for this brand, it is a competing worldview that the ad's own "insurance is a scam" hook actively recruits. The hook agrees with her, and she agrees back, and then declines the product. Confidence: mixed.

### The politically primed reactor

54 comments across 14 ads route the complaint to a political cause, in both directions, and they carry the highest like counts in the corpus after the deductible disclosures. "Thanks, Obama" drew 21 likes on 2026-03-16. "Everyone, thank Obama" drew 24 on 2026-04-13. "The affordable care act made insurance unaffordable for most with the premiums and the high deductibles." drew 36 on 2026-03-30, the second-most-liked comment in the corpus. Pointing the other way: "Keep fighting for billionaires, they care about you." drew 12 on 2026-03-22, and "FOR PROFIT HEALTHCARE IS MURDER." on 2026-03-16.

My read, marked inferred: this is mostly reaction-noise rather than persona signal, and I am treating it that way. It matters for one reason only. It tells you the emotional state the creative lands in. The emotional-delivery method calls this the landing state, and the state here is high-intensity negative, the Panic and Bummer zones, which narrows attention and suppresses the reflective processing that identification needs. That is a plausible reason recognition is so rare in this corpus and argument is so common.

### The person the ad was never for, showing up anyway

Dads, single dads, stay-at-home dads, women whose kids are grown, women with no kids, a 64-year-old, a student. 16 comments across 12 ads ask about dads or men. 16 across 7 ads say the commenter is not a mom or no longer has kids at home. "Moms aren't the only caregivers. I'm a stay at home dad" on 2026-08-17, `Moms43 - 4 - V3`. "What if your kids are grown" on 2025-08-07, `B1 samar- Copy`. "I have a $0 deductible and I am not a mom" on 2026-03-24, `MOMS38 - 1 - V3`. "What if I’m 64 only need coverage for myself" on 2026-05-31, `Moms36 - 3 - A - 2 - V4c`.

## Recurring objections, with the identity behind each

Ranked by how widely each recurs across different ads, because the review-mining method is right that spread beats raw count, and because this corpus is heavily concentrated on one ad family and one month.

### 1. "You call yourself Health For Moms and you won't cover me because I'm pregnant"

**42 comments across 15 different ads, spanning 2025-07-01 to 2026-06-09.** This objection spreads across more ads than any other in the corpus, and it has run the longest. It survives every creative refresh.

The identity behind it: the expecting or brand-new mom. That is not an accident of targeting. It is the brand's own stated ICP "Nicole — The Second-Chapter Mom," described in the brand context document as 41 and seven months postpartum with her first baby. The creative recruits her by name and the product screens her out.

The verbatims, exactly as written. "How can you have healthcare for moms if you don’t cover maternity? Makes zero sense. False advertising." on 2025-08-12, `B1 samar- Copy`. "Health for Moms, but only if your babies are out of the womb. I was denied for being pregnant. Scam." on 2026-02-03, `MOMS30 - 1 - V20`. "Health care for moms but you don’t qualify if your pregnant? Make that make sense." on 2026-05-05, `MOMS38 - 1 - V2`. "Marketing towards mothers while not covering pregnancy is a disgusting tactic." on 2025-11-23, `B1 samar- Copy`. "Ours is 2,500 but we pay $1700 a month and pay $25 for reg appts and $75 for special drs. Its freaking nuts but your insurance says im not eligible because im pregnant 😂 huh.. so much for being for Moms 😂" on 2026-04-01, `MOMS38 - 1 - V3`, with 7 likes. "One question literally asks if you are pregnant or planning to be pregnant? The answer choices are no and I’m not planning to be or yes I’m pregnant. I’m not pregnant but I’m planning to be. So I picked yes pregnant and it says there are no plans. You would think if it is advertising as a mom insurance company then pregnancy status should not matter." on 2026-02-08, `MOMS30 - 1 - V20`. And the one that names the exact edge case the funnel creates: "Why can’t you get this if you want another kid? I don’t know when I’m gonna have another kid, but I do know I want another kid. My family isn’t done growing. ￼" on 2026-04-22, `MOMS38 - 1 - V3`.

Why this is load-bearing rather than a complaint log: the objection is doing brand damage in public because the name of the brand is the setup for the joke. Nine of these comments use the brand's own name as the opening clause of the objection. And the brand's own stated objection list, pulled from the brand context document, does not contain it at all. The five objections the brand says it handles are "Is this legit?", "I don't want to get on a call and be sold to", "I don't have time", "My state probably isn't included", and "I should just wait for open enrollment." The widest objection in its own comment sections is not on that list. Marked verified as a gap between the two documents, since I read both directly.

### 2. "Pre-existing conditions disqualify you, so this isn't for anyone who actually needs it"

**55 comments across 17 different ads.** Diabetes is named 11 times specifically. The identity behind it is the chronic-condition mom described above, and this is where her intensity collides with the underwriting.

"Don’t bother looking into it if you’re diabetic . I’ll be uninsured until I die." on 2025-08-14, `B1 samar- Copy`. "Was so excited about this but as soon as i said diabetic i didnt qualify" on 2025-07-07, `B2 - 10TH JUNE - Copy 16`, with 1 like. "Preexisting health condition of cancer disqualified me" on 2026-09-02, `moms-63 3e`, which is three days ago and shows the objection is current. "It only works if you don’t have any preexisting conditions. You gotta be perfectly healthy to qualify it looks like" on 2026-08-13, `Moms43 - 4 - V3`, with 2 likes. "RIIIIIGHT…. As long as you have perfect health and no pre-existing conditions. Fucking scam." on 2025-08-21, `B1 samar- Copy`, with 1 like. "I like how it's \"insurance that has your back\" but apparently there's no plans for someone who's pregnant with type one diabetes. Yeah, totally has my back on the condition that I'm healthy before getting the insurance" on 2026-04-12, `MOMS38 - 1 - V3`, with 4 likes.

Two commenters go further and frame it as a legal problem rather than a product limit. "And they’re holding pre-existing conditions against you, which is illegal. Their system automatically bounced me out. Since I’m a certified application counselor for the healthcare marketplace I know these things I’ve done medical billing for 30 years plus. I wouldn’t waste my time on this page." on 2025-07-23, `B1 samar- Copy`. And "It’s illigal to deny coverage for women who are pregnant so yall need to keep that in mind with the deceitful marketing" on 2025-12-20, same ad. Marked stated, not verified. I am carrying what the commenters said, not endorsing the legal read, and this is a question for the brand and its counsel rather than for this doc.

### 3. "That's not a deductible, that's your out-of-pocket max"

**103 comments across 13 different ads**, the largest single objection by raw count in the corpus at roughly 8% of everything read. The identity is the insurance insider described above, plus a wide layer of ordinary commenters who have simply learned the terms the hard way.

"That’s your out of pocket maximum (aka: worst case scenario). Your deductible is lower. You meet your deductible for your co insurance to kick in." on 2026-03-29, `MOMS38 - 1 - V5`. "A deductible ≠ out of pocket max. You should consider yourself lucky if your OOP Max is $6,000." on 2026-03-23, `MOMS38 - 1 - V3`. "No, everything is not taken care of once your deductible is met. When you reach your deductible, then you’re out of pocket costs need to be met at coinsurance 80/20, usually." on 2026-03-31, `MOMS38 - 1 - V9`, with 2 likes. "That’s not a deductible that’s a medical maximum out of pocket. You should educate people, not misinform!!" on 2026-03-29, `MOMS38 - 1 - V5`, with 2 likes. "Please learn the difference between a deductible and a max out of pocket" on 2026-05-01, `MOMS38 - 1 - V3`.

Read this against the actual script. In `MOMS38 - 1 - V1`, the second speaker says "you need health insurance that has a zero-dollar deductible without spending thousands," after the first speaker has described what is, by the audience's own correction, an out-of-pocket maximum. The whole hook rests on a word the audience believes is being used wrong. This is the clearest example in the corpus of what the mining method calls a messaging opportunity: the customer is handing the brand more precise language than the brand is currently using.

### 4. "You'll sell my number and I'll get buried in calls"

**15 comments across 10 different ads.** Low count, but it recurs across many ads and it draws unusually high likes, which suggests agreement well beyond the people who typed it.

"Filled it out and have been getting calls everyday from all sorts of companies which are mostly India based. Also, the harassment from whomever keeps calling me about Medicare (India again). This is the ONLY form I've filled out since getting my new phone number 3 months ago so it came from this site!" on 2026-03-16, `MOMS38 - 1 - V3`, with **33 likes**, the third-most-liked comment in the corpus. "I filled this out because it literally says we won't be contacted by random agents. That's a lie. I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies." on 2025-11-28, `B1 samar- Copy`. "They just sell your info. I did the form, and immediately got multiple calls and texts from different, unrelated insurance agents." on 2025-10-06, `B2 - 10TH JUNE - Copy 16`. "Absolutely do not give them your info. You will receive calls and texts nonstop from an insane amount of reps." on 2025-09-17, `B1 samar- Copy`, with 6 likes. "Health for Moms is not a health care company. They sell your info to other companies. Within 5 min of requesting info, I had received multiple texts, phone calls, and emails from a range of companies." on 2025-08-20, `B1 samar- Copy`.

The identity behind it is the burned lead, and she is now doing unpaid negative word of mouth under live creative. Notice the shape of the objection changed over time: in 2025 it is a report from someone who did it, and by 2026 it is pre-emptive fear from someone who has not. "I don’t wanna put my information and get called by hundreds of people though.." on 2026-03-11, `MOMS38 - 1 - V8`, with 2 likes. "Is putting in my information to look at prices going to end up qith 50 million calls from health insurance people..." on 2026-04-04, `MOMS38 - 1 - V9`. This is the objection sitting closest to the click, and the brand's own site copy is quoted back at it: "It listed no selling my number to scammers but it’s been just a few hours and I’ve had multiple numbers contact me with different agency type names" on 2026-01-28, `MOMS31 - N1 - 1B`.

### 5. "This is a scam"

**45 comments across 12 different ads**, using the word directly. The identity is broad and mostly the general skeptic rather than a specific buyer. Most are one word. A few carry real detail, and the highest-liked one is a research report: on 2025-01-13 under `IMG 6`, a commenter pastes a summary of Reddit discussion concluding the brand is "generally considered not legitimate and likely a scam," citing minimal coverage, cancellation difficulty, and ACA non-compliance. That comment drew 14 likes. Marked stated, not verified: it is a commenter's summary of a third-party forum, and Reddit itself has not been pulled for this brand yet.

Worth separating the category-level use of the word from the brand-level use. Most of the 45 are aimed at health insurance in general, as in "All insurance is a scam." A smaller set is aimed squarely at this brand: "Markets to moms. Provides zero plans for moms. 🚩 Makes perfect sense." on 2025-07-29, `B1 samar- Copy`, with 15 likes.

### 6. "What about dads?"

**16 comments across 12 different ads**, one of the widest spreads relative to its size. Mostly asked by women on behalf of a husband, a son, or an ex, which is itself a persona signal about who is doing the household's insurance work. "What about the dads who need insurance, my husband has cancer and has no coverage cause he is the man in the house, make that make since!!!" on 2026-03-24, `MOMS38 - 1 - V1`, with 5 likes and 5 replies. "My son is a single parent with twins. He has full and sole custody. Can he do this?" on 2026-04-02, `MOMS38 - 1 - V2`. "With income restrictions? Also I'm a mom but I carry the insurance for my whole family, including dad. Can he get on this magical plan?" on 2026-04-23, `MOMS38 - 1 - V2`. And one from the man himself, on 2026-04-04, `MOMS38 - 1 - V9`: "What about dads 🙁 some of us are permanently physically fucked up for the rest of our lives from taking care of our households... I am the one racking up medical debt for my family 😢 makes me feel like a pile of shit."

### 7. "My kids are grown, so am I still a mom to you?"

**16 comments across 7 ads.** A genuine eligibility question, not a complaint, and it is asked politely, which is rare in this corpus. "What if your kids are over 18, do I still qualify as a Mom?" on 2026-04-29, `MOMS38 - 1 - V1`. "What about moms with adult children or children in college?" on 2026-04-21, same ad. "What if I'm a mom, but my son is in college 🤔 i pay more $ to take care of him now than ever before ijs" on 2026-03-28, `MOMS38 - 1 - V9`, with 2 likes. "OK, this is great for mom's of young children. What about the rest of us? ... What about those of us whose children are grown and moved out of the house now? My deductible used to be reasonable, now it's almost $7000 a year." on 2026-04-26, `MOMS38 - 1 - V2`, with 2 likes.

My read, marked inferred: the word "mom" is doing double duty in the creative. It is meant as an identity and it is being heard as an eligibility rule. That confusion generates questions the brand never answers on the thread.

### 8. "This is AI and I don't trust it"

**32 comments across 7 ads, but 25 of them sit on one ad**, `B1 samar- Copy`, between 2025-07-20 and 2026-04-05. This is the clearest case in the corpus where era tagging matters: it is a 2025 objection tied to one AI-presented creative, not a live one. Only 4 comments carry it in 2026, and the newest is 2026-04-05.

"Please dont use AI instead of actors. AI advertizing use in spite of actors goes against the morals that health for moms promotes" on 2025-07-20. "This is the problem with AI online commercials. If you are using a fake person for your testimonial, it unintentionally sends a message to people that no real actual person would say this about your service. I think it's always better to have a real person. Especially with something that is famous for being a scam, like health insurance." on 2025-07-25. "AI video. Watch her lashes morph" on 2025-07-21, with 2 likes. "If anyone ever pays attention, all the women voices for A.I. are exactly the same" on 2025-07-29, with 9 likes. And the caption error that fed it: "Why are the words saying Medicare instead of what she is saying which is Medicaid...two different insurances" on 2025-07-20, with 13 likes.

One 2026 sighting is worth carrying because it lands on live creative: "Creepy AI blonde lady ruins the ad tbh" on 2026-04-05, `MOMS38 - 1 - V2`.

### 9. "My state isn't on the list, so why am I even seeing this?"

19 comments across 8 ads. Still small next to the objections above, but pointed, because the state list is the account's central creative device and the brand's own objection list names it as a deliberate open loop meant to compel the click. In the comments it sometimes fires backward. "I didn't see my state... So why am I getting this ad?" on 2026-04-07, `MOMS38 - 1 - V10`. "Why the hell is this ad showing if they dont offer this in Oregon or ANY of the surrounding states??" on 2026-03-16, `MOMS38 - 1 - V2`. "Why is this being shown in IL if it’s not on the list???😭🤦🏼‍♀️" on 2026-09-02, `moms-53 3`. "Ofc Georgia ain’t on there 🤣" on 2026-08-29, same ad. "Of course PA isn’t on there. They hate us." on 2026-03-20, `MOMS38 - 1 - V2`. And one that reads the list as proof of a lie: "Ha… “in these states” proceeds to list all 50 states… scam" on 2026-03-26, `MOMS38 - 1 - V2`.

### 10. "Don't buy insurance at all"

33 comments across 10 ads. Covered under the anti-category identity above. It belongs on the objection list because it is the counter-offer the audience makes back to the ad, and because the ad's own "insurance is a scam" hook is what opens the door to it.

## Moments of recognition

This is the thinnest section in the doc, and the thinness is itself the finding. Across 1,322 comments I found roughly 12 clear recognitions, under 1%. For a source this large, that is very low, and it says the creative is generating argument rather than identification. The emotional-delivery method predicts exactly this: high-intensity negative creative narrows attention and suppresses the reflective processing that identification requires.

What matters more is where the recognitions cluster. Almost all of them sit on one creative family, `MOMS38 - 2`, the skit where one woman plays both a frustrated mom and a dismissive insurance rep who denies a claim because it "happened on a Tuesday" and because the provider was "in a different hallway."

"“It’s out of network”  “But it’s in the same building!”  “In a different hallway”  🤣🤣🤣🤣🤣 whoever came up with this ad deserves a raise!! Love this!" on 2026-04-03, `MOMS38 - 2 - V1`, with 4 likes. "TRUTH! A SAD TRUTH." on 2026-04-06, same ad. "I’m not laughing but that was her best video yet!" on 2026-04-11, same ad. "Absolutely accurate" on 2026-03-31 and "Pretty accurate!!" on 2026-04-07, both `MOMS38 - 2 - V3`. "Accurate!" on 2026-03-23 and "I swear this is true !! lol" on 2026-03-18, both `MOMS38 - 2 - V4`. "Had a similar conversation recently with my soon to be former insurance company." on 2026-03-23, `MOMS38 - 2 - V4`. "At the Mayo Clinic for my husband right now. Absolutely dealing with this." on 2026-04-06, `MOMS38 - 2 - V1`.

The identity these recognitions hand over, marked inferred: a woman who has recently spent hours on the phone losing an argument with an insurance company, and who wants that experience named out loud before anyone sells her anything. That is a different emotional doorway than the deductible number. The skit lets her laugh, which is low-intensity and positive, the quadrant the emotional-delivery method says most brands underinvest in and the one that builds identification.

Two more recognitions are worth pulling out separately, because they are aimed at the agent rather than the ad, and they are the only two moments in 1,322 comments where someone reports a good experience with this brand's actual service.

"Best advice I have gotten from an insurance agent! She didn’t have anything that fit but pointed me in the right direction!" on 2026-04-17, `Moms Nahuel WV#1 - V9`, with 2 likes. And "I was connected to a very helpful agent. They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful." on 2026-04-01, `MOMS38 - 1 - V1`.

Both people were told no and both left praise anyway. That is unusual enough to name. The brand positions its partner agents as "Mom BFFs" who are friendly and pressure-free, and these two comments are the only public evidence in the corpus that the positioning is landing. Confidence: thin, on two comments out of 1,322, but they are the only positive service signal that exists anywhere for this brand right now, so they should not be dropped.

A separate behavior that is not recognition but sits near it: 49 comments consisting of the single word "Help" or "help," all of them on one ad, `Moms43 - 4 - V3`, between 2026-05 and 2026-09. Marked data-limited on meaning. It reads like people responding to a prompt or trying to trigger a reply, and without the ad's caption comment or a moderation log I cannot tell whether it is inbound demand or an artifact.

## Targeted-versus-showed-up gap

The targeted side, read from the creative and from Meta delivery rather than from names. The `MOMS38 - 1` family and its siblings all speak the same line: "you can only get that if you are a mom and you live in one of these states." The creator mix across the 20 ads read is almost entirely white women in their late 20s to early 40s filming themselves at home, with one Black woman in her late 30s or early 40s in `MOMS38 - 1 - V9`. Delivery on those same eight ads ran 97% female, 72.2% aged 25 to 44, 99.7% mobile. The brand's five stated ICPs are Jen the family safety net, Danielle the overwhelmed planner at 38, Marissa the single mom at 33, Courtney the self-employed mom at 36, and Nicole the second-chapter mom at 41 with a seven-month-old.

The showed-up side diverges in seven ways. I am naming both sides and leaving them unresolved, because the synthesis has to weigh them against the ad-account read and against actual-buyer sources that do not exist yet for this brand.

**One. Built for the shopper, showed up the captive.** The creative assumes the viewer can choose a plan. A recurring group says her employer chooses for her. Targeted: a mom comparing options. Showed up: a mom with one option and a payroll deduction.

**Two. Built for moms, disqualifies mothers-in-progress.** Targeted: the mom, including ICP Nicole by the brand's own description. Showed up: 42 comments across 15 ads from women told they are ineligible for being pregnant or planning to be.

**Three. Built for cost relief, showed up medical necessity.** Targeted: a household trying to save 30%. Showed up: families with cancer, MS, autoimmune disease, a child in the NICU, and prescription costs in the thousands per fill, who are exactly the households medical underwriting screens out.

**Four. Built for the layperson, showed up the professional.** Targeted: a mom who does not understand her plan. Showed up: 103 comments across 13 ads from people who understand it better than the script does, including self-identified brokers, agents and medical billers.

**Five. Built for prospects, showed up competitors.** 39 comments across 10 ads are rival agents and brokers pitching Direct Primary Care, health shares, and their own books of business under the brand's paid creative.

**Six. Built for women, showed up men and the women advocating for them.** 16 comments across 12 ads ask about dads, husbands, sons and stay-at-home fathers.

**Seven. Built for moms with kids at home, showed up the after-stage.** 16 comments across 7 ads come from women whose children are grown, in college, or never existed, plus a 64-year-old asking about coverage for herself alone.

One caution on all seven, marked plainly. A gap in a comment section is not proof of a gap in the buyer base. The persona method warns against treating the served audience as the actual buyer, and here there is no actual-buyer source at all to check against. Every one of these gaps is a hypothesis for the synthesis to test, not a finding to act on.

## Behavioral-signal states observed

These are states layered on a person, not identities, and the persona method is clear that promoting a behavior or a life stage into a persona is the most common failure in this work. Each of these cuts across every identity above.

**Deductible-reset dread.** A calendar-driven state that spikes in December and January. "After my deductible, I pay 25% of all costs 'til I meet my max out of pocket, and then everything is finally taken care. And then it's the end of the year, and we start all over. I literally hate NYE for this reason!" on 2026-04-04, `MOMS38 - 1 - V3`, with 6 likes. "Mine is $8,000 and I hit it in the beginning of march 🤣😭" on 2026-03-26, `MOMS38 - 1 - V8`, with 2 likes.

**Open-enrollment lockout.** She wants to act and is told to wait. "yes there is. You have to sign up during open enrollment, not whenever you need it." on 2026-04-25, `MOMS38 - 1 - V3`. "Does this work in Louisiana? Because they wouldnt let me apply for good insurance here until November." on 2026-05-27, `Moms43 - 4 - V3`. The brand's own objection list names this as the timing objection, so this one corroborates something the brand already knows.

**An acute medical event, already scheduled.** The sharpest Trigger state in the corpus, and the highest intent. "This is what I'm afraid of. Just found out I desperately need a hysterectomy. My husband is looking into insurance for me so that I can get it done." on 2026-04-14, `MOMS38 - 1 - V2`, with 1 like. "Our deductible is $10,500 😭 And I have to have surgery in June" on 2026-04-02, `MOMS38 - 1 - V10`. "how can I get that because I pay $1000 a month for my insurance and tomorrow I have surgery" on 2026-05-04, `MOMS39 - 2 - V2`.

**A benefits change in the household.** "I’m heading in to work so couldn’t really look at this. And with bring a new rehiring I’m able to enroll into insurance. Not sure if I want to." on 2026-04-30, `MOMS38 - 1 - V2`. "we own our own business. It’s through healthcare.gov" on 2026-04-08, `MOMS38 - 1 - V1`.

**Phone-call avoidance.** A friction state that maps directly onto a lead-gen model built on a call. "Id be way more interested if I didn't have to talk on the phone immediately tbh. It's super difficult for me to process information without reading and I get so flustered on the phone" on 2025-02-15, `IMG 6`. "Do you have to talk to them on the phone? Or can they send a quote in email?" on 2026-03-10, `OMC - C11 - 2b`. "Just give some pricing without making people sign up 🙄" on 2026-03-15, `MOMS38 - 1 - V1`, with 3 likes. "Really wish you could see plans without adding all your personal information to get even more telemarketing calls than we already do." on 2026-03-13, `OMC - C11 - 2b`.

**Post-form burn.** Already in the funnel, already unhappy, now warning strangers. Covered under objection four above. It is a state rather than an identity because it can attach to any of the personas here.

**Geographic exclusion.** She was served the ad in a state the offer does not cover, so the state list turns from a hook into a rejection.

## Corroboration and noise

**What was read.** 1,322 comments, the full corpus, dated 2025-01-08 to 2026-09-03. 112 distinct ad IDs, 79 distinct ad names. 1,023 top-level comments and 299 replies. Full creative pulled and read on 20 ads carrying 997 of the 1,322 comments, or 75%, so three quarters of everything quoted here sits under an ad whose script, visuals, creator and hook I inspected directly.

**Signals I would trust enough to hand forward.** Four clear the bar of appearing on many different ads and across many months, which is the only kind of durability this single-source corpus can demonstrate.

The pregnancy exclusion, at 42 comments across 15 ads over 14 months. The pre-existing-condition denial, at 55 comments across 17 ads and still landing three days ago. The deductible-versus-out-of-pocket correction, at 103 comments across 13 ads. And the insured-but-still-broke identity, at 160 self-disclosed dollar figures across 17 ads. All four are marked **mixed confidence**, not verified, for the reason stated at the top: no buyer source exists for this brand to check them against.

**Signals I would treat as reaction-noise until something corroborates them.** The AI backlash, because 25 of its 32 comments sit on one ad and it has gone quiet since April 2026. The "Help" comments, because all 49 sit on one ad and their meaning is unreadable. The political blame comments, because they are about American health policy rather than about this brand, this product, or this buyer. The scam accusations, because most of the 45 are aimed at the insurance category rather than at Health For Moms. And every single-thread complaint, of which there are many, since the review-mining method is right that one striking comment is a candidate and never a pattern.

**Where the corpus is skewed, stated plainly.** 60% of comments sit on the `MOMS38 - 1` family and 38% were posted in April 2026. That means the corpus is closer to a deep read of one campaign moment than an even read of the account's history. Any rate quoted here is a rate within that skew, not a rate across the brand's whole advertising.

**Brand-self echo check.** The mining method asks whether brand language is coming back dressed as customer language. It is, in one specific place, and it is worth flagging. The phrase "make that make sense" appears in commenter language, and it is also the shape of the brand's own tweet-style creative. The ad `MOMS39 - 2 - V2` overlays a tweet reading "My deductible is $6000... Make that make sense...." and commenters then write "Health care for moms but you don't qualify if your pregnant? Make that make sense." and "make that make since!!!" The brand handed the audience a sentence pattern and the audience turned it around on the brand. That is not customer language for the voice bank. It is echo, and it should be tagged low confidence wherever it surfaces downstream.

**What no amount of reading here can produce.** Who actually bought. The real share of any identity in the buyer base. Whether any commenter became one of the 4,336 leads. Whether any objection here costs a single lead. Those need the post-purchase survey the brand does not have, or a join between comments and leads that Parker does not hold.

## Open loops

**1. The brand's name is the setup for its widest objection.**

Health For Moms disqualifies pregnant women and women planning a pregnancy, and 42 comments across 15 ads over 14 months say so in public, usually by quoting the brand's own name back at it. The brand's stated objection list does not contain this objection at all.

Pull: **Tension.** Two sources cannot both be true as stated. The brand context document says the objections are legitimacy, sales pressure, time, state coverage and timing, and the brand's own comment sections say the biggest objection is that the product excludes the mothers the name promises.

Question: What share of the people who start the qualification flow are screened out?

Why it matters: if the pregnancy and pre-existing screens are turning away a large share of the traffic the ads pay for, then the fix that moves the most is upstream of creative, in who the ads invite. If the share is small, the objection is loud but cheap and the answer is a line of copy.

Territory: **Product.** Only the brand can answer this one, since it needs the funnel's own screen-out data.

**2. The ad speaks to a shopper and the comments answer as captives.**

The creative assumes the viewer can switch plans. A recurring set of commenters says her employer picks the plan, she has one option, and she never considered that declining employer coverage was allowed. One commenter had to explain that in the replies because the brand never does.

Pull: **Surprise.** Given a creative built entirely on switching, the number of people saying they cannot switch is not what the setup would predict.

Question: How many of the leads this account produces already hold employer coverage?

Why it matters: it decides whether the next round of creative sells a better plan or sells permission to leave the plan she already has, and those are completely different scripts.

Territory: **Personas.** Only the brand can answer this, since it needs lead-level data the comment corpus cannot see.

**3. The audience keeps correcting the hook's central word.**

103 comments across 13 ads say the ad describes an out-of-pocket maximum, not a deductible. Self-identified brokers, agents and medical billers are among them. This sits on the account's highest-spend creative.

Pull: **Pattern.** The same correction keeps appearing across independent ads, months and commenters, which is the shape of something real rather than a few pedants.

Question: What happens to lead volume and cost per lead when the same offer is stated in the words the audience says are correct?

Why it matters: the brand is currently trading technical accuracy for a punchier hook, and nobody knows the price of that trade. If accuracy holds the hook and kills the correction thread, that is free credibility.

Territory: **Messaging.**

**4. Rival agents are working the comment section of the account's best ad.**

39 comments across 10 ads pitch competing offers, including one operator who posted the same Direct Primary Care and health-share script at least nine times under `MOMS38 - 1 - V1` on a single day. That ad has spent $54,173 lifetime.

Pull: **Gap.** There is obvious activity here and nothing appears to have been done about it.

Question: How much of the interest these ads create is being picked up by other agents in the comments before it reaches the brand's own funnel?

Why it matters: it is the cheapest possible leak to plug, and if it is meaningful, comment moderation becomes a performance lever rather than a housekeeping chore.

Territory: **Product.** This is a buyer-journey leak, and answering it needs the brand's own view of where its traffic goes.

**5. The one format that earns agreement is not the one getting the spend.**

Nearly every recognition in 1,322 comments sits on the `MOMS38 - 2` skit family, where a woman plays both the mom and the insurance rep denying a claim because it happened on a Tuesday. That family has spent about $3,433 lifetime across its two read variants. The deductible-vent family that earns argument has spent over $94,000.

Pull: **Resonance.** The skit is the only creative in the corpus that made people say it was about them instead of arguing with it, and the reason it works is worth understanding.

Question: Why does the denial skit earn agreement where the deductible complaint earns argument?

Why it matters: if the answer is that the skit names an experience she has lived rather than a number she can dispute, that reshapes the whole creative approach and not just one ad.

Territory: **Messaging.**

**6. The loudest pain in the corpus belongs to the person the product cannot cover.**

Families with cancer, MS, autoimmune disease and NICU stays write the longest and most emotional comments, and 55 comments across 17 ads say medical underwriting screens exactly those families out.

Pull: **Tension.** The emotional center of the audience and the eligible center of the product are two different people, and both cannot lead the creative.

Question: Who should the creative be built around when the most intense pain in the audience belongs to someone the product cannot serve?

Why it matters: it is the difference between creative that harvests attention it cannot convert and creative that finds the household the product actually fits, which is healthy, insurable, and still overpaying.

Territory: **Personas.**

**7. People who are not moms keep asking to be let in.**

16 comments across 12 ads ask about dads, husbands and sons. 16 across 7 ads come from women whose children are grown or who have none. Most are asked as sincere eligibility questions, not as complaints.

Pull: **Curiosity.** A brand whose entire creative device is a single word, "mom," keeps getting asked what that word actually means, and the answer is never given on the thread.

Question: Who besides mothers is being served these ads and asking whether they qualify?

Why it matters: if the "mom" framing is a marketing wrapper on a product anyone can buy, the brand is turning away demand with a word. If it is a real eligibility rule, the creative should say so and stop generating the question.

Territory: **Personas.**

**8. The only two happy comments about this brand are about a person, not a plan.**

In 1,322 comments, exactly two report a good experience, and both describe an agent who could not help them and was thanked anyway. One says "She didn't have anything that fit but pointed me in the right direction!" The other says "They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful."

Pull: **Resonance.** Being told no and leaving praise is not normal, and whatever produced it is worth knowing.

Question: What are the partner agents doing on those calls that earns thanks even when there is nothing to sell?

Why it matters: the brand's whole positioning rests on agents who feel like "Mom BFFs," and these are the only two public data points showing whether that is true. If the answer is repeatable, it is the strongest and least-used proof asset the brand has.

Territory: **Creators and talent.** Only the brand can answer this, since it needs call recordings or agent debriefs.

**9. The AI backlash may have been solved or may just be sleeping.**

32 comments call the creative AI-generated or fake, but 25 of them sit on one ad, `B1 samar- Copy`, and the objection has been near-silent since April 2026 apart from "Creepy AI blonde lady ruins the ad tbh" on live creative.

Pull: **Surprise.** An objection this sharp in 2025 going almost completely quiet in 2026 is not what a steady trend would look like, and the drop needs explaining before anyone assumes it is fixed.

Question: What specifically does this audience notice and reject in AI-presented creative?

Why it matters: the account is still running AI-assisted creative, so knowing whether the audience stopped caring or the brand stopped triggering it decides how much AI work is safe to scale.

Territory: **Creators and talent.**
