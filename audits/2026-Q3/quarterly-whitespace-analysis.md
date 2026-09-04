---
brand: health-for-moms
doc: quarterly-whitespace-analysis
quarter: 2026-Q3
generated_on: 2026-09-04
refresh_by: 2026-12-03
data_sources_read: [Parker MCP search_customer_reviews_sql (zero rows, verified live 2026-09-04), Parker MCP semantic_search_post_purchase_survey (zero responses, verified live 2026-09-04), Parker MCP search_facebook_ads_sql lifetime across the full Meta account HealthForMoms act 484897827497337 (1557 ad-name groups, $743218.09), Parker MCP search_facebook_ad_comments_sql (1322-comment corpus, two independent keyword counts run 2026-09-04), Parker MCP get_brand_persona (brand context document, ~50KB), running-notes/missing-context.md, running-notes/brand-rules.md, running-notes/success-definition.md, audits/2026-Q3/90-day-diversity-audit.md, audits/2026-Q3/90-day-creative-strategy-audit.md, audits/2026-09/monthly-organic-tiktok-audit.md, sub-context-docs/competitive-landscape.md, sub-context-docs/customer-journey-and-persona-discovery.md, sub-context-docs/website-and-product-audit.md, sub-context-docs/reputation-analysis.md, sub-context-docs/category-and-market-research.md, personas/voice-of-customer/voc-objection.md, source-pulls/ad-comments.md, prompts-run-log/2026-09-03-full-buildout.md]
review_personas_surfaced: [the insured mom who just found out the number, the employer-plan captive, the self-employed mom in the income gap, the chronic-condition family, the expecting and brand-new mom, the mom whose kids are grown, the mom leaving the category]
spend_personas_observed: [the deductible-shock mom, the peaceful-outcome mom, the employer-plan switcher, the claim-fight mom, the silent-clinician audience, the phone-call skit audience, the self-employed mom, the single mom, the income-gap mom, the expecting mom at zero]
data_limitations:
  - "There is no customer review corpus. A live unfiltered search_customer_reviews_sql call on 2026-09-04 returned totalReviews 0. Post-purchase surveys returned totalResponsesForBrand 0 on the same day, with the collection existing and empty. Both were checked directly rather than trusted from the notes. Section two is therefore built on the substitution rule the team gave Parker in Slack on 2026-09-03: Facebook ad comments, plus the category TikTok library, plus competitor and category signal. Nothing below is this brand's own review corpus and it must never be relayed as one."
  - "The persona method ranks post-purchase survey data first and public comments near the bottom. This brand holds only the bottom tier and only one source type. So the honest confidence ceiling on every persona below is mixed, never verified, no matter how many times a phrase recurs. Recurrence inside one noisy source is still one source."
  - "There is no personas-profile.md yet. Phase 1C has not reached the synthesis step. The five named ICPs used as a check in section four are stated brand input from the brand context document, not validated buyer profiles."
  - "There is no prior quarter whitespace analysis. This is the t0 baseline. There are no prior recommendations to score and no prior loops to close, so every trajectory claim below is built from a direct lifetime pull rather than from an earlier strategist read."
  - "Parker holds no persona tag for this account. brand_tags came back empty on the lifetime tag summary. Every per-persona spend figure in section three was built by hand from creative reads and keyword cuts across the lifetime library, and the classified share is named: $350435.98 of $743218.09, or 47.2 percent of lifetime spend, sits in a lane this doc can name. The rest sits in creative that addresses moms as one undifferentiated group."
  - "Lead quality is invisible to Parker. It lives with the partner insurance agencies. Every efficiency figure here clears gate one of the brand's own two-gate winner definition and says nothing about gate two."
  - "Northbeam is not connected. All attribution is Meta-reported on the account default window. ROAS is not used anywhere; the account has zero purchase events by design."
  - "No competitors are tracked. A live search_competitor_facebook_ads call returned totalCount 0 on 2026-09-04, per competitive-landscape.md. Competitive whitespace below is reasoned from the alternatives customers name themselves, not from any rival ad library."
  - "The comment corpus is lopsided. 795 of 1322 comments, 60.1 percent, sit on the MOMS38 - 1 creative family, and 846 of 1322, 64.0 percent, fall in March and April 2026. Ad spread is carried on every count for exactly this reason."
---

# Quarterly whitespace analysis — Health For Moms — 2026-Q3

## Executive summary

The largest under-invested proven buyer this account has is the mom who already has insurance through her job and does not know she is allowed to leave it. Two static ads speak to her directly. `B1 - Copy 7` carries the headline "Left my big insurance company for a mom-focused one. 24% cheaper and I choose my own doctor 😌" and `B1 samar- Copy 1` carries "Didn't know I could ditch my job's health plan… until I did." Together those two ads spent $30,845.69 lifetime and produced 2,580 leads at an $11.96 cost per lead. That is the cheapest lead at real scale anywhere in this account, against a lifetime blended $18.78 and a trailing-quarter $22.67. **Verified** from a direct adIds lookup on 2026-09-04. Neither ad has run in months. Meanwhile the same woman is in the comment section saying she cannot act: "nope. My job picks the plan that they offer," posted 2026-03-30 on `MOMS38 - 1 - V3`, and "Mine is $9,200/individual, $17,500/family and that's the only plan my employer offers 😬," posted 2026-03-27 on `MOMS38 - 1 - V2`. The brand proved it can buy this lead for twelve dollars and then stopped buying it.

Underneath that sits a bigger correction, and it changes what the whole quarter means. This audit was briefed on the idea that the account has never run a static ad. That is true of the last 90 days and false of the account's life. A lifetime pull filtered to image creative returns **308 ad-name groups, $168,907.73 of spend, 13,735 leads and a $12.30 cost per lead**. **Verified**, pulled 2026-09-04. Video carries the other $574,310.36 and 25,834 leads at $22.23. So statics took 22.7 percent of the money and delivered 34.7 percent of the leads, at a cost per lead 44.7 percent below video. This is not an untested modality the brand should try. It is a proven modality the brand switched off, and the switch is roughly the whole story of why cost per lead sat flat at $22.66 and $22.67 across two structurally different quarters while the cheap half of the account went dark.

The persona the brand is spending heavily on against the weakest buyer evidence is the mom at peace in a bedroom. Three ads carry that idea, `Moms43 - 4 - V3`, `Moms43 - 4 - V4` and `MOMS34 - N1 - 3a`, and together they spent $110,205.90 lifetime for 5,057 leads at $21.79. That is 14.8 percent of everything this account has ever spent, on a wordless montage of a woman who already has the thing the ad is selling. **Verified.** Hold against the buyer evidence and there is almost nothing there. Across 1,322 comments the source pull found roughly 12 clear moments of recognition, under 1 percent, and almost none of them sit on this creative. What that footage does produce is the account's largest single comment thread and its sharpest complaints. Nobody sees herself in it. She sees a woman with nicer bedding.

The persona that has emerged this quarter and did not exist in the account before is the expecting or brand-new mom, and she arrived through the category rather than through the brand. Twelve of the nineteen relevant videos in Parker's TikTok mining library, 63.2 percent, are anchored to pregnancy, delivery costs or a baby's first year, and the category's single biggest video, a doctor calling hospitals for cash delivery prices, holds 6.2 million plays. **Verified** from the organic TikTok audit's full-depth read. Against that, a keyword search for "pregnant" across every ad name, headline, body copy, text hook, verbal hook, visual hook, angle, script and AI analysis field in this account returns **totalMatching 0**, lifetime, all ad types. **Verified** by my own pull on 2026-09-04. She is 42 comments across 15 different ads, the widest and longest-running objection in the whole corpus, and the account has never once spoken to her. That is not a simple opportunity, because the product screens her out, and section five treats it as a product question rather than a creative one.

The lead recommendation for next quarter is narrow and it is not new creative. Put budget back behind the switching static, aimed at the employer-plan mom, and give it the one line the account has never said out loud: that she is allowed to decline the plan her job offers. The evidence is the $11.96 cost per lead on ads that already exist, the 44.7 percent modality gap between statics and video, and a comment thread where a stranger has to teach her the rule the brand should be teaching her. Behind it come three more: fund the phone-call format that already produced this account's best hold rate at 24.48 percent, let the clinician the brand already filmed actually speak, and name the income gap in the words the customer uses. The last of those runs straight into the brand's non-negotiable rule against naming the Marketplace and Medicaid, and section five says exactly where that binds and what is left after it does.

