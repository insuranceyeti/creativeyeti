---
brand: health-for-moms
doc: category-and-market-research
generated_on: 2026-09-03
refresh_by: 2026-11-15
sources_read:
  - "Parker MCP `search_facebook_ad_comments_sql`, brand aed0ff06-555d-4f4f-9bf8-31178e2fb977, corpus of 1,322 comments spanning 2025-01-13 to 2026-09-03. Nine keyword cuts run this session: open enrollment, obamacare, marketplace, medicaid, trump, underwrit, spam, call, deductible, afford."
  - "Parker MCP `search_facebook_ad_comments_semantic`, same corpus, one sweep on category-level system distrust filtered to comments with 2 or more likes."
  - "Parker MCP `search_tiktok_videos`, the brand's TikTok mining library. All 19 videos marked Relevant read with play, like, comment and share counts, relevancy reasoning, seed keywords and post dates."
  - "Public web search, 2026-09-03: KFF on 2026 ACA marketplace enrollment, premiums and the enhanced premium tax credit expiration; FTC press releases and case pages on Innovative Partners and on the December 2024 warning letters to health plan marketers and lead generators; CMS newsroom statements on unauthorized agent and broker marketplace activity; KFF Health News on ACA enrollment fraud; law firm analyses of Insurance Marketing Coalition v. FCC; healthinsurance.org, Paychex and the Federal Register on the 2024 short-term limited duration insurance rule; Georgetown CHIR on junk plans and on the 2026 open enrollment outlook; NAIC's Improper Marketing of Health Insurance (D) Working Group page; New Hampshire Insurance Department consumer alert; getinsureleads.com insurance lead industry report."
  - "`running-notes/missing-context.md`, `running-notes/brand-rules.md`"
  - "`sub-context-docs/brand-identity-analysis.md` and `sub-context-docs/website-and-product-audit.md`, both read in full"
  - "Method docs: `creative-strategy-fundamentals.md`, `seasonality.md`, `algospeak.md`, `customer-review-mining-method.md`, `expertise-routing.md`"
  - "Attempted and blocked: healthformoms.co, facebook.com, transparency.meta.com, kff.org"
data_limitations:
  - "WebSearch works in this session. WebFetch mostly does not. Every attempt to open a primary document returned EGRESS_BLOCKED: healthformoms.co, facebook.com, transparency.meta.com and kff.org were all refused by the network egress proxy. So every external fact in this doc reaches me through a search-result summary of a source, not through reading the source end to end. Treat each one as reported rather than as read at the primary record, and re-check the numbers against the original before anything legal or financial rides on them."
  - "Meta's own advertising rules for this category could not be read at the source. I could not open the Special Ad Category help page or the Health and Wellness ad standard. Marketing-agency blog posts in the search results asserted specific 2026 Meta rules, including a named review system and health-and-wellness conversion restrictions, and I could not verify any of it against Meta. Whether health insurance sits in a Special Ad Category, and what Meta's current personal-health restrictions actually say, are named blanks. This matters because the account already carries two DISAPPROVED ads with no recorded reason."
  - "Market sizing for the lead-generation layer rests on a single vendor-published blog figure with no visible methodology. No independent market report was reachable. The figure is labeled `stated` in the body and should not be treated as measured."
  - "No competitor set is tracked in the Parker app, so category density, share of voice, and how many rivals are actually bidding against this brand are all unmeasured. The competitor branch is deferred at the user's request, not failed."
  - "The TikTok mining library is keyword-seeded, not a neutral sample of category conversation. Three of its eighteen seed keywords are pregnancy or maternity terms, so any count of what moms talk about drawn from it is shaped by the seeds. Said plainly wherever it is used."
  - "The exact income band that lost the most marketplace coverage is reported by KFF as the group between 400% and 500% of the federal poverty level. I did not verify what dollar figure that maps to for a family of four in 2026, so the overlap with the brand's stated $50K to $150K+ audience is described directionally and not as a matched number."
  - "The 2024 short-term limited duration insurance rule was verified. A later Department of Labor statement dated 2025-08-07 appeared in search results and I did not read it, so whether the enforcement posture on those plans has since changed is unknown."
  - "No `get_current_time` tool was available. Every pull in this doc was run on 2026-09-03, which is the date the session reported at the time and the date every Phase 0 and Phase 1 doc in this build carries. The session clock rolled over to 2026-09-04 while this doc was being written. `generated_on` is deliberately held at 2026-09-03 so it matches the pulls it cites and the sibling docs it was built alongside, rather than claiming a research date a day later than the research."
  - "Customer reviews and post-purchase surveys are confirmed empty for this brand. Per the substitution rule in `running-notes/missing-context.md`, customer-side evidence here comes from the Facebook ad comment corpus and the TikTok mining library, and is labeled as such every time."
---

# Category and market research — US private health insurance lead generation for mothers

## How this read was built

The category around Health For Moms is not the one the brand's marketing describes. The brand talks about health insurance. The market it actually competes in is US private health insurance lead generation, which is a marketing business sitting between a consumer and a licensed agent, and it is one of the most actively policed consumer advertising verticals in the country right now. That distinction shapes everything below.

I worked from three kinds of evidence and I want to be plain about how uneven they are.

The strongest evidence is the brand's own Facebook ad comment corpus: 1,322 comments spanning 2025-01-13 to 2026-09-03. That corpus is unusually good for a category read, because a cold-traffic insurance ad draws a huge amount of general category venting that has nothing to do with this brand. Under the mining method in `customer-review-mining-method.md`, that is normally noise to strip out. Here it is the signal, because the general venting *is* the category talking. Every count below carries its denominator against those 1,322 records, and I ran ten separate keyword cuts to get them.

The second source is the brand's TikTok mining library, all 19 videos marked Relevant, read with their play, like, comment and share counts and their relevancy reasoning. That library is where the category's live cultural currents show up. It comes with a real caveat that I repeat wherever I use it: the library was pulled with eighteen seed keywords, three of which are pregnancy or maternity terms, so it is a seeded sample and not a neutral picture of what mothers talk about.

The third source is public web search on the category's regulators, its enforcement record and its size. This is where the environment hurt. Search works in this session. Fetching a page mostly does not. Every attempt to open a primary document was refused by the network proxy, including the brand's own site, Meta's policy pages and KFF. So the market and regulatory facts below reach me through search-result summaries of real sources rather than through the sources themselves. I have named each one, dated it, and said what it is. I have not filled a single gap from memory, and where I could not verify something I have left it as a blank in `data_limitations` rather than writing a confident sentence about it. In this vertical that discipline is not a formality. Fabricating a regulatory fact here would do real damage.