## Personas from customer reviews

**Read the source line before the personas.** This brand has no reviews. I checked it live rather than trusting the note: an unfiltered `search_customer_reviews_sql` call on 2026-09-04 returned `totalReviews: 0`, and `semantic_search_post_purchase_survey` returned `totalResponsesForBrand: 0` with the collection existing and empty. **Verified.** So the substitution rule the team gave Parker in Slack on 2026-09-03 applies, in their own words: *"we don't have reviews but you can pull from competitor reviews or health insurance Reddit etc."* Every persona below is built from the brand's 1,322 Facebook and Instagram ad comments, dated 2025-01-08 to 2026-09-03, cross-checked against the category TikTok library and the category research. **Anywhere downstream, the honest sentence is "commenters under the brand's paid ads said," never "customers said."**

That ceiling is real and it applies to all seven profiles. The persona method ranks post-purchase survey data at the top of the evidence pile and public comments near the bottom, and this brand holds only the bottom rank, and only one source of it. Recurrence inside one noisy source is still one source. So no persona below rises above **mixed** confidence, and I have marked each one rather than rounding any of them up. One more shape to hold: 795 of the 1,322 comments, 60.1 percent, sit on a single creative family, and 846, 64.0 percent, fall in two months. That is why every count below carries its ad spread. Spread is the durable number here. Raw count is not.

There is one genuine advantage in this thin surface, and it is worth naming so the section is read correctly. A comment section is where doubt gets performed. People come under an insurance ad to argue, correct strangers, and warn each other. That selection bias would ruin a read of what customers love. It is close to ideal for reading who shows up and what stops them, which is most of what a whitespace audit needs.

### One. The insured mom who just found out the number

She is the dominant identity in the corpus and she is not the woman the creative was built for. **160 of 1,322 comments, 12.1 percent, spread across 17 different ads, disclose her own deductible or premium unprompted.** She is not an uninsured shopper. She already pays every month, and she is saying the plan does not do anything. Delivery on this account runs 96.1 percent female and 77.0 percent aged 25 to 44 lifetime, so the demographic frame around her is solid, though her age and income are **inferred** from how she writes rather than known.

Why she buys, or would: not to get covered, because she is covered. To stop paying for something that does not work. Watch what her own words do with a number. The ad `MOMS38 - 1 - V1` opens on a woman filming herself, annoyed, under the words "Health Insurance is a scam 🙄," saying "My deductible is $6,000." The comment section did not treat that as a pain point to be soothed. It treated it as an opening bid. "Wow only 6? Must be nice" drew 13 likes on 2026-03-27. "$6000???? Huh mine is $18000 .....where can I get the $6k" landed 2026-03-26. "6k....try 13k!" landed 2026-04-02. The most-liked comment in the entire corpus, 47 likes on 2026-03-22, is hers: *"This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family. It's insane. I have 2 members of the family with chronic diseases. This absolutely insane. I want the 1990's back."* **Verified** verbatims from the comment pull.

What almost stops her is that she does not believe the offer. "This sounds too good to be true" is the first clause of the corpus's single most-liked line. And what converts her, when anything does, is being agreed with before being sold to. The trigger moment is plain and it is the one the account is already built on: the day she opened the bill and found out the number. In the emotional model that puts her in Trigger, where a need has just become conscious, while nearly every funded script in this account is written for Evaluation, where a specific plan is being compared. That mismatch is visible in the behavior itself. She answers the ad's number instead of the ad's offer. **Inferred**, confidence mixed.

### Two. The employer-plan captive

She sits inside the group above and she is the one who quietly breaks the ad's premise. Every funded script in this account assumes she can choose a plan. She says, repeatedly and calmly, that she cannot. This is a smaller and much sharper identity than the one above, and it is the highest-value persona in this document.

Who she is, **inferred** from what she writes: a working or partnered mother whose coverage comes through a job, hers or her husband's, with a deductible she can quote to the dollar and no visible way out. Her verbatims are flat rather than angry. "nope. My job picks the plan that they offer," 2026-03-30 on `MOMS38 - 1 - V3`. "Mine is $6k per person too but since it's thru my job I don't really have a choice," 2026-03-17 on `MOMS39 - 2 - V2`. "The hospital I work for only provides the option to use their insurance company. Last year it was over 18k," 2026-03-28 on `MOMS38 - 1 - V3`. "Mine is $9,200/individual, $17,500/family and that's the only plan my employer offers 😬," 2026-03-27 on `MOMS38 - 1 - V2`. And the one that names the trap from inside the industry, 2026-05-03: "Yep…I work for an insurance company and they now outsource our insurance and our deductible is 4k with no copays." **Verified** verbatims.

What almost stops her is a belief, not a price. She does not know that declining employer coverage is allowed. The proof of that is who tells her. Not the brand. A stranger in the replies, on 2026-05-05 under `MOMS38 - 1 - V2`: *"if it's an employer insurance, you don't have to sign up with that employer insurance you can decline the coverage and go out and find your own insurance carrier."* **Verified.** The brand's own context document already names employer coverage as *"the most common 'competitor' — the default option families already have."* **Stated.** So the brand knows the alternative and has not built the one sentence that unlocks it.

Her trigger is a benefits change. Open enrollment arriving, a plan getting worse, a company being acquired, a rehire. "I'm heading in to work so couldn't really look at this. And with bring a new rehiring I'm able to enroll into insurance. Not sure if I want to," 2026-04-30. **Verified.** Confidence on this persona is mixed, and the reason it still leads the audit is that it is the one identity here with hard spend evidence behind it, covered in section three.

### Three. The self-employed mom in the income gap

She is the one identity in this corpus that a stated brand ICP and the comment evidence both point at, which makes her the best-corroborated persona in the document even though she is small by volume. The brand calls her Courtney and describes her as 36, running her own business outside Denver, priced out of her husband's employer plan at an extra $480 a month, on a short-term plan she found by Googling at midnight and is about 60 percent sure covers anything. **Stated**, brand context Section 2.

The corpus narrates her from the inside. "Well you being a teacher is why. I'm self employed and can't find anything that doesn't have at least $5k deductible," 2026-04-02 on `MOMS39 - 2 - V2`, with 7 likes. "Literally why I refuse to.get insurance as a self-employed person," 2026-03-22, same ad. "There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy," 2025-08-09 on `B1 samar- Copy`. And the clearest statement of the gate itself, 2025-08-03: *"I don't make very much, just more than medicaid allows (which is far below poverty level)."* **Verified** verbatims. Her category twin says the same thing on TikTok in the same register: @yolys.world, 14,700 views, opens *"If you're pregnant and you're looking for insurance and you didn't qualify for Medicaid like me, listen up,"* and explains that her household income disqualified her.

Why she buys: she is not looking for cheap, she is looking for a number she can plan against, because every dollar in a self-employed household already has a job. What almost stops her is that she reads everything before she calls anyone, and this brand gives her nothing to read. The brand's own context says she *"doesn't want to be sold to"* and *"will read every FAQ on a website before she picks up the phone."* **Stated.** Her trigger is a good month, or finishing her taxes, or any moment that proves the business is real enough to insure. Confidence mixed, and unusually well corroborated for a persona in a corpus this thin.

### Four. The chronic-condition family

Smallest by volume, largest by emotional intensity, and the persona method is explicit that those two rankings must be kept apart rather than flattened. Roughly 20 comments carry her voice directly, while 55 comments across 17 ads name a pre-existing condition denial, and diabetes alone appears 11 times. She is not describing a budget preference. She is describing a medical reality.

"Add having a son fighting cancer for 7+ years," 2026-04-12. "My daughters 1 January claim was $364,000. She had half a million in claims over a week," 2026-04-20. "girl, we pay $2,200 a month and its a battle for them to cover anything. I have MS so I NEED to be covered for my treatments," 2026-03-23, with 4 likes. And the one that shows what a deductible actually means in her house, 2026-03-31: *"This year it took 35 days to hit our 8k OOP. Next year it could take as few as 1 depending on how prescriptions hit. Child is on 1 med that is $3600 per fill. I am on a combo of meds that are $2,600, 1,800, and $3,200."* **Verified** verbatims.

What stops her is not an objection and cannot be reframed away. It is a gate. These are medically underwritten private plans, and the funnel screens her out. "Was so excited about this but as soon as i said diabetic i didnt qualify," 2025-07-07. "Preexisting health condition of cancer disqualified me." **Verified.** She is in this document not as an opportunity but as a cost. The advertising recruits the loudest, most motivated person in the category and then the product tells her no, and she goes back to the comment section and says so in front of everyone else. Confidence: strong on the intensity, thin on the volume, and the read that she is unservable is **inferred** from the denial pattern rather than stated by the brand.

### Five. The expecting or brand-new mom

She has the widest spread of any single objection in the corpus: **42 comments across 15 different ads, running 2025-07-01 to 2026-06-09.** Fourteen months, every creative refresh, no movement. She is also, by the brand's own description, ICP Nicole, 41 and seven months postpartum with her first baby. **Stated.** The creative recruits her by name and the product excludes her, and she uses the brand's name as the setup for the complaint.

"your insurance says im not eligible because im pregnant 😂 huh.. so much for being for Moms 😂," 2026-04-01 with 7 likes. "Says this is for moms….but you can't get a plan if you're pregnant or planning to become pregnant… 🤔," 2026-05-19 with 4 likes. "Health for Moms, but only if your babies are out of the womb. I was denied for being pregnant. Scam," 2026-02-03. "Marketing towards mothers while not covering pregnancy is a disgusting tactic," 2025-11-23. And the one that shows the screen is forward-looking, 2026-02-08: *"One question literally asks if you are pregnant or planning to be pregnant?... I'm not pregnant but I'm planning to be. So I picked yes pregnant and it says there are no plans."* **Verified** verbatims.

Her trigger is the price of having a baby, and that is where the category lives. **Twelve of the nineteen relevant videos in the brand's TikTok mining library, 63.2 percent, are built around pregnancy, delivery costs or a baby's first year.** The library's biggest video by a factor of seven is Dr. Ashlee Hendry cold-calling hospitals for cash delivery prices, 6.2 million plays, 208,000 shares. **Verified** from the full-depth library read. Against that, the brand's lifetime ad library returns zero matches for "pregnant" on any field. She is the loudest buyer in the category and the emptiest lane in the account, and she is the one persona in this document where the right move may not be a creative move at all. Confidence mixed on the identity, strong on the absence.

### Six. The mom whose kids are grown

**16 comments across 7 ads**, and what makes her worth a profile is the tone. She is not complaining. She is asking a polite eligibility question that nobody answers. "What if your kids are over 18, do I still qualify as a Mom?" 2026-04-29. "What about moms with adult children or children in college?" 2026-04-21. "What if I'm a mom, but my son is in college 🤔 i pay more $ to take care of him now than ever before ijs," 2026-03-28 with 2 likes. And the fullest version, 2026-04-26 with 2 likes: *"OK, this is great for mom's of young children. What about the rest of us? ... What about those of us whose children are grown and moved out of the house now? My deductible used to be reasonable, now it's almost $7000 a year."* **Verified** verbatims.

The read, **inferred**: the word "mom" is doing two jobs in this creative. The brand means it as an identity. She hears it as an eligibility rule, and she assumes she has aged out. Her economics say the opposite. A woman in her late forties with a $7,000 deductible and a kid in college is closer to the product's actual buyer than a 28-year-old with a newborn, because she is healthy enough to pass underwriting and expensive enough to care.

What almost stops her is that she thinks the ad is not for her, and nothing in the account tells her otherwise. Her trigger is watching a deductible climb after the kids left. Confidence mixed. There is a live spend signal behind her, covered in section three: the one ad family that reaches her puts 40.2 percent of its money on women 45 and over, against 21.2 percent for the account as a whole, and it got there by accident.

### Seven. The mom leaving the category

**33 comments across 10 ads** argue that the right answer is to drop insurance and pay cash. She will not buy this product. She is in this section because she is persuasive, because she is growing, and because the brand's own best hook recruits her.

"I stopped paying for health insurance. Its actually WAY cheaper to not have insurance. We have saved thousands and that includes xrays treatments routine visits," 2026-03-21. "I would rather have no insurance you would get better self-pay rates then you do with 'having coverage,'" 2026-03-26, with 14 likes. **Verified.** The category feed says the same thing at enormous scale. A former nurse explaining her family of four has been uninsured for three years holds 872,100 plays. A phone video panning a hospital bill from $55,623.00 charged down to $1,404.00 paid cash holds 213,100 plays. **Verified** from the TikTok library.

Here is why she belongs in a whitespace audit rather than a footnote. The account's most-watched creative ever opens with the words "Health Insurance is a scam 🙄." That ad holds 17.12 percent of viewers lifetime, against 3.81 percent on the current top spender. **Verified**, lifetime pull 2026-09-04. It works because it agrees with her. And then it asks her to buy insurance. The brand is paying to win an argument whose natural conclusion is the competitor with no ad account, no brand and no sales rep. **Inferred**, confidence mixed.

### What is not a persona here, and why it matters

Several loud things in this corpus look like personas and are not, and promoting them would be the exact failure the persona method warns about. **Behavioral overlays** that cut across every identity above: the December deductible reset, a procedure already on the calendar, open-enrollment lockout, phone-call avoidance, the burn after submitting the form, and geographic exclusion when her state is not on the list. Every one of those can sit on any buyer here, so each informs offer, timing and landing-page work, never who to target.

Two more are noise rather than buyers, and both are expensive. **The insurance insider**, 103 comments across 13 ads correcting the ad's use of the word deductible, including self-identified brokers and medical billers. That is not an audience, it is a credibility leak sitting on the account's highest-spend creative. **The rival agent**, 39 comments across 10 ads pitching a competing offer under the brand's own paid creative, 17 of them on `MOMS38 - 1 - V1` alone. And the **politically primed reactor**, 54 comments across 14 ads, is reaction rather than persona signal, though it does tell you the emotional state this creative lands in, which is high-intensity negative and the worst possible ground for identification.

## Where the money is going

**How the persona split was built, because Parker has no persona tag for this account.** The lifetime tag summary returns `brand_tags: {}` and no persona category. **Verified.** So I built the lanes below by hand from creative reads and keyword cuts across the full lifetime library, then checked each lane for overlap by ad name. The classified total is **$350,435.98 of $743,218.09, or 47.2 percent of lifetime spend.** The remaining 52.8 percent sits in creative that addresses moms as one undifferentiated group and cannot honestly be assigned to a persona. That number is the denominator for every share in this section and I would rather name it than pad the table.

The account's lifetime shape first. **$743,218.09 spent, 39,569 leads, $18.78 cost per lead, 33.6 million impressions, a $22.09 CPM and a 2.14 percent click-through rate, across 1,557 ad-name groups. Zero purchases, by design.** Delivery runs 96.1 percent female, 99.3 percent mobile, 58.1 percent Facebook to 41.3 percent Instagram, and by age 32.5 percent to 25-34, 44.5 percent to 35-44, 16.4 percent to 45-54 and 4.2 percent to 55-64. **Verified**, lifetime pull 2026-09-04.

**The modality split is the finding that reframes everything else, and it corrects the premise this audit was handed.** A lifetime pull filtered to image creative returns 308 ad-name groups carrying **$168,907.73, 13,735 leads and a $12.30 cost per lead.** Subtract that and video carries **$574,310.36 and 25,834 leads at $22.23.** **Verified**, both figures from direct pulls on 2026-09-04. So statics took 22.7 percent of the money, delivered 34.7 percent of the leads, and cost 44.7 percent less per lead than video. The 90-day audits are right that zero statics ran in the trailing quarter. They are describing a shutdown, not an absence. The brand did not fail to try statics. It stopped running the cheaper half of its own account.

Per-lane lifetime spend, all figures **verified** from the 2026-09-04 pulls unless marked.