Two things changed my read while I worked. The first is that the category's dominant seasonal event, Open Enrollment on November 1, turns out to be nearly invisible in this brand's own audience conversation, and the reason is structural rather than an oversight. The second is that the enforcement wave rolling through this category is not aimed at fringe operators. It is aimed precisely at the layer Health For Moms occupies.

One note on the refresh date. This doc type runs on a 180-day cadence, which would put it at 2027-03-02. I have set `refresh_by` to 2026-11-15 instead, because the category's biggest seasonal event lands on November 1 and the FTC case that most affects this vertical is still moving. A category read written in early September is out of date the week Open Enrollment opens.

---

## Category size and dynamics

**The category is being reshaped by one event, and it happened eight months ago.**

The enhanced ACA premium tax credits expired on 2026-01-01. `verified` as reported by KFF via search, 2026-09-03. What followed is the whole story of this market right now.

- Average marketplace premium payments more than doubled, rising 114%, from about $888 in 2025 to about $1,904 in 2026. `verified` as reported by KFF.
- Average monthly effectuated marketplace enrollment is projected to fall to roughly 17.5 million in 2026, and possibly as low as 16.5 million, down from 22.3 million in 2025. `verified` as reported by KFF.
- A KFF survey fielded in late February and early March 2026 found that 9% of 2025 marketplace enrollees had become uninsured. `verified` as reported.
- The drop is concentrated in a specific band. KFF reports that 27% of the fall in sign-ups came from people with incomes between 400% and 500% of the federal poverty level, a group that made up only 3% of 2025 plan selections. `verified` as reported.

Read the last one slowly, because it is the most important number in this doc. The people who lost the most are the ones who earn just too much to qualify for help. That is not the poorest group. It is the group directly above the subsidy cutoff, and it lines up directionally with the household income band the brand's own guidelines describe, $50K to $150K+. I did not verify the dollar mapping of 400% to 500% of the poverty level for a family of four in 2026, so I am calling this a directional overlap and not a matched number. `inferred`, and the inference rests on the KFF income band plus the brand's stated criteria from `brand-identity-analysis.md`.

So the direction of the category splits in two, and both halves are true at once. The subsidized marketplace is shrinking hard. The pool of people shopping outside it is growing, because roughly 4.8 million people are being pushed out of a product they used to be able to afford. That last figure is my arithmetic on the two KFF enrollment numbers, 22.3 million down to a projected 17.5 million, so mark it `inferred` rather than measured. Not all of those people go shopping. KFF's own survey says 9% of them simply became uninsured.

The brand's own commenters describe that push in their own words, without being asked. One on 2026-04-24: *"new federal rules put in place by the Trump administration, including potential funding cuts for navigators and changes in marketplace operations were put in place in 2025. Enhanced subsidies that made healthcare more affordable and accessible were cut and many lost their Medicaid and Medicare costs skyrocketed."* `verified`, comment corpus. That comment opens with *"i'm not a democrat, but"*, which tells you the person is describing something they experienced, not something they are arguing for.

**The lead-generation layer itself.** The one size figure I could find for US insurance lead generation is $3.8 billion in 2026, growing 8.2% year over year, up from $2.1 billion in 2019 and projected to pass $4 billion in 2027. `stated`, and I want to be blunt about the quality here: this comes from a single lead-vendor blog with no published methodology. It is a vendor describing its own market. No independent market report was reachable from this session. Do not build a business case on that number. The direction it points, digital lead generation growing while traditional distribution shrinks, is consistent with everything else in this section, and that is all I would lean on it for.

**Is this brand competing for new entrants or for switchers?** Overwhelmingly for switchers, and the evidence is direct rather than inferred from market shape.

The account's own top-spending creative is built entirely around a person who already has coverage. From `Moms43 - 4 - V3`, the account's biggest spender at $42,741.16 in the 90 days to 2026-09-02, transcript at 0:18: *"Listen, this is why you can't simply just say, 'Oh, I have insurance, I'm covered.'"* From `moms-63 3e` at 0:11: *"I almost scrolled past this because I thought, 'I already have health insurance, this doesn't apply to me.'"* Both `verified` from transcripts in `brand-identity-analysis.md`.

The comments agree. The single loudest theme in the whole corpus is the deductible: 207 of 1,322 comments, 15.7%, contain the word. `verified`, keyword cut run 2026-09-03. You do not complain about your deductible unless you have a plan. A representative one from 2026-08-15: *"Has anyone tried this? I pay quite a bit for an employee plan with a very high deductible. Is this worth it and is it widely accepted?"*

**Confidence: strong** on the switcher read. It shows up in the brand's paid creative, in the comment corpus at a 15.7% theme rate, and in the national enrollment data, which are three independent kinds of source pointing the same way.

**What is not measured.** How many advertisers are actually competing for this audience. No competitor set is tracked in the Parker app and I could not reach Meta's ad library, so category density and share of voice are blanks. This is the largest hole in the section.

---

## Maturity and commoditization read

**This is my read, not a stated fact. I am marking it `inferred` and saying exactly what it rests on.**

### Where the category sits on the maturity arc

**Late. This is a mature category with a literate audience, and pitching creative at the education altitude would be a mistake.**

Four pieces of evidence, in order of how much weight I put on them.

**One. The audience polices the vocabulary in public.** The strongest signal in the whole corpus is not what people say about insurance, it is how hard they correct an ad that gets a term wrong. An ad in the account used the on-screen word "Medicare" while the speaker said "Medicaid," and the comment section took it apart. The top correction, 13 likes on 2025-07-20: *"Why are the words saying Medicare instead of what she is saying which is Medicaid...two different insurances"*. At least eight separate commenters made the same correction in different words, including *"Medicare and Medicaid are COMPLETELY different… A.I. Fail"*, *"Medicare is for retirees on Social Security or SS Disability and does not have a means test. Do you mean MedicAID?"*, and *"If you can't understand the difference between Medicaid and Medicare you probably should not be posting about it. Just saying…"*. Seventeen comments in the corpus contain "medicaid," and a clear majority of them are corrections. `verified`, keyword cut. An audience that catches a caption error at that rate is not an audience that needs the basics explained.

**Two. Commenters teach each other the technical rules unprompted, and they get them right.** From 2026-08-21, a long unprompted explanation to another commenter: *"Marketplace plans are guaranteed issue by law, meaning there is no medical underwriting, as long as he's eligible to enroll during a valid enrollment period. Marketplace plans cannot deny him coverage or charge him more because of a pre-existing condition, and they cannot exclude an otherwise covered benefit simply because the condition existed before enrollment."* That is accurate and it is volunteered by a member of the audience, not by an agent. `verified`, comment corpus. Another, 3 likes on 2025-08-28: *"If they're providing plans of private insurance companies, they can discriminate against pre-existing conditions (including pregnancy), which is why Obamacare was such an important thing."*