- **The deductible-shock mom.** $179,619.63 across four ad-name groups, 8,131 leads, $22.09 cost per lead. That is 24.2 percent of lifetime spend and the account's largest named lane. It holds `MOMS38 - 1 - V1` at $54,322.63 and a 17.12 percent hold rate, `MOMS39 - 2 - V2` at $53,946.44, `MOMS38 - 1 - V2` at $41,592.95 and a 16.69 percent hold rate, and `MOMS38 - 1 - V3` at $29,757.61 and a 16.46 percent hold rate. Peak was March and April 2026. This lane holds attention better than anything else the account has ever run at scale.
- **The peaceful-outcome mom.** $110,205.90 across three groups, 5,057 leads, $21.79 cost per lead, 14.8 percent of lifetime spend. `Moms43 - 4 - V3` at $57,506.21 with a 3.81 percent hold rate, `MOMS34 - N1 - 3a` at $26,858.12 with a 1.88 percent hold rate, `Moms43 - 4 - V4` at $25,841.57 with 3.81 percent. Peak is the current quarter. Costs the same as the lane above and holds a fifth as many people.
- **The employer-plan switcher.** $30,845.69 across two static ads, 2,580 leads, **$11.96 cost per lead**, 4.2 percent of lifetime spend and 6.5 percent of lifetime leads. `B1 - Copy 7` at $16,212.61 and $12.02 per lead, `B1 samar- Copy 1` at $14,633.08 and $11.89 per lead. Peak was spring and summer 2025. Nothing in this lane is live.
- **The claim-fight mom.** $14,789.67 across nine groups, 553 leads, $26.74 cost per lead, 2.0 percent of lifetime spend. Led by `OMC - C11 - 2b` at $12,257.71 with a **59.11 percent hook rate and an 18.63 percent hold rate**, the best paired attention numbers in the account. The most expensive leads in this table and the deepest watching.
- **The silent-clinician audience.** $7,407.34 on one group, 381 leads, **$19.44 cost per lead**, 1.0 percent of lifetime spend. `MOMS30 - 1 - V20`, a pediatrician in a lab coat checking a baby's heartbeat, 39.38 percent hook rate, 2.44 percent hold rate. Its age delivery is the youngest in the account at 52.7 percent aged 25 to 34.
- **The phone-call skit audience.** $3,774.02 across three ads, 163 leads, $23.15 blended, 0.51 percent of lifetime spend. `MOMS38 - 2 - V3` alone spent $1,823.59 for 59 leads at $30.91 with a **51.78 percent hook rate and a 24.48 percent hold rate, the highest hold rate anywhere in this account**, and a 13-second average play time.
- **The self-employed mom.** $1,878.04 across two ads, 112 leads, $16.77 cost per lead, 0.25 percent of lifetime spend. Essentially one static headlined "If you're self-employed, between jobs, or just tired of paying too much..." Its delivery is startling: **28.5 percent of spend on women 45-54 and 25.9 percent on 55-64**, so 54.4 percent went to women over 45 against 21.2 percent account-wide.
- **The single mom.** $1,745.23 across two ads, 119 leads, $14.67 cost per lead, 0.23 percent of lifetime spend. One static, headlined "I'm a single mom, and I didn't know my insurance was failing us... 😭."
- **The income-gap mom.** $170.46 across two ads, 9 leads, $18.94 cost per lead, 0.02 percent of lifetime spend. Two December 2025 videos whose narrator says "Making over 50k just disqualified this family from affordable healthcare" and "you're basically making a second mortgage payment every month."
- **The expecting mom.** **$0.00. Zero ads. Zero impressions.** A lifetime keyword search for "pregnant" across every ad field returns totalMatching 0.
- **The chronic-condition family.** No ad in the account names a health condition, a diagnosis or a medication. Marked **data-limited** rather than zero, because a keyword search cannot prove the absence of an angle the way it proved the pregnancy one, but no doc in this brain and no ad I read carries it.
- **The mom whose kids are grown.** No ad names her. The lane that reaches her does so by accident: `Moms36 - 3 - A - 2 - V4c`, the "I wish this was a joke... (health insurance)" skit, spent $14,436.16 across two groups for 572 leads at $25.24, and put **30.8 percent of its spend on women 45-54 and 9.4 percent on 55-64**, so 40.2 percent landed on women over 45. It holds 14.43 percent.

**What the posture actually is.** This account is not spread thin and it is not focused. It is drifting. Two lanes, the deductible-shock mom and the peaceful-outcome mom, hold 39.0 percent of everything ever spent, and the second of the two is not a persona at all. It is a mood. Every named persona lane in the account combined, the seven below the top two, holds $60,610.45, which is 8.2 percent of lifetime spend. Read through the breakdown effect, Meta pushed money into the pocket it predicted would stay cheapest, and the pocket it found was the one with the most creative in it. That is a delivery outcome, not a targeting decision, and nothing in the brand context or the chat history records anyone choosing it. **Inferred** from the concentration pattern against a shrinking format menu.

Two more shape facts belong here because section four turns on them. On desire, lifetime spend runs **65.9 percent on care and protection of loved ones and 22.0 percent on freedom from fear, pain and danger**, with social approval at 0.8 percent and four of the eight Life Force desires at zero, including survival and life extension, which is the most literal thing a health plan sells. On awareness, **60.9 percent problem aware, 28.6 percent solution aware, 0.1 percent most aware and 0.0 percent unaware**, the last being $75.22 across two ads in the account's entire life. **Verified.** The account has never once tried to reach a woman who was not already unhappy with her insurance.

## The gap

Put the two sides next to each other and the mismatch is not subtle.

**Where the brand is roughly aligned.** The deductible-shock mom is the biggest identity in the comment corpus and the biggest named lane in the spend, at 12.1 percent of comments and 24.2 percent of lifetime money. That is a real match and it should stay funded. The creative built for her also holds attention better than anything else the account owns, at 16 to 17 percent against a craft floor of 12. The one honest caveat is that the corpus is 60.1 percent concentrated on that same creative family, so some of her apparent size is the ad's own comment volume talking back to itself.

**Where the brand is over-investing.** The peaceful-outcome mom takes $110,205.90 of lifetime spend, 14.8 percent, and has almost no counterpart in the buyer evidence. Across 1,322 comments there are roughly 12 clear moments of recognition, under 1 percent, and they cluster on the phone-call skit rather than on the bedroom montage. What the montage generates instead is argument and its most-quoted response is a rejection of the footage itself: *"I'm sure the mom that can afford matching outfits prob just pays in cash 🤦‍♀️,"* posted 2026-09-03. **Verified.** The brand's own five ICPs are a woman with a cracked windshield and a $900 emergency fund, a woman who did the math six times on a $480 premium, a woman getting three different answers from HR, and a woman afraid of dropping one of the plates she is holding. **Stated.** None of them lives in that bedroom. The account is spending its second-largest lane showing a mom the outcome she does not have, in a house she cannot afford, with the sound off.

**Where the brand is under-investing, and this is the heart of it.** Three proven buyers are getting a rounding error.

The employer-plan captive is the sharpest case, because the evidence runs both ways at once. On the buyer side she recurs across at least five ads in her own words and the brand's own context names employer coverage as its most common competitor. On the spend side the two ads built for her returned an $11.96 cost per lead across 2,580 leads, the cheapest at real scale anywhere in the account, 36.3 percent below the lifetime blend and 47.2 percent below the trailing quarter. And she gets 4.2 percent of lifetime spend, none of it recent. This is not a persona that needs testing. It is a persona that was tested, won, and was put down.

The self-employed mom in the income gap gets 0.25 percent of lifetime spend against a stated ICP built for her and independent corroboration in the comments. Her one static returned $16.77, inside the brand's good band, on $1,878.04 total.

The mom whose kids are grown gets nothing named at all, while the one ad family that happens to reach her sends 40.2 percent of its spend to women over 45 and holds 14.43 percent of them. The brand said in its own testing priorities that it wants to reach *"All different ages of moms with ages of kids"* and named older second-chapter moms. **Stated.** The account has never built an ad that says so.