**Three. The brand's own rulebook already agrees with this read**, which is corroboration rather than proof, since the brand could be wrong about itself. Its guidelines say: *"don't over-explain concepts the audience already understands (e.g., what a deductible is) — assume problem-awareness and reframe the cause instead."* And its pool-pricing rule tells creative to *"explain why, not define terms."* `stated`, via `brand-identity-analysis.md`. Read against Schwartz, which the brand names as its own canon, that is a market-sophistication move. It is what a category does after the simple version of the claim has been made too many times to land. A brand does not write that rule for a young category.

**Four. The buyer is problem-aware and solution-aware, not product-aware.** She knows the problem cold, she knows options exist, and what she does not know is whether *this* option is real. That sets the altitude for everything downstream: the work is not explaining insurance, it is differentiating one offer from the pile.

**Confidence: strong.** Three independent source types agree, and the brand's own written strategy is the fourth.

### How commoditized the category is

**Two answers, because the offer and the audience sit at different places, and conflating them would be the wrong read.**

**At the offer level, heavily commoditized.** The pitch is the same everywhere: a savings percentage, a low or zero deductible, freedom to pick a doctor, a short form, a call from an agent. Nothing in that stack belongs to anyone. Even the brand's own named mechanism, the MomSmart Coverage Method™, is on the evidence a naming asset rather than a technology moat, as `website-and-product-audit.md` established: no commenter among 1,322 describes ever being shown a plan comparison. Under the commoditization test, this is not a category where hunting for an empty message gap works. The gaps in the message are filled. The work at this level is a differentiator, and the durable ones usually come from outside the creative, from the product, the distribution or how the brand treats people.

There is direct evidence of that commoditization inside the brand's own comment section. Rival agents openly poach there. From 2025-07-17: *"yeah medically underwritten plans want you to sign up when you are healthy - we have underwritten plans but we also have a plan that does not have strict requirements and can provide coverage with diabetes if you want to message me, we can check it out?"* And from 2026-07-16, a licensed advisor doing the same thing while warning people off the form: *"As a licensed health insurance advisor, never put your info online unless you want 100 calls a day about health insurance... DM and I can help you look at the plans available in your state."* `verified`, comment corpus. When a competitor can substitute for you in your own comment section with one message, the offer is a commodity.

**At the audience level, possibly not commoditized at all, and nobody has checked.** No major insurance lead-generation rival appears to speak only to mothers. That is the brand's own claim and `website-and-product-audit.md` already marked it `inferred` with mixed confidence, resting on the absence of a mom-specific name in the brand's own list of EverQuote, QuoteWizard, HealthPlusLife and SmartFinancial. I cannot improve on that here, because no competitor set is tracked and Meta's ad library is unreachable. So the honest statement is: the offer is a commodity, the audience position may be genuinely open, and the second half of that sentence is unverified and should not be leaned on until someone looks.

---

## Category-specific behavioral barriers

These are the things that stop a mother from entering this category at all. They are not objections to Health For Moms. They sit above it, they were built by other companies, and every brand in this space pays for them.

### 1. The phone number is the real gate, and the fear is about a different form

This is the biggest one and it is the most clearly category-level. **49 of 1,322 comments, 3.7%, mention a call.** `verified`, keyword cut. What makes them category evidence rather than brand evidence is that the most-liked ones describe a *prior* experience with somebody else's form.

From 2026-03-29, 5 likes: *"wondering the same. I filled out something like this years ago- and got spam phone calls every 10 minutes for months!"*

From 2026-05-17, 17 likes and one of the most-liked comments in the whole corpus: *"How many calls will I get if I try to see how this works?"*

From 2025-09-17, 6 likes: *"Absolutely do not give them your info. You will receive calls and texts nonstop from an insane amount of reps."*

And from an industry insider, 2026-07-16: *"As a licensed health insurance advisor, never put your info online unless you want 100 calls a day about health insurance."*

That last one is the tell. When people inside the category tell consumers not to fill out the form, the barrier is structural. Every brand in this space ends its ad by asking for a phone number, and the audience has been trained by a decade of lead resale to treat that ask as the trap. **Confidence: strong.** It recurs across fourteen months, it carries more likes than almost anything else in the corpus, and it is corroborated by the regulatory history in the trust-events section below.

### 2. The ACA taught this audience that being denied is illegal

For more than ten years the category's loudest public message has been that you cannot be turned away for a pre-existing condition. That is true of marketplace plans and false of medically underwritten ones, and the audience has generalized it into a right.

From a commenter who identifies as a certified application counselor for the healthcare marketplace, 2025-07-23: *"they're holding pre-existing conditions against you, which is illegal. Their system automatically bounced me out."*

Whether the belief is legally correct is beside the point. **The belief itself is the barrier**, and it is a category barrier, because it applies to every non-marketplace product equally. Only 3 comments in 1,322 use the word "underwrit" at all, and all three come from people who appear to sell insurance, not from buyers. So the audience does not have the vocabulary for the thing that is happening to them. They have a rule they were taught, and a rejection that breaks it.

**This is a misconception, not an objection**, and per `creative-strategy-fundamentals.md` those are different creative jobs. A value barrier gets reframed. A false belief has to be overturned, which is slower and needs a different kind of proof.

### 3. Learned helplessness about price

The category's deepest friction is not "is your price good." It is that a large part of the audience has already concluded that nothing is affordable and has stopped shopping. **46 of 1,322 comments, 3.5%, contain "afford."** `verified`, keyword cut.

From 2025-07-21, 9 likes and 6 replies, one of the most-engaged comments in the corpus: *"My husband and I both work more than full time (about 50 hrs a week each). The best we could find on the stupid Marketplace is $2100/month for just myself and my husband... How is $2,100/month 'affordable' insurance???"*

From 2026-04-07: *"I tried to get obamacare (I only make 45k with a family of 5) and the lowest plan that would allow me to visit a nearby hospital was $900 monthly for ONLY ME. Needless to say, I still have no insurance. I haven't been to a doc in over 10 years except when I was pregnant 5 years ago."*

That second one describes ten years of not seeing a doctor. That is the barrier at full strength. A savings claim, however good, is arriving to somebody who has already given up on the premise that a savings claim could be true.

### 4. The middle-income trap, which the audience names itself

This is the barrier and the opening at the same time, and the audience has a phrase for it. From 2025-08-09: *"There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy."*

From 2025-08-03: *"my income doesn't fall into the sweet spot. I don't make very much, just more than medicaid allows."*

From 2025-08-08: *"My family makes too much for Medicare and doesn't qualify for a low Obamacare plan. I can't afford the rates I'm being offered but need coverage!!"*

This is the same population KFF measures as the group between 400% and 500% of the poverty level that lost the most coverage in 2026. The customer-side language and the national data describe the same people. That cross-source agreement is why I rate this **strong** despite a small raw count.

### 5. The category is politically charged, and the politics arrive uninvited

Insurance in the US is not a neutral subject, and a mother scrolling past an insurance ad brings her politics with her. **14 of 1,322 comments, 1.1%, mention Obamacare. 6 mention Trump.** The tone runs both ways. From 2026-04-11, 8 likes and 9 replies: *"Is that Obamacare not awesome? It really made health care more affordable. Awesome."* From 2026-04-13: *"he's the best! If it wouldn't be for Obamacare people who most need it couldn't afford healthcare."*

The barrier here is not that people disagree. It is that any ad in this category converts its own comment section into a political argument, and the brand pays a moderation and brand-safety cost for a fight it did not start. Health For Moms bars political framing in its own creative and its own testing verdict is *"Anything political doesnt work."* `stated`, via `brand-identity-analysis.md`. The rule governs what the brand says. It does not govern what shows up underneath.

One timing note that keeps this honest: 9 of the 14 Obamacare mentions and 5 of the 6 Trump mentions fall between 2026-03-25 and 2026-05-26. That is a cluster, not a steady rate, and it most likely reflects one ad reaching a broad audience rather than a durable rise in political heat. I am recording it as a real barrier with a lumpy distribution rather than as a trend.

### 6. Platform moderation is a category condition, not a brand problem

Health insurance is a policed advertising vertical. Per `algospeak.md`, moderation runs in four layers rather than one: automated filters, human reviewers, engagement signals and policy enforcement. Meta specifically keeps humans in the loop, which means the durable posture in a category like this is legitimate framing and accurate claims rather than clever wording. There is no coded-language play available here and there should not be. The account already carries two DISAPPROVED ads with no visible reason, per `brand-identity-analysis.md`.

**Named blank, and it is a real one.** I could not read Meta's own rules from this session. Whether health insurance sits inside a Special Ad Category, what Meta's current personal-health restrictions say, and whether the 2026 health-and-wellness conversion restrictions that agency blogs describe are real, are all unverified. Search results asserted several specific Meta rules and I refuse to repeat them as fact. Someone with unblocked access should read Meta's Special Ad Category page and its Health and Wellness ad standard and write down what they actually say, because this is the constraint that decides what targeting and optimization are even available to the account.

---

## Cultural moments and trends

I am separating the durable shifts from the passing moments, because trends are the easiest thing in this doc to overstate. Everything in this section is raw opportunity for a later step to weigh, not a direction to commit to.

### Durable shifts

**1. The subsidy cliff moved, and it is structural rather than a moment.** Covered in full above. It is listed here because it is also a cultural event, not only an economic one. It gave a large group of people a shared, recent, specific grievance about health insurance cost, and it happened to all of them at the same time.

**2. Cash pay and price transparency have become a consumer movement.** The single biggest video in the brand's mining library is a physician calling around to get self-pay prices for pregnancy care: 6.2 million plays, 661,800 likes, 22,700 comments, from @drashleehendry. A second in the same vein, @readra21 showing a self-pay emergency room bill top-down, drew 213,100 plays. `verified`, Parker MCP TikTok pull, 2026-09-03. This is the audience routing around insurance entirely, and it is the most-watched thing in the category the mining library found. **Durable.** It is a movement with named practitioners and its own vocabulary, not a viral moment.

**3. Alternative coverage structures are going mainstream in the feed.** Three of the nineteen relevant videos are moms explaining a coverage structure that is not a traditional health plan.

- @kaseyjaneanderson, 872,100 plays, 75,400 likes, 1,316 comments, a stay-at-home mom on health care sharing through CrowdHealth. Her own caption: *"I've wanted to make this video for so long but was embarrassed that we couldn't afford regular health insurance... You'd be shocked at how much of a discount we've gotten for 'cash pay' or 'self pay'."*
- @friencine, 175,800 plays, 25,100 likes, on hospital indemnity insurance covering a delivery, with an honest update in the caption about pregnancy counting as a pre-existing condition with her carrier.
- @kclairemoore, 131,200 plays, on the same indemnity structure: *"Ever heard of indemnity insurance for moms? 👶 It's the type of plan that reimburses you for your hospital and delivery costs."*

These are the real competitors for this audience's attention and their belief about what a solution looks like, and none of them is an insurance lead generator. **Durable**, and worth flagging that indemnity plans are exactly the product shape now drawing regulatory attention, which is covered below.

**4. Maternity cost is the loudest money conversation among mothers, and this product cannot join it.** Roughly 11 of the 19 relevant videos in the mining library are about pregnancy, delivery, or the cost of a new baby, and they carry the largest numbers in the library. **The caveat is load-bearing and I am not burying it:** three of the eighteen seed keywords used to build that library are pregnancy or maternity terms, so the library is seeded toward this result and the share is not a measurement of what mothers talk about generally. What the seeding does not explain is the engagement gap. The pregnancy videos sit at the top of the library by plays, and the top one by a wide margin. Read as **directional and strong on engagement, unmeasured on share.**

The collision is obvious and it is a category fact rather than a brand failing. The most engaged conversation in this audience is about a life stage that medically underwritten plans screen out. `website-and-product-audit.md` documented 38 of 1,322 comments, 2.9%, describing a pregnancy denial, several with 4 to 7 likes.

### The seasonal pattern, and the thing that is odd about it

**5. Open Enrollment on November 1 is the category's dominant seasonal event. It is nearly absent from this brand's own audience conversation, and the reason is structural.**

The category treats November 1 as its calendar. Creators peg content to it: @insurancebyalexa tags #openenrollment, #openenrollment2022 and #openenrollment2023 on a video about employer coverage being too expensive; @adulting_with_kim tags #openenrollment2025 on a video explaining ACA subsidies. `verified`, TikTok library.

In this brand's 1,322-comment corpus, "open enrollment" appears **exactly once**. `verified`, keyword cut run 2026-09-03. Here is the whole comment, from 2026-04-25: *"Jacinda Rose yes there is. You have to sign up during open enrollment, not whenever you need it."* It is one commenter correcting another about how the ACA works. Nobody in this brand's audience is anticipating a deadline. Nobody is asking when the window opens.