**Where the gap is a product question rather than a creative one.** Two personas here cannot be solved by spending differently. The expecting mom is the widest and longest-running objection in the corpus, 42 comments across 15 ads over fourteen months, and she is 63.2 percent of the category's organic feed, and the product screens her out. The chronic-condition family is the most emotionally intense identity in the corpus and underwriting screens her out too. Reaching either one harder makes the problem worse, not better, because the advertising is already recruiting them and the funnel is already turning them away in public. **Inferred**, confidence strong on the mechanism and thin on the size, since nobody outside the brand can count how many of the 39,569 leads met the gate instead of the offer.

**What the disconnect reveals about the account.** For an ecommerce brand, a persona with heavy spend and thin buyer evidence is usually a retention play, and the audit's job is to name the gap and let the brand decide whether it is deliberate. That escape hatch does not exist here. **This account has zero purchase events, no returning buyer, no repeat purchase, and 0.1 percent of lifetime spend at the most-aware stage.** **Verified.** There is no retention story that explains $110,205.90 on a mood. Every dollar in this account is acquisition, so every persona mismatch is an acquisition mismatch, full stop.

Which makes the modality finding the real diagnosis. The brand's whole cheap half is static, and its statics are where the persona-named creative lives. Look at what the static library actually says: "Left my big insurance company for a mom-focused one," "Didn't know I could ditch my job's health plan," "If you're self-employed, between jobs, or just tired of paying too much," "I'm a single mom, and I didn't know my insurance was failing us," "One ER visit could've wiped us out" at $9.62 per lead, "I PAID $1,000 OUT-OF-PICKET FOR A 5-MINUTE ULTRASOUND" at $6.99 per lead. **Verified.** Every one of those names a person and a moment. Now look at the video the account has been buying instead: a woman in bed, no words, "Wife of the year energy." The account did not just switch formats. It switched from talking to somebody specific to talking to nobody in particular, and it paid 44.7 percent more per lead to do it.

**Where the brand's own rules bind, stated plainly.** The two largest alternatives customers name unprompted are the ones the brand has forbidden itself from mentioning. My own comment counts on 2026-09-04 confirm both: **"medicaid" appears in 17 of 1,322 comments and "marketplace" in 14.** **Verified**, two independent SQL counts. The brand's non-negotiable compliance section bans *"No government/ACA references"* and lists "ACA" among the words never used in creative, and the villain must always be the system, never a named company. **Stated**, brand context Section 8. So the income-gap mom's entire story, that she earns too much for one program and too little for the other, is a sentence the brand cannot finish. That is the single most specific place the rule costs money in this document, and it is worth the brand knowing the price rather than only the rule.

The rule is also already being broken, at small spend, in the account's favor. `MOMS25 - 5TH DEC - Y1 - Copy 5` and `Copy 3`, both created 2025-12-05, run a script whose narrator says *"there's companies like health for moms that operate completely outside the marketplace system"* and *"They're not locked into Obamacare rules."* **Verified** from the script block, pulled 2026-09-04. Those two ads spent $170.46 for 9 leads at $18.94, inside the brand's good band, and they are the only ads in the account's life that speak the income-gap mom's language: "Making over 50k just disqualified this family," "you make too much for a subsidy," "a second mortgage payment every month." Nine leads settles nothing. But the account currently holds one live example of the forbidden comparison performing at good-band cost, and nobody has reconciled that against the rule. That reconciliation belongs to the brand, not to this audit.

## Whitespace and recommendations

Ranked by conviction about fit and by the weight of the buyer evidence in section two. Every one is checked against the spend history in section three, and where the persona was tried and underperformed I have said so rather than recommending a fresh test.

### 1. The employer-plan captive. A proven buyer the brand is under-investing in.

This is the highest-conviction call in the document and it is not close. She has been served, she converted at the cheapest cost per lead in the account's history, and she has been dark for months. `B1 - Copy 7` and `B1 samar- Copy 1` together returned **2,580 leads at $11.96** on $30,845.69 of lifetime spend. **Verified.** Against the trailing quarter's $22.67, that is a 47 percent gap. Both are statics, which means the production cost is a sentence and a photograph, and the brand's stated bottlenecks are casting first and production fourth, so this recommendation routes around the constraint the brand says hurts most.

The creative angle is one line the account has never said. Not "you could save." The rule: she is allowed to decline the coverage her job offers. Right now a stranger teaches her that in the replies, and the brand watches. Pair it with the switching frame that already works, first person and past tense, "Didn't know I could ditch my job's health plan… until I did," because that headline is the account's second-cheapest lead at scale and it is doing exactly this job at half strength. The risk is honest and it sits downstream: a woman on an employer plan may have a payroll-deducted, pre-tax arrangement that a private plan cannot beat on real cost, which would show up as a lead the agent cannot close. That is a gate-two question and Parker cannot see it. Fund it anyway, because the lead is twelve dollars.

### 2. Restart statics as a modality. A proven format the brand switched off.

Strictly this is not a persona recommendation, and it sits second because everything below it gets cheaper if it happens. **308 static ad-name groups, $168,907.73, 13,735 leads, $12.30 per lead against video's $22.23.** **Verified.** Zero ran in the last 90 days. The brand's own guidance permitted them: *"We want to focus mostly on video ads. MAYBE some image ads are fine to find angles."* **Stated.**

The case is not that statics are better creative. It is that this account's statics are where the persona-named messages live, and the persona-named messages are where the cheap leads are. "One ER visit could've wiped us out" at $9.62 per lead and "I PAID $1,000 OUT-OF-PICKET FOR A 5-MINUTE ULTRASOUND" at $6.99 are the two cheapest leads in the whole static library, and both are one specific sentence about one specific moment. The constraint worth naming: this brand's stated volume is one to five net-new concepts a month, which is very few shots on goal, and a headline static is the only asset in the brand's whole repertoire that needs no creator, no shoot and no script. Before the November 1 open enrollment ramp, that is the difference between five swings and twenty. There is one real open question in the way, and it is loop two below: nobody has written down why statics stopped.

### 3. The mom whose kids are grown. A proven buyer the brand has never served.

She is 16 comments across 7 ads asking politely whether she still counts, and she gets zero named spend. The accidental evidence is strong enough to act on: the `Moms36 - 3 - A - 2 - V4c` skit family spent $14,436.16, returned 572 leads at $25.24, holds 14.43 percent, and sends 40.2 percent of its money to women over 45 against 21.2 percent account-wide. **Verified.** The self-employed static does the same thing harder, at 54.4 percent over 45. So the account already knows two ways to reach her and has never once addressed her.

The angle is the one she hands over herself: her deductible got worse after the kids left, and she assumes the word "mom" no longer includes her. "My deductible used to be reasonable, now it's almost $7000 a year." **Verified.** Say plainly that a mom is a mom whether her kid is four or twenty-four. Two constraints. First, an older audience needs slower pacing and longer cuts than this account's current creative uses, and the brand's own guardrail against punching down at demographic groups means the line has to be inclusive rather than a joke about age. Second, the format that reaches her is skit and educational work, which the account collapsed by 97.7 percent last quarter, so reaching her means restarting a production lane, not just changing a headline.

### 4. Let the clinician speak. A half-tested authority play inside an already-served persona.

The brand lists Authority as untested at number three on its own video wish list. **Stated.** That is true of the hook and false of the casting. `MOMS30 - 1 - V20` put a pediatrician in a white lab coat and mask on screen, spent $7,407.34, and returned **381 leads at $19.44**, inside the brand's good band. The whole transcript is one line at 0:11 from an unnamed narrator: "Finally, insurance that actually feels like it has our back." **Verified.** The doctor never speaks. That is not a failed test. It is an unfinished one, and the 2.44 percent hold rate is exactly what you would expect from an opener that promises authority and a body that never delivers it.

The reason this earns a slot is the trust problem underneath it. The brand's own context flags that people search whether Health For Moms is legitimate, the comment section carries "don't believe this" and "Not recommend" twice, and a self-identified licensed advisor publicly tells viewers never to submit their information. **Verified.** A peer saying "this worked for me" cannot answer a legitimacy question. The constraint is the brand's own non-negotiable rule: a doctor character requires a real licensed physician or adjusted language that implies no false credential. **Stated.** So do not cast a doctor. Cast a licensed partner agent, who is real, licensed, already inside the funnel, and whom the brand already describes as *"like your Mom BFFs."* That is authority that is compliant by construction. The risk is scheduling a real professional, which is a slower shoot than the account is used to.

### 5. Fund the phone call. The best-holding format in the account's history, tested at 0.5 percent of spend.

`MOMS38 - 2 - V3` holds **24.48 percent of viewers**, double the 12 percent craft floor and more than six times the current top spender's 3.81 percent, on a 51.78 percent hook rate and a 13-second average play time. **Verified.** Its two siblings hold 17.43 and 9.15 percent. All three together cost $3,774.02. Nothing else in this account clears the floor at any spend.

Two things make this a real recommendation rather than a curiosity. First, the comments prove the mechanic works on the persona: almost every one of the roughly 12 recognitions in 1,322 comments sits on this skit family. *"'It's out of network' 'But it's in the same building!' 'In a different hallway' 🤣🤣🤣🤣🤣 whoever came up with this ad deserves a raise!! Love this!"* and *"Had a similar conversation recently with my soon to be former insurance company."* **Verified.** Second, the category's biggest video is the same mechanic played straight, with a real hospital employee on the other end of the line.

The honest counterweight is the cost. $30.91 per lead puts the best-holding ad in this account in the brand's worst band. So this is a funded test with a clear question, not a scaling call: whether the format's cost survives a real budget, or whether deep attention here simply does not convert. The production constraint is that a real recorded call needs a real second party and a release, which is heavier than a scripted skit and is the reason the account made a comedy sketch instead.

### 6. The income-gap mom. A proven buyer the brand has mostly forbidden itself from serving.

She is well corroborated, she matches a stated ICP, and she gets 0.02 percent of lifetime spend. Her ads returned $18.94 on $170.46 and $16.77 on $1,878.04, both inside the brand's good band on volumes too thin to call. **Verified.** So this is genuinely untested rather than tested and failed, and the reason it is ranked sixth rather than second is the rule, not the evidence.

**Here is exactly where the constraint binds.** Her whole story is a comparison between two things the brand may not name. She says it herself: *"I don't make very much, just more than medicaid allows,"* and *"There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy."* **Verified.** Seventeen comments name Medicaid and fourteen name the marketplace. The non-negotiable rules ban government and ACA references outright and put "ACA" on the never-used word list. **Stated.** Write her story without those two nouns and most of it survives: the income number, the subsidy cliff, the second mortgage payment, the plan that costs more than the house note. Write it with them and it is sharper and against the rules.

What is left after the rule, and it is not nothing. Two of the eight alternatives customers name are fully open to the brand, because neither is a named company or a government program: **going without insurance entirely, which is 33 comments across 10 ads and the most popular alternative in the corpus**, and health shares, which is 5. Direct primary care, at 8 comments, is also nameable. And the brand has already written the line that does it, in the December script: *"And before you ask, yes it's real insurance. Not a health share, not some discount card."* **Verified.** That is competitive positioning against a real alternative, inside the rules, already drafted. The other thing the brand should settle is the tension named in section four: those same two ads say "outside the marketplace system" and "not locked into Obamacare rules," which reads as a breach of the brand's own rule, and only the brand can say whether that was an exception, an oversight, or a rule that has moved.

### 7. The expecting mom. The largest category demand in the market, and the one recommendation that is not a creative brief.

I am putting her last on purpose, and the ranking is the point. On buyer evidence she would be first: 42 comments across 15 ads over fourteen months, the widest and longest-running objection in the corpus, and 63.2 percent of the category's organic feed. On spend she is a perfect zero, lifetime, on every field. **Verified.** In a normal audit that is the definition of whitespace.

It is not whitespace here, because the product screens her out and the brand knows it. The website audit reached the same conclusion from the other side, and the guardrail says *"No pregnancy-only targeting — focus on moms with kids, not expectant mothers exclusively."* **Stated.** Recommending pregnancy creative would send more of this woman into a funnel that tells her no, in public, under an ad the brand paid for, using the brand's own name as the punchline.

So the recommendation is a question routed to the brand, and it is a business question, not a creative one: whether the partner agency's carrier shelf holds any product that a pregnant or planning woman can qualify for. If it does, this is the largest single opportunity in this document by a wide margin, and the category feed hands over the exact register that works, which is calm and practical rather than distressed. **Not one of the nineteen relevant videos in the category library opens on crying**, while this account's own distress creative runs $25.75 to $38.09 per lead. **Verified.** If the shelf holds nothing, the right move is the opposite of a campaign: keep her out of the targeting and answer the objection honestly when it appears, because the brand is currently paying to create a complaint it cannot resolve.

**A note on the prior quarter, required and empty.** There is no prior whitespace analysis for this brand. This is the t0 baseline. There are no prior recommendations to score, no outcomes to report, and no persona movements to track against an earlier read. Every trajectory claim in this document was rebuilt from a direct lifetime pull rather than carried forward, and the next run of this prompt will be the first one able to close a loop.

## Open loops

**1. The cheapest leads this account ever bought came from the format it stopped making.**
Statics carry 22.7 percent of lifetime spend and 34.7 percent of lifetime leads, at $12.30 against video's $22.23, and zero statics ran in the last 90 days. The two cheapest ads at real scale in the account's history are both statics that name a specific person and a specific moment, and both are dark.
*Pull: Gap.* It fired when a filtered lifetime pull returned 308 static ad-name groups worth $168,907.73, in an account three separate 90-day audits describe as having never run a static.
**Question: What made the team stop making statics?**
If it was a staffing or agency change, statics are the fastest way to raise this brand's one to five concepts a month before November 1. If something was learned, a lead-quality problem from static form-fills or a platform issue, that reason is a hard constraint that changes two of this audit's top three recommendations. **Only the brand can answer this one.**
*Territory: Product.*

**2. The account's most expensive persona is the one nobody in the comments recognizes.**
$110,205.90 of lifetime spend sits on the peaceful-outcome montage. Across 1,322 comments there are roughly 12 clear recognitions, under 1 percent, and they cluster on a skit that cost $3,774.02. The most direct response to the montage's footage is a rejection of it.
*Pull: Tension.* Meta's delivery says this is the most potent creative in the account, and the only unprompted audience evidence available says nobody sees herself in it, and both cannot be a full account of what is happening.
**Question: Who is actually clicking the bedroom ad?**
The whole case for reallocating that lane rests on whether the montage is buying a different, quieter buyer than the comment section contains, or whether it is buying a cheap click from a woman who will not close.
*Territory: Personas.*

**3. Naming a job or a life situation moves who Meta finds, and nobody planned that.**
The self-employed static put 54.4 percent of its spend on women over 45. The skit family put 40.2 percent there. The silent-clinician ad went the other way, 52.7 percent to women 25 to 34. The account overall sends 21.2 percent to women over 45. None of these was a targeting choice; all three are broad delivery reacting to what the creative says.
*Pull: Surprise.* Three ads with no audience targeting difference between them produced three completely different age distributions.
**Question: How much of this account's audience mix is being set by the words in the creative rather than by the targeting?**
The brand says it wants to reach moms of all ages, and if the copy is the lever that reaches a 48-year-old, then the persona-allocation problem and the creative-brief problem are the same problem, and the fix is a sentence rather than an ad set.
*Territory: Personas.*

**4. The brand's compliance rule and its own account disagree.**
The non-negotiable rules ban government and ACA references and put "ACA" on the never-used word list. Two ads created 2025-12-05 run a script saying the brand operates "completely outside the marketplace system" and is "not locked into Obamacare rules." They spent $170.46 for 9 leads at $18.94, and they are the only ads in the account's life that speak the income-gap mom's language.
*Pull: Tension.* A rule the brand marked non-negotiable and a live script in the brand's own account cannot both be describing what this brand is allowed to say.
**Question: What is the actual boundary on naming government programs in this brand's creative?**
The income-gap mom is a stated ICP whose entire story is a comparison the rule forbids, so knowing whether the rule is a hard legal line or a strong preference decides whether a whole persona is reachable or permanently off the table. **Only the brand can answer this one.**
*Territory: Messaging.*