That absence is not an oversight, and reading it as one would be the wrong call. Private medically underwritten plans are not gated to the November window, so this brand's product genuinely has no enrollment deadline. The brand's own document already names the resulting risk as a "feast-or-famine" vulnerability, and `website-and-product-audit.md` reached the same conclusion from the other side: life events are a year-round entry point for this product in a way they are not for marketplace plans.

Per `seasonality.md`, the useful question is never "does demand spike." It is what shifts underneath: who buys, what message lands, what the customer's context is, and when an offer actually helps. Reading that way, here is what November 1 changes for this brand even though its product has no deadline:

- **The audience's frame changes.** In November a mother who has ignored her coverage all year is actively choosing a plan. That is a different state of mind arriving at the same ad.
- **The competitive environment changes.** Every marketplace, carrier, broker and lead generator in the country is bidding for the same attention in the same feed at the same time. What that does to this account's CPMs and cost per lead is **not measured**, because no year-over-year seasonal cut has been run.
- **The conversation gets louder and more informed.** More people around her are talking about coverage, which raises both her attention and her scrutiny.

`seasonality.md` is also blunt about the most common and costly seasonal mistake, which is pulling proven evergreen creative to make room for untested seasonal creative. The evergreen winners carry the proven value propositions. Seasonal work layers on top of them and only displaces one when the data says so.

And one piece of timing that matters as of this doc's date. It is 2026-09-03. Open Enrollment opens in under two months. `seasonality.md` puts the planning lead time at three to four months, and `website-and-product-audit.md` records the brand's own two-month planning window, meaning creative for this window should already be in production. Whatever the brand decides about November, it is deciding late.

### Not a trend

**The April 2026 political spike.** Nine of fourteen Obamacare mentions and five of six Trump mentions cluster in a two-month stretch in spring 2026. One cluster in one comment section is a moment, not a shift in the culture. Recorded so nobody builds on it.

---

## Industry-wide trust events

This is the section that matters most for this brand, and the finding is not subtle. **This category is in the middle of an active enforcement wave, and the wave is aimed at the exact layer Health For Moms occupies: the non-carrier online intermediary marketing non-marketplace coverage to people who were just priced out of the marketplace.**

Every event below was verified through public web search on 2026-09-03. As stated in `data_limitations`, none of the primary documents could be opened from this session, so each is reported rather than read at the source.

### 1. FTC v. Innovative Partners, filed April 2026. The most live event, and the closest to home.

The FTC sued Innovative Partners LP doing business as Innovative Health Plan, American Collective LP, Health Plan Administrators LLC, Papyrus Green Investments LLC and two individual defendants. At the FTC's request a federal district court **in Florida** temporarily halted the operation. The FTC alleges a nationwide scheme that took roughly **$91 million** from consumers by impersonating the government and large insurance carriers to sell people who were shopping for health insurance what they were told were comprehensive PPO plans, and which the FTC describes as non-comprehensive medical discount memberships and limited benefit plans. A receiver was appointed. The New Hampshire Insurance Department opened a time-limited special enrollment period for residents affected by it. `verified` as reported via FTC press release, the FTC case page, the New Hampshire Insurance Department, the Kansas Department of Insurance and trade press.

**How live: extremely.** Five months old and still in progress.

**Blast radius, and this is my read.** It damages trust across the whole intermediary layer, not just the defendants. The specific lesson a consumer takes from it is: an online health insurance offer that is not a carrier, that reaches you through an ad, and that leads to a phone call, may not be what it says it is. That describes the shape of every lead generator in the category, including this one. The Florida connection is coincidental, since Health For Moms is based in Orlando and operates as Insurance Yeti, LLC, but coincidence is not how a suspicious consumer reads a headline.

### 2. FTC warning letters to 21 health plan marketers and lead generators, December 2024

FTC staff sent warning letters to 21 companies that market health plans or generate sales leads for them, with guidance on deceptive or unfair claims. The letters cited the agency's prior actions in this field: **Simple Health Plans**, where the FTC obtained a $195 million judgment against the company and its CEO over sham health care plans; **Benefytt Technologies**, which agreed to $100 million in consumer refunds, with its former CEO and a former vice president of sales **permanently banned from selling or marketing any healthcare-related product**; plus Partners in Healthcare Association and Consumer Health Benefits Association. The FTC's own framing tied the timing to the start of open enrollment. `verified` as reported via FTC press release and trade press.

**How live: very.** Twenty-one months old, and it is the clearest public statement of where the line is for a business that does exactly what this brand does.

**Blast radius.** This one constrains what the brand can safely say. The Benefytt case in particular is instructive because the FTC named **deceptive lead generation websites** as part of the violation, not just the plans themselves. That means the funnel is in scope, not only the product at the end of it. Against this backdrop, the finding in `brand-identity-analysis.md` that nine of the ten highest-spending statics carry a flat savings claim with no "up to," holding $116,622.92 and 69.0% of all static spend the account has ever made, stops being an internal rulebook violation and becomes a category-shaped exposure.

### 3. The ACA broker fraud wave of 2024

CMS received more than **275,000 complaints** during 2024 about unauthorized ACA enrollments and plan switching. In the first six months of 2024 alone it logged 73,884 complaints of unauthorized plan switches. Between June and October 2024 CMS **suspended 850 agents' and brokers' Marketplace Agreements** for reasonable suspicion of fraudulent or abusive conduct. From 2024-07-19 CMS blocked agents from changing a consumer's federal marketplace enrollment unless already associated with it. `verified` as reported via CMS newsroom statements and KFF Health News.

**How live: fading but not gone.** The peak was two years ago and the system changes are in place, but reporting indicates unauthorized changes continued after the mid-2024 rules took effect.

**Blast radius, and this is the one people underestimate.** It damaged trust in **the agent**, not the insurer. That is a different wound, and it lands directly on this brand's business model, which is a handoff to an agent. A mother in the brand's own comment section on 2026-02-24 describes exactly what that wave taught her: *"Someone on marketplace, we talked for 2 hours... At one point she said, let's put in that you make 25k less than what you do. Hubby and I, right then and there, knew this wasn't the lady to go with."* `verified`, comment corpus. She did not report the agent. She just walked away, which is what most people do, and which is why this shows up as a conversion problem rather than a complaint.

### 4. The TCPA one-to-one consent whipsaw, 2023 through 2025

The FCC's 2023 one-to-one consent rule would have required a consumer's consent to name the single company contacting her, which would have effectively ended the practice of one form feeding a long list of buyers. The Eleventh Circuit **vacated it on 2025-01-24** in *Insurance Marketing Coalition v. FCC*, holding that the FCC exceeded its authority under the TCPA. The FCC said in April 2025 it would not challenge the ruling, and in September 2025 issued a final rule formally eliminating the requirement and reinstating the prior version. `verified` as reported via multiple law firm analyses.

Note the name of the case. The insurance lead generation industry sued to keep multi-buyer consent legal, and won.

**How live: settled law, live consequence.**

**Blast radius.** This is the regulatory reason the category's biggest behavioral barrier still exists. The one rule that would have stopped "I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies" is gone. `verified` comment, 2025-11-28, from `website-and-product-audit.md`. For a category read this matters twice: the harassment barrier is not going to be fixed by regulation, and a brand in this category cannot point to a rule as proof that it will not happen.

### 5. The short-term plan rule, effective 2024-09-01

HHS, Labor and Treasury finalized a rule on 2024-03-28 limiting new short-term limited duration insurance to three-month terms and four months total including renewals, and amending the consumer notice requirements so people can tell the difference between comprehensive and non-comprehensive coverage. STLDI does not have to comply with ACA protections, including coverage of pre-existing conditions. `verified` as reported via the Federal Register, healthinsurance.org, AHA and Paychex.

**Named blank:** a Department of Labor statement on STLDI dated 2025-08-07 appeared in the search results and I did not read it, so whether the enforcement posture changed after that date is unknown. Someone should read it.

**Blast radius.** It narrowed the shelf of non-marketplace products and, more importantly for a marketer, it made a formal norm of the disclosure that a plan is not comprehensive coverage. I cannot say from here which product type Health For Moms' partner agency actually sells, since the plan names, tiers and carriers are all named blanks in `website-and-product-audit.md`. That gap is exactly what makes this rule impossible to apply and worth routing to the brand.

### 6. The standing regulatory watch, and the reason it exists

The NAIC runs an **Improper Marketing of Health Insurance (D) Working Group**, coordinating state and federal regulators on monitoring and enforcement of improper health plan marketing. Georgetown's Center on Health Insurance Reforms published analysis in this period on **"the peddling of junk plans to consumers facing higher insurance premiums,"** and the Commonwealth Fund published a February 2026 explainer on what consumers need to know about coverage that does not comply with the ACA. `verified` as reported.

**Blast radius, and it is the one that ties the whole section together.** The regulators and the policy researchers have explicitly connected the 2026 premium spike to a surge in deceptively marketed alternative coverage. In other words, the exact market opening this category is riding is the thing being watched. A brand advertising private coverage to people who just lost their subsidy is operating inside a lane that consumer advocates have publicly named as the risk lane.

### The read on the whole picture

**This is not a clean category, and checking was worth it.** Six distinct events, four of them federal enforcement actions, all landing between 2024 and April 2026, all aimed at the marketing layer rather than at carriers.

The blast radius runs three ways at once, which is unusual.

It **wounds trust across the category**, because the FTC cases teach consumers that an online health insurance offer from a company that is not a carrier may be a discount card in a PPO costume.

It **constrains what any brand here can safely claim**, because the Benefytt case put the lead generation funnel itself inside the violation, and because the December 2024 letters told 21 companies in this exact business where the line sits.

And it **opens a position**, which is the part a later step should weigh rather than assume. When enforcement defines publicly what bad looks like, a brand that is visibly and checkably not that has something to stand on. The catch is that standing apart requires evidence a consumer can check, and `brand-identity-analysis.md` found that every credibility marker this brand carries is owned and self-asserted, with no named carrier, no named partner agency, no third-party recognition and no reviews. Naming the opening is my job. What to do about it belongs to the strategy work downstream.

---

## Open loops

Four. Creators and talent is not clean at the category level, but the question there is already open in `website-and-product-audit.md` as the synthetic-talent loop, so I am consolidating rather than restating it.

**1. What actually changes for this brand's buyer between November and February?**

Open Enrollment on November 1 is the category's dominant seasonal event. Creators peg content to it with #openenrollment2025 and similar tags, and the category's whole calendar runs on it. In this brand's 1,322-comment corpus it appears once, on 2026-04-25, and that one mention is a commenter explaining ACA rules to somebody else rather than anyone anticipating a deadline. The product itself is not gated to that window, because private medically underwritten plans have no enrollment period.

*Pull: Gap.* The category's biggest moment of the year leaves essentially no fingerprint in this brand's own audience conversation, and nobody has checked whether that absence is real or just unmeasured.

*Question:* What changes for this brand's buyer between November and February?

*Why it is a loop:* If very little changes, then the brand should not spend its short planning runway building for a window it does not actually sell into, and the eleven other months are the bigger prize. If a lot changes, in her frame of mind, in what the feed costs, or in how much competition she sees, then September is already late and the answer decides what gets produced in the next four weeks.

*Territory: Product.*

**2. How much of the health insurance conversation among mothers is about something other than pregnancy and a new baby?**

Roughly 11 of the 19 relevant videos in the TikTok mining library are about pregnancy, delivery, or the cost of a new baby, and they carry the largest view counts in the library, topping out at 6.2 million plays. The product screens out women who are pregnant or planning to be. Three of the eighteen seed keywords used to build that library are maternity terms, so the library is pointed at that conversation rather than measuring it.

*Pull: Tension.* The loudest, most-watched conversation this brand's mining has surfaced among mothers is the exact one its product is barred from joining, and I cannot tell how much of that is the world and how much is the keyword list.

*Question:* How much of the health insurance conversation among mothers is about something other than pregnancy and a new baby?

*Why it is a loop:* If the conversation really is mostly maternity, the brand is buying attention in a room where most people cannot buy, and the persona work should aim at a later stage of motherhood. If a large non-maternity conversation exists that the seeds never looked for, then the brand's own inspiration library has been pointing it at the wrong lane, and re-seeding is cheap.

*Territory: Personas.*

**3. How much of the gap between a click and a finished form is fear of the phone call?**

49 of 1,322 comments, 3.7%, mention calls, and the loudest ones describe a different company's form. One with 5 likes: *"I filled out something like this years ago- and got spam phone calls every 10 minutes for months!"* Another with 17 likes just asks: *"How many calls will I get if I try to see how this works?"* A licensed advisor in the same comment section tells people never to put their information online. Meanwhile the FCC rule that would have banned multi-buyer lead sharing was struck down in January 2025 and formally repealed that September, so nothing is coming to fix this.