**5. The account keeps recruiting the two buyers its product cannot serve.**
The expecting mom is the widest objection in the corpus, 42 comments across 15 ads over fourteen months, and pregnancy is 63.2 percent of the category's organic feed. The chronic-condition family is the most emotionally intense identity in the corpus. Both are screened out by medical underwriting, and both keep arriving anyway because a broad audience of women 25 to 44 always contains them.
*Pull: Pattern.* The same collision surfaced independently in the comment corpus, the website audit, the reputation read and the category feed, always with the brand's own name used as the setup for the complaint.
**Question: What does it cost this brand to keep buying attention from people its product turns away?**
Nobody has connected the disqualification rate to the cost per lead, and if a meaningful share of the 39,569 leads met the gate instead of the offer, then the north-star metric has been rewarding the wrong creative for the whole life of the account. **Only the brand can answer this one**, because the disqualification data sits with the partner agencies.
*Territory: Product.*

## Appendix - Parker media links

Every ad, post and source discussed in the body, indexed so a strategist can reopen the media without searching. Links and paths are preserved exactly as returned by the Parker MCP on 2026-09-04, or exactly as carried in the sibling audits where noted. Entries M001 through M028 are this brand's own Meta ads. M029 through M035 are category TikTok videos from Parker's mining library.

**M001: `Moms43 - 4 - V3`.** $57,506.21 lifetime, 2,668 leads, $21.55 CPL, 45.84% hook, 3.81% hold. The silent bedroom montage. Lead example of the peaceful-outcome lane in sections three, four and open loop 2.
Facebook ad id: 120241073380060519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

**M002: `MOMS38 - 1 - V1`.** $54,322.63 lifetime, 2,693 leads, $20.17 CPL, 17.12% hold. The "Health Insurance is a scam 🙄" ad. Anchor of the deductible-shock lane and the host of most of the corpus's comments.
Facebook ad id: 120239934711290519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239934711290519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/50a0309be06d87e55299b9e00d7962b88516c847dec96e80cfd47e6ba5959b66.mp4
Landing page: https://www.healthformoms.co/save/

**M003: `MOMS39 - 2 - V2`.** $53,946.44 lifetime, 2,317 leads, $23.28 CPL, 8.23% hold. The $6,000 deductible tweet overlay. Deductible-shock lane.
Facebook ad id: 120239934711200519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239934711200519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b5709e2fc3c51b32fc818394fcc0d33d94206dccad0c923f953671d48875d937.mp4

**M004: `MOMS38 - 1 - V2`.** $41,592.95 lifetime, 1,770 leads, $23.50 CPL, 16.69% hold. Deductible-shock lane; carries the employer-plan verbatims quoted in section two.
Facebook ad id: 120239934711130519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239934711130519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/69af0d6f1d49f1bb1d77aab8a83c89100912a7bb4f0c7a12c5f177edb41c4e93.mp4

**M005: `MOMS38 - 1 - V3`.** $29,757.61 lifetime, 1,351 leads, $22.03 CPL, 16.46% hold. Deductible-shock lane.
Facebook ad id: 120239934711030519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239934711030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/34abf0402e049c2957caeafa6a203a955020b08a7b48b7547bb5867a59a033eb.mp4
Landing page: https://www.healthformoms.co/save/

**M006: `B1 - Copy 7`.** STATIC. $16,212.61 lifetime on the single ad, 1,349 leads, $12.02 CPL. Headline: "Left my big insurance company for a mom-focused one. 24% cheaper and I choose my own doctor 😌". Recommendation 1.
Facebook ad id: 120216241083030519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120216241083030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/7e3133fccf8b205622146f7297669b76296123fb46177e5262ee89f0040ca8ba.jpg
Landing page: https://www.healthformoms.co/save/

**M007: `B1 samar- Copy 1`.** STATIC. $14,633.08 lifetime on the single ad, 1,231 leads, $11.89 CPL. Headline: "Didn't know I could ditch my job's health plan… until I did." The employer-plan captive's ad. Recommendation 1.
Facebook ad id: 120227092759640519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227092759640519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b219b0aa7f7e7ed8d83fa471803f4b6c96ad98b2de118b2a8e68038439e759a9.jpg
Landing page: https://www.healthformoms.co/save/

**M008: `B1 samar- Copy`.** The account's largest ad-name group at $61,237.93 lifetime across 76 variants, 4,917 leads, $12.45 CPL; its static half alone is $54,224.86 and 4,441 leads at $12.21. Host of the income-gap verbatims quoted in section two.
Facebook ad id: 120228910482200519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120228910482200519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/59bf52c09c6081e3dfc63e0b17e649c989b490ad5b03079e469d1dc258e2cc0f.jpg
Landing page: https://www.healthformoms.co/save/

**M009: `B2 - 10TH JUNE - Copy 1`.** STATIC. $1,877.94 lifetime, 112 leads, $16.77 CPL. Headline: "If you're self-employed, between jobs, or just tired of paying too much..." 54.4% of its spend landed on women over 45. Section three and open loop 3.
Facebook ad id: 120224684049440519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120224684049440519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/45c5cbc54f430c3c07a32a71077cdc97e1329a6f91856c6fbce9fef811164548.jpg
Landing page: https://www.healthformoms.co/save/

**M010: `OMC-Health for Moms-[B1-C3-V3] - Copy`.** STATIC. $1,127.41 lifetime, 70 leads, $16.11 CPL. Headline: "I'm a single mom, and I didn't know my insurance was failing us... 😭". Its sibling `OMC-Health for Moms-[B1-C3-V3]` ran $617.82 for 49 leads at $12.61.
Facebook ad id: 120237155754180519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120237155754180519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/df25fba1bc9d23d5ca5a0febe5f3c8c33eb8c3a132cebfb6ab8f863858369ab1.jpg
Landing page: https://www.healthformoms.co/save/

**M011: `5TH APR - Copy 29`.** STATIC. $7,188.80 lifetime, 747 leads, **$9.62 CPL**. Headline: "One ER visit could've wiped us out." Cited in recommendation 2.
Facebook ad id: 120219260803030519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120219260803030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/45224b0b0e41a9bf1b7f5d5615b382462b10f5e321ab7875df4adcbb3870f17c.jpg
Landing page: https://www.healthformoms.co/save/

**M012: `5TH APR - Copy 8`.** STATIC. $2,363.21 lifetime, 338 leads, **$6.99 CPL**, the cheapest lead in the static library. Headline verbatim, typo included: "I PAID $1,000 OUT-OF-PICKET FOR A 5-MINUTE ULTRASOUND." Recommendation 2.
Facebook ad id: 120219260387410519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120219260387410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1c600b8eb0d0ca0d4d8bf5adb40a4db4f49f64c6296f7c12987b7ac6aa8c61dc.jpg
Landing page: https://www.healthformoms.co/save/

**M013: `IMG 6`.** STATIC. $9,293.03 lifetime, 1,331 leads, $6.98 CPL. The account's oldest cheap static, created 2024-12-10. Carries the phone-call-avoidance verbatim quoted in section two.
Facebook ad id: 120212962325000519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120212962325000519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6df006357f9778a16ec730b9dcd952bb67a21915ff1a38fa4ab1227b85fc784e.jpg
Landing page: https://www.healthformoms.co/save/

**M014: `B2 - 10TH JUNE - Copy 16`.** STATIC. $18,409.73 lifetime, 1,181 leads, $15.59 CPL. Headline: "Moms....". Third-largest static in the account.
Facebook ad id: 120224684049380519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120224684049380519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/2196cede33edbb670d810d017aa0c57568dc50db2e8c71b7b7a608410b0c0aae.jpg
Landing page: https://www.healthformoms.co/save/

**M015: `MOMS30 - 1 - V20`.** $7,407.34 lifetime, 381 leads, **$19.44 CPL**, 39.38% hook, 2.44% hold. The pediatrician in the lab coat who never speaks. 52.7% of spend to women 25-34. Recommendation 4.
Facebook ad id: 120238476016180519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238476016180519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1138af6ab844716ddbcd78a371c0ea9d4897abfc8c71f84bbdadbee2a0bdd3b8.mp4