*Pull: Pattern.* The same fear keeps surfacing from independent people across fourteen months, aimed at the category rather than at this brand, and it sits on the exact step every ad in the account asks for.

*Question:* How much of the gap between a click and a finished form is fear of the phone call?

*Why it is a loop:* Every ad here ends by asking for a phone number. If the phone fear is the main leak, then hook rewrites and savings claims are working on the wrong part of the funnel, and the leverage moves to what the form promises about what happens next. The account already shows link clicks against landing page views against leads, so this is answerable with data Parker can reach.

*Territory: Messaging.*

**4. What does a mom in this category treat as proof that a health insurance offer is real?**

The FTC sued a Florida operation in April 2026 for allegedly taking $91 million by impersonating carriers and the government to sell limited benefit plans as comprehensive PPO coverage, and it warned 21 health plan marketers and lead generators in December 2024. Regulators are actively teaching this audience to distrust intermediaries whose names they do not recognize. Health For Moms names nobody: no carrier, no partner agency, no third party, no reviews, and every credibility marker it carries is its own assertion.

*Pull: Curiosity.* The category is running a public education campaign about how to spot a fake insurance offer, and I do not know what the audience has learned to look for.

*Question:* What does a mom in this category treat as proof that a health insurance offer is real?

*Why it is a loop:* Trust is the binding constraint in this category, not attention. If the proof she wants is a carrier name, a license number, or another mother she can see, then a warm mom-to-mom voice is solving a problem she does not have, and the brand's whole credibility stack is pointed the wrong way. The answer is reachable from the ad comments, from category forums and Reddit, and from competitor reviews, all of which the substitution rule in `running-notes/missing-context.md` already permits for this brand.

*Territory: Messaging.*

---

## Appendix - Parker media links

All links preserved exactly as returned by Parker MCP or by web search.

**Brand:** Health For Moms, brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`. **Ad account:** `HealthForMoms`, act `484897827497337`.

### TikTok mining library — the videos this category read rests on

Cash pay and price transparency:

- @drashleehendry, "Join me as I call around and get self pay pricing for pregnancy care 💰", 6.2M plays, 661.8K likes, 22.7K comments
  - https://www.tiktok.com/@drashleehendry/video/7571648042147908894
- @readra21, self-pay emergency room bill, 213.1K plays
  - https://www.tiktok.com/@readra21/video/7572985864435879181

Alternative coverage structures:

- @kaseyjaneanderson, health care sharing through CrowdHealth, 872.1K plays, 75.4K likes, 1,316 comments
  - https://www.tiktok.com/@kaseyjaneanderson/video/7616717859724545311
- @friencine, hospital indemnity insurance for delivery, 175.8K plays, 25.1K likes
  - https://www.tiktok.com/@friencine/video/7584916120965008671
- @kclairemoore, "Ever heard of indemnity insurance for moms?", 131.2K plays
  - https://www.tiktok.com/@kclairemoore/video/7567018980993469710
- @yolys.world, Aetna Enhanced Maternity Program, 14.7K plays
  - https://www.tiktok.com/@yolys.world/video/7629381899118546206

Maternity and new-baby cost:

- @paumod, insurance covering maternity and postpartum items, 916.2K plays, 81.4K likes
  - https://www.tiktok.com/@paumod/video/7593050209676987662
- @asap.kristy, cost of monthly doctor visits while insured and pregnant, 120.2K plays
  - https://www.tiktok.com/@asap.kristy/video/7536693373290270007
- @camryunique, Medicaid during pregnancy, 105.3K plays
  - https://www.tiktok.com/@camryunique/video/7645420799112842527
- @camryunique, Medicaid benefits for expecting mothers, 20.2K plays
  - https://www.tiktok.com/@camryunique/video/7656091476400672031
- @dannitangie, "How much did you pay for your delivery???", 28.2K plays
  - https://www.tiktok.com/@dannitangie/video/7611735950615498014
- @amandatalksalot, budgeting for a baby including added insurance cost, 14.4K plays
  - https://www.tiktok.com/@amandatalksalot/video/7538841869065768247
- @goojiepooj, insurance billing confusion, "Literally scared to check my credit", 83.9K plays
  - https://www.tiktok.com/@goojiepooj/video/7444916814754237742

Open Enrollment as an organic content peg:

- @insurancebyalexa, "is your employer health insurance too expensive?", tagged #openenrollment, #openenrollment2022, #openenrollment2023, #familyglitch, 29K plays
  - https://www.tiktok.com/@insurancebyalexa/video/7172410850244988206
- @adulting_with_kim, ACA marketplace explainer tagged #openenrollment2025 and #uninsured, 25.5K plays
  - https://www.tiktok.com/@adulting_with_kim/video/7431177503483415839

Cost of a family, and the frustration of picking a plan:

- @salina_sunshine, political ad on eliminated healthcare tax credits, opens on an unexpected ER visit, 235.8K plays
  - https://www.tiktok.com/@salina_sunshine/video/7680344555161521421
- @molly_daw, "Are we not living in the same economy", cost of children, 31.2K plays
  - https://www.tiktok.com/@molly_daw/video/7576033059330329886
- @kennyslifejourney, cost of adding a spouse to an employer plan, 21.3K plays
  - https://www.tiktok.com/@kennyslifejourney/video/7442341495849471275
- @nothingeversticks, "Picking a health insurance plan is so much fun", single mom, 13.1K plays
  - https://www.tiktok.com/@nothingeversticks/video/7651751227738410253

Parker inspiration dashboard for the mining library:

- https://app.heyparker.ai/dashboard/inspiration?video_report=c284bf02-419e-4332-a8a9-aae37bcc4704&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- https://app.heyparker.ai/dashboard/inspiration?video_report=f61d6671-3d49-4e61-96d1-97a730a56ca4&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- https://app.heyparker.ai/dashboard/inspiration?video_report=3b443979-1d81-4537-a25c-a9f44715c240&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- https://app.heyparker.ai/dashboard/inspiration?video_report=9723d817-f5c9-46d8-829f-996332d76784&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- https://app.heyparker.ai/dashboard/inspiration?video_report=2204a185-fb6d-4470-9f62-efd10d301e93&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- https://app.heyparker.ai/dashboard/inspiration?video_report=1368ee20-a5a2-4dff-8040-da1bc9b4b88b&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- https://app.heyparker.ai/dashboard/inspiration?video_report=19a1fcb8-fa59-40fb-b9a5-f76ba6590777&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- https://app.heyparker.ai/dashboard/inspiration?video_report=8311a25c-dbdd-48b4-8ae9-b0da327be0ac&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- https://app.heyparker.ai/dashboard/inspiration?video_report=9d665f4b-7c17-4ff0-9ac8-03d35c5ee0c8&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

### Ad creative quoted in this doc

The category-switcher read rests on transcripts read at full media depth in `brand-identity-analysis.md` and `source-pulls/ad-account.md`.

- `Moms43 - 4 - V3`, account top spender, "you can't simply just say, 'Oh, I have insurance, I'm covered'"
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4
- `moms-63 3e`, "I already have health insurance, this doesn't apply to me"
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4

### Comment corpus

All comment evidence comes from Parker MCP against brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`, corpus of 1,322 comments spanning 2025-01-13 to 2026-09-03. Comments carry no permalink in the Parker response, so they are cited by their exact text, date and like count throughout the body. Keyword cuts run 2026-09-03 with their totals:

- `deductible` — 207 of 1,322, 15.7%
- `call` — 49 of 1,322, 3.7%
- `afford` — 46 of 1,322, 3.5%
- `medicaid` — 17 of 1,322, 1.3%
- `obamacare` — 14 of 1,322, 1.1%
- `marketplace` — 14 of 1,322, 1.1%
- `trump` — 6 of 1,322, 0.5%
- `underwrit` — 3 of 1,322, 0.2%
- `open enrollment` — 1 of 1,322, 0.08%
- `spam` — 1 of 1,322, 0.08%

Individual comment ids for the most load-bearing quotes:

- The single open-enrollment mention, 2026-04-25 — `023c37e1-2748-efef-4383-e4a1a7d7df54`
- Medicare and Medicaid caption correction, 13 likes, 2025-07-20 — `207fb93d-357e-da7a-8511-6eab8265828a`
- Guaranteed issue explained by a commenter, 2026-08-21 — `96452dd4-651e-9034-cd92-5fa35c41e6e1`
- "$2100/month... How is $2,100/month 'affordable' insurance???", 9 likes, 2025-07-21 — `df773e22-e868-6360-d77a-e55132f0345d`
- "spam phone calls every 10 minutes for months", 5 likes, 2026-03-29 — `71641880-734a-b77f-ceb1-abe83694586d`
- "never put your info online unless you want 100 calls a day", 2026-07-16 — `130ef5af-fa52-7d27-3b94-bcb84e327a3c`
- The broker asking her to understate income, 2026-02-24 — `4c3ad278-1bd4-6637-e12a-ae5e592bbeb6`
- "There is no middle class on the marketplace", 2025-08-09 — `8a885e35-71be-e442-a0da-f462b6eb3e9f`
- Enhanced subsidies cut, described by a commenter, 2026-04-24 — `87bf7f5d-1445-c1d8-1813-51f904002be8`
- Pre-existing conditions and private plans explained, 3 likes, 2025-08-28 — `162dd382-ba52-d990-e760-19dd74bf7ff1`
- Competing agent poaching in the comments, 2025-07-17 — `87abec51-416d-15b6-61c9-e7b6633465fa`
- "Its underwritten, if you have health concerns, be warned", 3 likes, 2025-07-01 — `aeb4e727-7062-862d-8629-9ae52aeaae79`

### Public web sources

Category size and dynamics:

- https://www.kff.org/affordable-care-act/what-we-know-so-far-about-2026-aca-marketplace-enrollment-premiums-and-deductibles/
- https://www.kff.org/affordable-care-act/aca-marketplace-premium-payments-would-more-than-double-on-average-next-year-if-enhanced-premium-tax-credits-expire/
- https://www.kff.org/affordable-care-act/aca-marketplace-enrollment-is-down-in-2026-but-all-of-the-data-isnt-in-yet/
- https://chir.georgetown.edu/what-to-expect-for-open-enrollment-2026-edition/
- https://www.getinsureleads.com/blog/insurance-lead-industry-report-2026 — the $3.8B lead-generation figure, vendor published, no methodology

Trust events and regulation:

- https://www.ftc.gov/news-events/news/press-releases/2026/04/ftc-sues-stop-deceptive-health-care-scheme
- https://www.ftc.gov/legal-library/browse/cases-proceedings/2423043-innovative-partners-ftc-v
- https://www.insurance.nh.gov/news-and-media/new-hampshire-insurance-department-alerts-consumers-special-enrollment-period
- https://www.insurance.kansas.gov/consumers/notice-from-the-ftc-and-cms-on-innovative-partners-dba-american-collective
- https://www.ftc.gov/news-events/news/press-releases/2024/12/ftc-staff-sends-warning-letters-healthcare-plan-marketers-lead-generators
- https://www.ftc.gov/system/files/ftc_gov/pdf/2025-00542_healthcare_plan_marketers_and_lead_generators_warning_letters_0.pdf
- https://www.cms.gov/newsroom/press-releases/cms-statement-system-changes-stop-unauthorized-agent-broker-marketplace-activity
- https://www.cms.gov/newsroom/press-releases/cms-update-actions-prevent-unauthorized-agent-and-broker-marketplace-activity
- https://kffhealthnews.org/insurance/obamacare-aca-fraud-gao-enrollment-marketplace-brokers/
- https://www.mofo.com/resources/insights/250130-eleventh-circuit-vacates-fcc-s-tcpa-one-to-one-consent-rule
- https://www.consumerfinanceinsights.com/2025/09/15/the-ftc-issues-final-rule-formally-eliminating-the-one-to-one-consent-requirement/
- https://www.federalregister.gov/documents/2024/04/03/2024-06551/short-term-limited-duration-insurance-and-independent-noncoordinated-excepted-benefits-coverage
- https://www.healthinsurance.org/blog/finalized-federal-rule-reduces-total-duration-of-short-term-health-plans-to-4-months/
- https://www.dol.gov/agencies/ebsa/laws-and-regulations/laws/affordable-care-act/for-employers-and-advisers/short-term-limited-duration-insurance/stldi-statement-08-07-2025 — not read this run, named blank
- https://content.naic.org/committees/d/improper-marketing-health-insurance-wg
- https://chir.georgetown.edu/the-peddling-of-junk-plans-to-consumers-facing-higher-insurance-premiums/
- https://www.commonwealthfund.org/publications/explainer/2026/feb/what-consumers-need-know-health-coverage-doesnt-comply-aca

Sources attempted and blocked by this session's network egress proxy:

- https://healthformoms.co/save/
- https://www.facebook.com/business/help/298000447747885
- https://transparency.meta.com/policies/ad-standards/restricted-goods-services/health-wellness/
- https://www.kff.org/affordable-care-act/what-we-know-so-far-about-2026-aca-marketplace-enrollment-premiums-and-deductibles/