**M016: `MOMS38 - 2 - V3`.** $1,823.59 lifetime, 59 leads, $30.91 CPL, 51.78% hook, **24.48% hold, the highest in the account**, 13-second average play time. Ad set "Moms38 - 2 - 1 (when you call your insurance)". Recommendation 5.
Facebook ad id: 120239427583990519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239427583990519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/ac618198a35cfeb2673e5da1357fffe956395a61101a1885c2e462f2e58c1319.mp4
Landing page: https://www.healthformoms.co/save/

**M017: `OMC - C11 - 2b`.** $12,257.71 lifetime, 476 leads, $25.75 CPL, **59.11% hook, 18.63% hold**. "Just got off a two hour call fighting for them to cover my newborn son's hospital stay." Lead ad of the claim-fight lane.
Facebook ad id: 120239479305810519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239479305810519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/36b471d709ee3360cc4941c6c7e08f8cea2596ba52b363a7089a43cd2150abeb.mp4

**M018: `moms54-3`.** $1,283.69 lifetime, 43 leads, $29.85 CPL, 56.81% hook, 13.48% hold. The 2026-08 rebuild of the claim-fight opener. Cited in recommendation 7 on the distress register.
Facebook ad id: 120247063711860519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063711860519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/5a62b11062812d9509cb2cd8c95e89777a15d1a6ac1cdb1f6e9a92eb77f93a9d.mp4
Landing page: https://www.healthformoms.co/save/

**M019: `Moms36 - 3 - A - 2 - V4c`.** $13,753.29 lifetime, 538 leads, $25.56 CPL, 14.43% hold. "I wish this was a joke... (health insurance)". **30.6% of its spend to women 45-54 and 9.3% to 55-64.** The accidental route to the grown-kids mom. Recommendation 3 and open loop 3.
Facebook ad id: 120242561229770519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120242561229770519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/fe4ef9c25b9bd439ba7664d9b004e6a952789df99e759dd325e2a638e364cf42.mp4
Landing page: https://www.healthformoms.co/save/

**M020: `MOMS25 - 5TH DEC - Y1 - Copy 5`.** $92.60 lifetime, 5 leads, $18.52 CPL. Script names "the marketplace system" and "Obamacare rules". The income-gap mom's only real ad. Section four and open loop 4.
Facebook ad id: 120235426343210519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120235426343210519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/c9fc4d3728ca9cdd2c6ce4059f93365dbac70700a7dff0b04e2f88f969068516.mp4

**M021: `MOMS25 - 5TH DEC - Y1 - Copy 3`.** $77.86 lifetime, 4 leads, $19.47 CPL. The sibling of M020, carrying the "cheat code" open and the "Not a health share, not some discount card" line. Recommendation 6.
Facebook ad id: 120235426337000519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120235426337000519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/a2b878f11ea8418310fa610c8614f6678acf7974e99fbfc037a6f3808fc39496.mp4

**M022: `MOMS34 - N1 - 3a`.** $26,858.12 lifetime, 1,297 leads, $20.71 CPL, 49.09% hook, **1.88% hold, the lowest in this appendix**. The wordless hide-and-seek montage. Peaceful-outcome lane.
Facebook ad id: 120238774764390519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238774764390519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1c501ac53c00f4e6b9f3ee87626968c02aa9861c6958bcf6c338644cbaf1fa8d.mp4
Landing page: https://www.healthformoms.co/save/

**M023: `Moms43 - 4 - V4`.** $25,841.57 lifetime, 1,092 leads, $23.66 CPL, 47.66% hook, 3.81% hold. Third ad of the peaceful-outcome lane.
Facebook ad id: 120241073380050519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380050519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/985c6a8045a5bcfb5e7450ad0f3a00ca783b996f4ba3633337e8c84e1aac8a39.mp4

**M024: `Moms Nahuel WV#1 - V9`.** $17,723.91 lifetime, 635 leads, $27.91 CPL, 26.95% hook, 5.58% hold. The emotional-face reaction hook with the tweet overlay. Excluded from the deductible-shock lane total to keep that figure conservative.
Facebook ad id: 120240699602520519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120240699602520519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/645496c411d82a546a3e2deada69459c716615ad09f635ca0b978625c2778b37.mp4
Landing page: https://www.healthformoms.co/save/

**M025: `moms-63 3e`.** The only ad in the account that opens by voicing the employer-coverage objection: "I almost scrolled past this because I thought, 'I already have health insurance, this doesn't apply to me.'" Carried from `audits/2026-Q3/90-day-diversity-audit.md` M006.
Facebook ad id: 120247093478820519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4
Landing page: https://www.healthformoms.co/save/

**M026: `moms-53 3`.** The "Approved State List ✔️" ad and the account's highest-CTR creative in the trailing quarter. Carried from `audits/2026-Q3/90-day-diversity-audit.md` M008. Hosts the state-exclusion verbatims.
Facebook ad id: 120247254787160519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4
Landing page: https://www.healthformoms.co/save/

**M027: `OMC - C14 - 1c`.** $225.10 lifetime, 6 leads, $37.52 CPL, 61.71% hook, 12.15% hold. A mother crying while holding newborn triplets in a hospital chair. The account's closest approach to the newborn window, and one of its most expensive leads.
Facebook ad id: 120238888462850519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238888462850519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/23d1c09a115e1a2c348f07d3edb3b135b28e7eb583fcd1fdc8ae9474f8f652c4.mp4
Landing page: https://www.healthformoms.co/save/

**M028: `Yeti State Angle - 3 - V3`.** $417.33 lifetime, 15 leads, $27.82 CPL, 55.12% hook, 15.47% hold. Claim-fight lane. Routes to the `go.healthformoms.co` subdomain flagged as a tracking break in `prompts-run-log/2026-09-03-full-buildout.md`.
Facebook ad id: 120239524801690519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239524801690519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/d2882bab7fa2d6650c6781c1814092f56b9bd5c05c9816be8e09ddb97635cf4e.mp4
Landing page: https://go.healthformoms.co/save/

**M029: @drashleehendry, "This is Dr. Ashley Hendry. I was calling to get a quote for a self-pay patient."** Posted 2025-11-12. 6,200,000 plays, 661,800 likes, 22,700 comments, 208,000 shares, 108,770 saves. The category's biggest video and the real-recorded-call mechanic behind recommendation 5.
https://www.tiktok.com/@drashleehendry/video/7571648042147908894

**M030: @kaseyjaneanderson, "We have not had health insurance for three years."** Posted 2026-03-13. 872,100 plays, 75,400 likes, 12,100 shares. The category-defector persona in section two, seven.
https://www.tiktok.com/@kaseyjaneanderson/video/7616717859724545311

**M031: @readra21, "You ever wonder why we don't want insurance?"** Posted 2025-11-15. 213,100 plays. The itemised bill panning from $55,623.00 charged to $1,404.00 cash. Section two, seven.
https://www.tiktok.com/@readra21/video/7572985864435879181

**M032: @yolys.world, "If you're pregnant and you're looking for insurance and you didn't qualify for Medicaid like me, listen up."** Posted 2026-04-16. 14,700 plays, 1.96% save rate. The closest match in the library to ICP Marissa and to the income-gap mom in section two, three.
https://www.tiktok.com/@yolys.world/video/7629381899118546206

**M033: @camryunique, "I wish somebody told me about Medicaid sooner during pregnancy."** Posted 2026-05-29. 105,300 plays, 6,158 likes. The calm regret register cited against this account's distress creative in recommendation 7.
https://www.tiktok.com/@camryunique/video/7645420799112842527

**M034: @kennyslifejourney, "I just joined my husband's benefits...this to expensive 😩".** Posted 2024-11-28. 21,300 plays, 381 comments, joint-highest comment rate in the library. The employer-plan captive narrated from the inside, at $240 a month to add herself.
https://www.tiktok.com/@kennyslifejourney/video/7442341495849471275

**M035: @kclairemoore, "Stop scrolling if you're having a baby in 2026."** Posted 2025-10-30. 131,200 plays, 2,938 saves. The newborn-window content the brand has zero lifetime spend against.
https://www.tiktok.com/@kclairemoore/video/7567018980993469710
