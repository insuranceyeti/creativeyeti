---
brand: health-for-moms
doc: competitive-landscape
generated_on: 2026-09-04
refresh_by: 2026-12-03
sources_read:
  - "Parker MCP `search_competitor_facebook_ads` mode `brands`, brand aed0ff06-555d-4f4f-9bf8-31178e2fb977, run live 2026-09-04. Returned `totalCount: 0` and an empty brands array."
  - "Parker MCP `brand_discovery` operation `matches`, three runs: unfiltered, `industryFilter: finance`, and `industryFilter: medical`, 10 results each, run 2026-09-04. Corpus size reported as 3,716 brands, 763 persona-shortlisted."
  - "Parker MCP `brand_discovery` operation `compare`, Health For Moms against Globe Life, run 2026-09-04, read for the per-persona pair scores."
  - "Parker MCP `search_competitor_facebook_ads` mode `discover`, keyword `health insurance`, 15 ads, run 2026-09-04. Returned 15,335 matching ads across the corpus. Full media fields read on all 15: text hook, verbal hook, visual hook, angle, value props with timestamps, landing URL, video URL."
  - "Parker MCP `search_competitor_facebook_ads` mode `search_brand_by_name`, two batches, 18 names, run 2026-09-04."
  - "Parker MCP `search_facebook_ad_comments_sql`, eight keyword passes over the brand's 1,322-comment corpus: `Direct Primary Care`, `DPC`, `share`, `blueocean`, `pm me`, `DM me`, `licensed`, `help you`, `Confidant`, `marketplace`, `Medicaid`. Run 2026-09-04."
  - "Parker MCP `search_facebook_ads_sql`, lifetime lookup on ads 120239479305920519 and 120241073380060519, run 2026-09-04, with full creative fields and media URLs."
  - "Parker MCP `search_chat_history`, `listThreads` plus `getMessages` on Slack thread 1788479022.847859, run 2026-09-04."
  - "`source-pulls/ad-comments.md`, the full 1,322-comment read, used as the denominator source and cross-check."
  - "`source-pulls/ad-account.md`, the Phase-1 ad-account pull, 13 ads read at full media depth."
  - "`sub-context-docs/brand-identity-analysis.md` and `sub-context-docs/website-and-product-audit.md`, both read in full."
  - "`running-notes/missing-context.md` and `running-notes/brand-rules.md`."
  - "Creative-strategy method docs loaded before analysis: `analyzing-public-ad-accounts.md`, `creative-strategy-fundamentals.md`, `customer-review-mining-method.md`, plus the routing map in `expertise-routing.md`. No `brand-lens.md` exists for this brand yet."
data_limitations:
  - "This brand has zero tracked competitors. A live `search_competitor_facebook_ads` call in mode `brands` returned `totalCount: 0` with an empty array on 2026-09-04. The team deferred building a competitive set on 2026-09-03, per `running-notes/missing-context.md`. Every read in this doc that would normally come from a rival's ad library is therefore missing, and the deep-audit set is empty by fact, not by judgment. Adding real rivals in the Parker app is the single fix, and it backfills this whole branch without redoing anything else."
  - "Everything sourced from `brand_discovery` is marked `data-limited`. Those results are Parker's ranking of what happens to sit in its 3,716-brand database, scored on audience, positioning and tone. They are not a set this team chose, nobody has confirmed any of them is a real rival, and the ranking cannot surface a brand the database does not hold."
  - "Everything sourced from `discover` mode is marked `data-limited` for the same reason. An absence in Parker's corpus is an absence in a database, not proof of an absence in the US market."
  - "I did not open the media for the brands returned by `brand_discovery`. What I have is Parker's own evidence fields, which quote those brands' ad hooks and describe their visuals. Those reads are carried as Parker's, marked `inferred`, and are not my own viewing. The 15 ads from `discover` mode are different: those came back with full hooks, visual descriptions, value props and playable video URLs, so creative claims about those 15 are mine and are marked `verified`."
  - "No competitor ad comments are reachable, so there is no category baseline. I cannot say whether the rate of rival agents pitching in this brand's comment sections is high, low, or ordinary for health insurance lead generation."
  - "`author_name` is null on all 1,322 comment rows and `permalink_url` is null on all of them. Every count below is a count of comments, never of people. Where I attribute a run of comments to one operator, that is an inference from identical text and a tight time window, not from an identity."
  - "My comment counts come from substring searches, which is a narrower net than the full read in `source-pulls/ad-comments.md`. Where my number is lower than that doc's, mine is a floor that confirms the pattern rather than a correction to it. I say so at each point."
  - "The brand's own site is blocked from this environment, confirmed in two prior docs. So I could not read how Health For Moms frames its alternatives on its own pages."
  - "There is no `get_current_time` tool on this MCP surface. The date comes from the session clock, which rolled to 2026-09-04 during the run. Sibling docs in this build are stamped 2026-09-03."
---

# Competitive landscape — Health For Moms

## How this read was built, and the shape of what came back

Start with the thing that decides the character of this whole document. **Health For Moms tracks zero competitors.** I did not take that from the notes. I ran it live: `search_competitor_facebook_ads` in mode `brands` came back with `totalCount: 0` and an empty array, in 79 milliseconds. The team deferred building a competitive set on 2026-09-03 and that deferral stands. So the read a competitive landscape usually rests on, walking rival ad libraries, does not exist here, and no amount of writing can conjure it.

That left three honest routes, and I ran all three.

**Route one, ask Parker what it would suggest.** `brand_discovery` ranks external brands already sitting in Parker's database against this one, scoring audience, positioning and tone. I ran it three ways: with no filter, filtered to `finance`, and filtered to `medical`. Thirty results in total. Every one of them is `data-limited`, because this is Parker telling you what is in its own cupboard, not a set anyone chose.

**Route two, search the wider corpus by what ads actually say.** `discover` mode searches ad content across all 3,716 brands, tracked or not. The keyword `health insurance` matched 15,335 ads. I read the top 15 by impression rank at full media depth, with hooks, visuals, value props and playable video.

**Route three, mine the brand's own comment sections.** This is the only route that produced verified, primary evidence about real rivals, and it turned out to be the strongest thing in the document. Rival agents pitching competing offers under this brand's own paid creative are a genuine competitive signal, and they leave a text record with dates attached.

Two things shaped the read as I went.

The first is that Parker's own suggestions confirm the gap rather than fill it. Across all thirty discovery results, exactly one carries a `competitor` relationship lens, and that one is flagged `backfilled: true`, meaning the system supplied it rather than earning it. Everything else comes back as `affinity` at low strength or with no lens at all. Parker is being honest with itself: within the brands it holds, there is nothing that competes with this one for the same purchase.

The second is that the field is genuinely there in the customer's own words, just not in any ad library. Moms in these comment sections name the alternatives they are weighing, by name, unprompted. That gives a map of the field built from the buyer rather than from a database, and it is the part of this doc a strategist can actually use tomorrow.

One more piece of context I picked up on the way. At 23:43 UTC on 2026-09-03, roughly an hour before this run, a team member asked Parker in Slack: *"Do you have permissions to clean up comments or no?"* and then *"give me all ads LIVE its on so i can go hide them."* The team is actively moderating these comment sections right now. That matters for this doc, because the competitive evidence below lives in exactly the material they are hiding.

Method note. I read this field through `analyzing-public-ad-accounts.md`, and two of its ideas do most of the work here. The first is the three-tag taxonomy: competitor, inspo, affinity are separate fields, not one label, because the action each implies is different. The second is the cut between a **market competitor** and a **creative competitor**. A brand can be a giant rival for the purchase and a complete non-entity in the ad feed, and the two need different handling. For this brand that distinction is not academic. Its biggest market competitors are ones it has forbidden itself from ever naming.

---

## Direct competitors, the deep-audit set

**The deep-audit set is empty, and it is empty as a matter of fact.** No brand is slated for a deep audit, because no brand is tracked, and a deep audit is built from a rival's ad library. Naming a set here without the library behind it would be the exact failure this doc exists to avoid. `verified`, from the live pull that returned zero on 2026-09-04.

That said, the field is not empty. Below is what I can place as a direct rival on evidence, sorted by how solid that evidence is.

### Verified and named, but invisible to Parker: the brokers working the comment sections

These are direct competitors in the strictest sense. They chase the same purchase, from the same woman, at the same moment, on the same screen. They just do it for free, in the replies, under an ad Health For Moms paid for.

**Blue Ocean Employer Benefits.** The clearest case in the corpus. I found 15 comments from what reads as a single operator, all on `MOMS38 - 1 - V1`, all posted on 2026-04-07 inside a 54-minute window running from 22:31:59 to 23:26:03 UTC. Thirteen of them carry the link `www.blueoceanemployerbenefits.com/individual-plans`. The operator worked down the comment list addressing women by first name, one after another, with two rotating scripts.

Script one, posted four times to Rachel Reeves, Heather, Becky Haugen and Jaime McNall between 22:31 and 22:36: *"you can pair Direct Primary Care with a low premium health plan and have a comprehensive health plan. It's a holistic & proactive approach to primary care, where you pay a monthly membership fee to be part of a physician's panel. You can call/text. Have same day appts. Check mapper.dpcfrontier.com for a location near you. And then you can pair DPC with an unbundled health plan like this hybrid that is a month-to-month renewing plan, to meet major medical at 100% after IUA: www.blueoceanemployerbenefits.com/individual-plans"*

Script two, posted six times to Kästle Brandy, Jenn Harmon, Morgan Allen, Krystal Ahmad Sonsky, Leslie Hurt and Kristen Johnson between 22:49 and 22:55: *"consider a level-funded plan, with fair-priced coordination, paired with Healthshare. They spend your money like you would. Care coordination negotiates for you at time of service for preventive. And you present as self-pay for major, and they pay 100% after IUA. No copays. No coinsurance."*

Plus five shorter ones in the same window, including *"Bethany Blackburn check out this option, it's different!"* and *"Jeanine Stupka look into DPC. Mapper.dpcfrontier.com"*.

`verified` that the comments exist and say this, from `search_facebook_ad_comments_sql` on 2026-09-04. `inferred` that they come from one operator, resting on the identical scripts and the 54-minute window, since `author_name` is null on every row and there is no way to confirm a person.

**Health Insurance Confidant Consulting.** Two comments, both on `B1 samar- Copy`, both on 2025-07-25, 26 seconds apart, to Montana Garza and Michaela Dutson: *"my team can assist you if and when you need it. I think it's odd to market to moms but not offer anything for maternity...682-307-0039 Health Insurance Confidant Consulting"*. Same move, cruder, with a phone number instead of a URL. `verified`.

**Unnamed agents.** At least four more operators, identifiable by their offer rather than their brand. One works `MOMS38 - 1 - V2` on 2026-04-07 with *"You can get a health insurance without paying premiums $0/month (depending on your eligibility) as well as $0 deductible. Pm me if you need health insurance"* and two follow-ups asking women to send their zip code and age. One posts on `MOMS38 - 1 - V3` on 2026-04-13: *"I can help you get MUCH better rates! And not just for women or moms! Let me know if I can help :)"*, which drew 3 likes and 3 replies. One posts on `Moms43 - 4 - V3` on 2026-07-16, and this is the sharpest of them because it attacks the funnel and pitches in the same breath: *"As a licensed health insurance advisor, never put your info online unless you want 100 calls a day about health insurance. Also you dont have to be a single mom to find a zero deductible plan... DM and I can help you look at the plans available in your state and find fits your needs best."* And two push health shares, on `MOMS38 - 1 - V9` on 2026-04-24 and `MOMS39 - 2 - V2` on 2026-04-09. `verified`.

**The size of this, with its denominator.** My keyword sweeps found 26 comments that pitch a competing offer, spread across 7 distinct ad names, against a corpus of 1,322 comments. That is 2.0%. The full read in `source-pulls/ad-comments.md`, which went through all 1,322 comments one by one rather than by keyword, put it at 39 comments across 10 ads, or 3.0%, with 17 of those on `MOMS38 - 1 - V1`. My number is lower because a substring search misses pitches that use none of my search terms. Treat 39 as the number and my 26 as independent confirmation that the pattern is real and concentrated in the same place. My own count on `MOMS38 - 1 - V1` came to 15, against that doc's 17, which is close corroboration on the ad that matters most.

**Why they picked that ad, and why it is worth noticing.** `MOMS38 - 1 - V1` is the ad with the text hook *"Health Insurance is a scam 🙄"* and the verbal opener *"My deductible is $6,000."*, over a woman filming herself close up, visibly frustrated, gesturing with two fingers. Lifetime it has spent $54,173.20 and produced 2,689 leads at a $20.15 cost per lead. Its hold rate is **17.12%**. For contrast, the account's current top spender `Moms43 - 4 - V3` has spent slightly more at $55,794.26 and holds **3.81%**. `verified`, Parker MCP lifetime lookup, 2026-09-04.

So the raided ad is not the biggest spender. It is the one people actually watch, by a factor of about four and a half. My read, marked `inferred`: an agent farming comments goes where the argument is, and the argument is where attention is. The creative that holds a mom longest is the same creative that gives a rival the longest window to stand in front of her. Confidence: mixed. It rests on one raid on one ad, and one event is not a pattern.

**Why none of these can be given a deep audit today.** I checked. `search_brand_by_name` returns "Not in Parker's database" for Blue Ocean Employer Benefits, Health Insurance Confidant Consulting and DPC Frontier. `verified`, 2026-09-04. They do not run tracked Meta creative, so there is no library to walk. The right handling, under the cut between a market competitor and a creative competitor, is to treat them as real market competitors and creative non-entities: they cost this brand leads without ever buying an impression. Watching them is a job for whoever moderates the comments, not for whoever walks the ad libraries.

### The alternatives the brand names but has never tracked

The brand context document names three layers it sees itself against, quoted in `brand-identity-analysis.md`: the government marketplace, which it refuses to name in creative by choice; employer plans, which the document calls *"the most common 'competitor' — the default option families already have"*; and the big carriers, framed as *"faceless corporate entities with CEO salaries inflating costs."* It also names EverQuote and QuoteWizard as direct competitive alternatives. All `stated`. Section 6 of that document says plainly: *"The brand did not provide any specific competitors or competitor websites."*

I resolved the two named brands against Parker's corpus. **EverQuote** is there, brand id `4e05011e-475f-4e52-8088-043234e0c28f`, blue-verified, 55,364 page likes, with 8 ads scraped and a page bio reading *"The Largest Online Auto Insurance Marketplace in the U.S."* Auto, not health. **QuoteWizard** has two page entries, `8c5faf7c-bce1-4c24-962f-6c40aa2c3449` and `33ed3cdb-fa50-4bd0-af01-e4f824294f6d`, with **0 ads scraped on both**. `verified`, 2026-09-04.

The routing call, and it is the practical point of this section: **subscribing to those two today buys almost nothing.** Eight auto insurance ads and zero ads is not a library, and `analyzing-public-ad-accounts.md` is blunt that a handful of ads reads as too little to analyze at all. If the team wants a real deep-audit set, the move is not to track the two names already in the database. It is to ingest the Facebook pages of advertisers actually selling private health coverage to American mothers, which `brand_discovery` can do with `operation: 'ingest'` given a page URL.

### The direct rivals the customer names herself

This is the part the ad library could never have given, and it is `verified` primary evidence from the brand's own comment corpus.

**The ACA marketplace.** 14 comments across 8 distinct ad-name groups, spanning 2025-01-13 to 2026-08-21. Moms bring it up unprompted, both as the thing they compare against and as the thing they were told to use instead. One on `MOMS38 - 1 - V9`, 2026-04-04, with 4 likes: *"Ingrid Zagers have you checked marketplace? There has got to be better coverage. That's insane"*. One on `MOMS38 - 1 - V8`, 2026-03-19: *"I have a policy through the marketplace with zero deductible as long as I stay within network. You just gotta do your research and not pick the first one that you see"*, which claims the exact benefit this brand advertises, from the source this brand refuses to mention. And one on `B1 samar- Copy`, 2025-07-21, with 9 likes and 6 replies, arguing the other way: *"The best we could find on the stupid Marketplace is $2100/month for just myself and my husband. That's almost my entire salary... How is $2,100/month 'affordable' insurance???"*

This is the brand's largest direct competitor and it is the one the brand has gagged itself against. Its own non-negotiable rule bars *"No government/ACA references"* and *"The villain in any narrative is always the system/mechanism — never a named company or individual."* Both `stated`, brand context section 8. So the customer is standing in a comparison the creative is not allowed to enter.

**Medicaid.** 17 comments across 5 distinct ad-name groups, 2025-07-20 to 2026-04-26. Mostly people establishing who qualifies and who does not, which is precisely the gate this brand's funnel runs on. On `MOMS38 - 1 - V8`, 2026-04-15: *"That would be Medicaid. And you stop qualifying after you make more than $14.25 an hour."*

**Health share ministries.** Five comments name them outside the Blue Ocean run, across five ad-name groups, from 2025-01-12 to 2026-08-31. *"Medishare"* drew 4 likes on `IMG 6` in January 2025. *"Health share is the way to go my insurance went down 60% lmk if you want info"* on `MOMS39 - 2 - V2`, 2026-04-09. And a mom on `moms-63 3e` asking the question directly on 2026-08-31: *"Is this insurance or something like a Christian health share?"* I checked the corpus for the named brands. Medi-Share, Christian Healthcare Ministries, Zion HealthShare, Sedera and Crowd Health are all "Not in Parker's database." `verified`.

**Direct Primary Care.** 8 comments, all on `MOMS38 - 1 - V1`. Six trace to the Blue Ocean operator. Two come from customers with nothing to sell: one on 2026-03-19: *"DPC!! Screw insurance"*, and one on 2026-03-23 that pulled 9 likes and 10 replies: *"Direct primary care practices solve this problem, and many others."* Nine likes and ten replies makes it the most engaged comment pitching an alternative anywhere in the corpus, and it came from someone with nothing to sell.

**Going without insurance.** The read in `source-pulls/ad-comments.md` counted 33 comments across 10 ads arguing that the right move is to drop coverage and pay cash, including one with 14 likes: *"I would rather have no insurance you would get better self-pay rates then you do with 'having coverage'"*. This is the competitor with no brand, no ad account and no sales rep, and on the evidence it is more popular in these comment sections than any named rival.

**My read on the whole set, marked `inferred`.** The distinct ways a mom can go in this category are: an underwritten private plan through an agency, which is what Health For Moms sells; a guaranteed-issue marketplace plan; Medicaid; a health share; direct primary care paired with a thin catastrophic plan; whatever her employer offers; a generic quote comparison site; or nothing at all. Eight lanes. The brand's compliance rules forbid it from naming two of the biggest ones. Confidence: strong that these are the lanes, because they come from the customer unprompted across at least fourteen distinct ad-name groups and a twenty-month span. Thin on their relative size, because comments are not a market survey and nothing here connects a comment to a decision.

---

## Indirect and category-adjacent competitors

Everything in this section is `data-limited`. It comes from Parker ranking its own database, and the ranking cannot see a brand the database does not hold.

### What Parker suggests when you do not filter it

The unfiltered run returned ten brands: Hydrasana at 0.776, Peachies at 0.747, By Winona at 0.744, Miku Care at 0.719, Cardly at 0.706, Serenity Kids Baby Food at 0.706, Waterdrop at 0.703, Freja Bone Broth at 0.701, Marama Products México at 0.698, and may.app at 0.697.

Water purifiers, diapers, hormone therapy, baby monitors, greeting cards, baby food, drink mixes, bone broth, shampoo and a pregnancy tracking app. Not one sells insurance or anything financial.

Read what that actually tells you rather than dismissing it. The scoring weights audience at 2 and positioning and tone at 1 each, so when there is no product overlap in the database, audience and voice are all that is left to match on. Every one of these ten pairs against a Health For Moms persona archetype that Parker names as **The Protective New Mother** or **The Household Hero**. So the honest translation is: *within Parker's database, the closest thing to this brand is a set of brands that speak to a protective mother in a warm voice, like a friend who is also a mom.* That is an affinity read, and Parker labels it as one. Six of the ten carry `affinity` as their top lens and the other four carry no lens at all. None carries `competitor`. `verified` that these are the results; the interpretation is `inferred`.

Where an adjacency here could close into something real: **may.app**, a pregnancy and early-childhood health app, scores the highest single persona pair in the unfiltered set at 0.707, matching Parker's Protective New Mother against its Reassurance-Seeking New Parent. It reaches the same anxious new mother at the same life moment, about health, with a free digital front door. If it ever added a coverage or benefits feature, it would be standing in this brand's doorway with an audience already assembled. That is speculative and marked `inferred`, and it is exactly the kind of adjacency the prompt asks to be flagged, because adjacency closes fast.

### What Parker suggests when you filter to medical

Ten results: By Winona 0.744, Maven Clinic 0.690, Sollis Health 0.674, Join Amble 0.673, ezra 0.670, Dr. Will Cole 0.663, Fridays 0.661, Elektra Health 0.658, Ideal Image 0.648, Beltwell 0.642.

These are health services, not coverage. But two of them are genuinely adjacent in a way worth naming, and the evidence is in Parker's own persona pairing.

**Join Amble** pairs against Health For Moms at 0.661 on a persona Parker calls **The Insurance-Denied Patient**, with the supporting evidence that a large share of its spend goes to ads about *"same price at every dose"* and overcoming lost insurance. **Fridays** pairs at 0.647 on **The Insurance-Denied Frustrated Dieter**, with the evidence that its ads use the headline *"My insurance said I didn't qualify for GLP-1 coverage."* Both matched against this brand's own archetype, **The High-Deductible Prisoner**.

That is a real adjacency and it points somewhere uncomfortable. These brands win the same woman by helping her route around insurance entirely rather than buy better insurance. They are selling the same emotion, that her coverage failed her, and closing it with the opposite conclusion. `inferred`, from Parker's evidence fields, which quote the ads themselves; I did not open their creative.

**Elektra Health** is worth a line for the opposite reason. Its evidence field notes ads leading with *"Get affordable, in-network menopause care"* and explicit mentions of Medicaid and Medicare, plus state callouts like *"Hey, New York."* It runs the state-by-state qualification move that is this brand's own closing mechanism, and it names the government programs this brand cannot. `inferred`, same caveat.

### What Parker suggests when you filter to finance

This is the run that should have produced the real rivals, and it is the most instructive failure in the document.

Ten results: A-MAX Auto Insurance 0.668, John Anderson 0.662, NégocierMonTaux.com 0.659, Ethos 0.656, Globe Life 0.652, Insurify 0.646, Adriana's Insurance Services 0.643, Canadian Life Rates 0.617, Senior Serenity Insurance 0.616, Right Life Insure Canada 0.612.

Every one of them sells insurance or debt help. **Not one sells health insurance.** Four are life insurance, three are auto, one is final expense, one is debt consolidation in France. Four are Canadian. `verified`.

Only one carries `competitor` as its top lens: **Globe Life**, and the result marks it `backfilled: true`, meaning the system filled the slot rather than the brand earning it. I tested that placement directly with a `compare` run, and it does not hold. Positioning similarity comes back at **0.412**, the lowest number in any of the thirty results, because Parker reads Health For Moms as a **challenger** at 0.9 confidence and Globe Life as **lifestyle_identity** at 0.8. Of the three persona pairs, only one clears 0.5, at 0.700 on The Protective New Mother; the other two land at 0.442 and 0.426. And it sells life insurance. **Globe Life is not a direct competitor to this brand and should not be treated as one.** `verified`, from the compare run on 2026-09-04.

**Ethos** is the most useful brand in this section. It is a term life insurer selling through a fast online application with no medical exam, and Parker's evidence field describes ads featuring *"women in their 30s and 40s filming from their cars, explicitly framing a $2M no-exam policy as a '#MomHack' to quickly solve the mental load of family protection."* Same buyer, same register, same promise to take the friction out, adjacent product. It is also the biggest advertiser in the corpus sitting one product away from health insurance, by a distance: 1,620 of its 1,977 corpus ads matched the keyword `health insurance`. `verified` for the counts; `inferred` for the creative read, since it comes from Parker's evidence field rather than my viewing.

Where Ethos could become direct: it already owns the lane Health For Moms occupies, one product over: financial protection sold to mothers with no medical exam. If it added health coverage, or if a health insurer copied its posture, this brand's positioning would stop being unusual.

---

## Emerging and micro-competitors to watch closely

`analyzing-public-ad-accounts.md` says to give this group extra attention in a commoditized category, because that is where the next real threat usually comes from. Health insurance lead generation is about as commoditized as a category gets, so this section carries more weight here than it would elsewhere.

### The brokers are the micro-competitors

The operators in the comment sections belong here as much as in the direct set, and they are the reason this section is not a formality. They are small, they are fast, they are in nobody's database, and they compete on effort rather than on media spend. One person spent 54 minutes on a single evening writing 15 personalized replies under one ad. That is a competitor with no CPM at all.

**The right cadence is a periodic check, and the check is cheap.** Re-run the same keyword sweeps over the comment corpus on the monthly comment refresh and see whether new operators, new URLs, or new phone numbers have appeared. Two things make now the moment to start. The first is that the raid on `MOMS38 - 1 - V1` was concentrated in a single hour five months ago, and that ad set is now `ADSET_PAUSED`, so the account may simply not have been raided since. The second is that the team began hiding comments on 2026-09-03. If they hide this material without logging it first, the record of who is intercepting disappears along with the damage.

### The small operators in the corpus, and the one mechanic worth watching

Route two gave a clean read here. The `discover` keyword `health insurance` matched 15,335 ads across the corpus, and I read the top 15 by impression rank at full media depth. Every one of those 15 sits at rank 1 and 13 of the 15 are currently active. Here is what they are.

Six are lead generation for senior life insurance, five of those Canadian: **National Protection Plan**, **Canada Quoter**, **Canadian Life Rates**, **InsuranceSaver.io**, plus two pages run under a person's name, **Michael Doyle** and **Maya Sinclair**, both pointing at National Protection Plan's tracking domain. One, **Senior Serenity Insurance**, sells US burial coverage. The other eight matched the keyword incidentally: 4ocean mentions health insurance as a crew benefit, Budpop uses "insurance policy" as a metaphor for sleep, Thriveworks and Talkiatry accept insurance, and three are supplement pages.

**Not one advertiser in the top 15 of a 15,335-ad keyword match sells health insurance to American mothers.** `verified`, 2026-09-04. Marked `data-limited`, because this is a database and not the market.

The mechanic worth watching is what those small operators open with. Their hooks tell you that you already qualify for something, using a benefit you already receive as the proof. InsuranceSaver.io, launched 2026-06-24 and running 71 days, opens on a hand placing a paper cutout labelled "GROCERY REBATE" onto a rustic wooden tabletop while a voice says *"If you received the Canada grocery rebate, you are officially eligible to check your 2026 senior benefit status."* National Protection Plan, launched 2026-03-26 and running 161 days, opens on a middle-aged woman in her kitchen with the overlay *"Stop If You Collected 🚨 CPP Before 65 🚨"*. Canadian Life Rates opens *"Urgent Message For PSWs 🚨"* over a split screen of a crowded hospital hallway. `verified`, from full media on all three.

Why that matters here. Health For Moms runs the same mechanic. Its state list is a qualification gate, sitting at 0:24 to 0:33 in the winning ads per `source-pulls/ad-account.md`. And its own paused `MOMS25 - 5TH DEC - Y1` ads ran the government version of it, with the verbal hook *"making over 50k just disqualified this family from affordable healthcare, but it secretly qualified them for something way better."* Those three ads hold $436.08 of lifetime spend and `brand-identity-analysis.md` flags them as tripping the brand's own no-government rule. So the mechanic these small operators are winning with is one this brand has already tested and then walked away from for compliance reasons, not for performance reasons. That is worth watching, and it is not the same as recommending it.

These operators are worth a periodic check for the mechanic, not for the buyer. They sell life insurance to Canadian seniors. Nobody here should confuse them with a rival for a Georgia mom's health plan.

### The named brands that are not in the database yet

Worth logging as the watch list, because each is a real US player and each came back "Not in Parker's database" on 2026-09-04: HealthMarkets, Assurance IQ, SelectQuote, Sidecar Health, Oscar Health, Medi-Share, Christian Healthcare Ministries, Zion HealthShare, Sedera, Crowd Health. `verified` that they are absent from Parker; whether each is a real rival to this brand is `stated` at best and unconfirmed. I am naming them as candidates to check, not asserting they compete.

---

## Open loops

**1. Why do rival agents work the comment sections of some Health For Moms ads and not others?**

The observation. Fifteen pitches from a single operator landed on one ad, `MOMS38 - 1 - V1`, inside 54 minutes on one evening, and almost nothing landed anywhere else. That ad is not the account's biggest spender. It is the one people watch longest, with a hold rate of 17.12% against 3.81% on the current top spender, a difference of more than four times.

The pull: **pattern**. The same behavior repeated fifteen times in under an hour, and it clustered on one specific creative rather than spreading across the account.

The question: **Why do rival agents work the comment sections of some Health For Moms ads and not others?**

Why it is a loop. If what draws a competing agent is the same thing that holds a mom's attention, then every time the team picks a creative it is trading reach against leakage, and right now nobody knows the exchange rate. Answering it would change which ads get moderated first and possibly which get scaled.

Territory: **messaging**.

**2. What are moms actually comparing Health For Moms against at the moment they decide?**

The observation. The brand's whole story runs on a single villain, the system, and its rules forbid naming any specific alternative. But in the comments the alternatives are named constantly and specifically: the marketplace 14 times across 8 ad-name groups, Medicaid 17 times across 5, health shares 5 times, direct primary care 8 times, and going without insurance 33 times across 10 ads. All on a 1,322-comment corpus.

The pull: **tension**. The brand says the fight is against a faceless system. The customer writes as if the fight is a shortlist of named options she is picking between, and both cannot be the right description of the decision.

The question: **What are moms actually comparing Health For Moms against at the moment they decide?**

Why it is a loop. If the real comparison is a short list of specific alternatives rather than a vague broken system, the creative is answering a question the buyer is not asking, and the brand is doing it under a rule that stops it from answering the one she is. That changes what the ads have to say, and the rule is self-imposed rather than legal, so it can be revisited.

Territory: **messaging**.

**3. Why is nobody else advertising health insurance to mothers?**

The observation. Parker holds 3,716 brands. The keyword `health insurance` matched 15,335 ads across them, and the top 15 by impression rank contain senior life insurance, burial coverage, telehealth and supplements, but no health coverage aimed at American mothers. Health For Moms has spent $743,218.09 in that exact lane since December 2024.

The pull: **gap**. An absence sitting where you would expect a crowd, in a category with plenty of money in it.

The question: **Why is nobody else advertising health insurance to mothers?**

Why it is a loop. `creative-strategy-fundamentals.md` says to interrogate an empty lane before claiming it, because an absence has three very different explanations: the lane failed for someone, a real constraint blocks it, or nobody has tried. If carriers or platform rules block it, this brand's position is far more fragile than it looks. If it is genuinely open, the moat is real and worth spending hard against. The answer points opposite directions on how aggressively to scale.

Territory: **product**.

*Two territories are left empty on purpose. Personas produced no loop this doc earned, because who this brand's rivals target is a question for the persona work, not for a map drawn at this altitude. Creators and talent produced none, because with no rival libraries there is no competitor casting to read.*

---

## Appendix - Parker media links

**Health For Moms own ads referenced in this doc**

- `MOMS38 - 1 - V1`, the ad the brokers raided. Parker: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239479305920519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977`
- `MOMS38 - 1 - V1` video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/50a0309be06d87e55299b9e00d7962b88516c847dec96e80cfd47e6ba5959b66.mp4`
- `MOMS38 - 1 - V1` landing page: `https://www.healthformoms.co/save/`
- `Moms43 - 4 - V3`, the current top spender used as the hold rate contrast. Parker: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977`
- `Moms43 - 4 - V3` video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4`

**Corpus ads read at full media depth, from `discover` mode**

- InsuranceSaver.io, archive 1363125325698464, launched 2026-06-24. Parker: `https://app.heyparker.ai/dashboard/ad-library?adId=1363125325698464&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977`
- InsuranceSaver.io video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/ext/0d3f4e88-1a35-434b-9c4b-7f7ae47465c8/32217216645926e07b3d217eb0bac3e52cfb5d5477c5d83126b5bf3a7fa237b1.mp4`
- InsuranceSaver.io landing: `https://insurancesaver.io/lp/clife/`
- National Protection Plan, archive 998325566192393, launched 2026-03-26. Parker: `https://app.heyparker.ai/dashboard/ad-library?adId=998325566192393&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977`
- Michael Doyle, archive 1994473094505853, launched 2026-06-12, pointing at National Protection Plan. Parker: `https://app.heyparker.ai/dashboard/ad-library?adId=1994473094505853&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977`
- Maya Sinclair, archive 1737181297650553, launched 2026-04-30, same tracking domain. Parker: `https://app.heyparker.ai/dashboard/ad-library?adId=1737181297650553&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977`
- Canadian Life Rates, archive 1445308893668748, launched 2026-02-25. Parker: `https://app.heyparker.ai/dashboard/ad-library?adId=1445308893668748&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977`
- Canada Quoter, archive 1971353183577146, launched 2026-08-04. Parker: `https://app.heyparker.ai/dashboard/ad-library?adId=1971353183577146&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977`
- Senior Serenity Insurance, archive 1529615138856888, launched 2026-07-08. Parker: `https://app.heyparker.ai/dashboard/ad-library?adId=1529615138856888&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977`

**Brand discovery**

- Discovery tab deep link returned by every `matches` run: `/dashboard/brand-discovery?tab=brands`
- Ethos logo: `https://scontent-iad3-2.xx.fbcdn.net/v/t39.30808-1/352519702_651919840166554_3794842382125977636_n.png`
- Globe Life logo: `https://scontent-lax3-1.xx.fbcdn.net/v/t39.30808-1/327210878_528309752699304_8688079694297119757_n.png`
- may.app logo: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/39cf34c6-1bf7-498e-ba69-109db7ca94bd/logo.jpg`
- Join Amble logo: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/924e7333-e441-4883-a75a-e977de4bd0a0/logo.jpg`

**Brand ids for anything the team decides to track**

- EverQuote: `4e05011e-475f-4e52-8088-043234e0c28f`, Facebook page 633198056761517
- QuoteWizard: `8c5faf7c-bce1-4c24-962f-6c40aa2c3449`, page 977342492345200, and `33ed3cdb-fa50-4bd0-af01-e4f824294f6d`, page 85500877099
- Ethos: `fcc3a6f6-46ae-40f4-8071-6341dbd5e1fb`
- Globe Life: `6e0578ab-6674-4ab4-8a89-b29fe1d1c24e`
- UnitedHealthcare: `6a49fae1-d447-4df7-b1e8-54a531410b43`
- Humana: `3b6ad3ed-92de-451e-8a36-e2b47703c12f`
- Compare Rates Today: `1e74b1a5-e9eb-4350-ba90-7c553cae28e3`
- InsuranceSaver.io: `0d3f4e88-1a35-434b-9c4b-7f7ae47465c8`
- Three River Insurance: `e2ce6c09-e7ff-4d70-b571-4549ae61ca56`
- American Health Support: `0203c092-24ba-4ef2-b4b9-65488efe24ab`

**URLs named by rival operators inside this brand's comment sections, quoted exactly as posted**

- `www.blueoceanemployerbenefits.com/individual-plans`
- `mapper.dpcfrontier.com`

**Prior source docs whose media handles support this read**

- `source-pulls/ad-comments.md`, the full 1,322-comment read
- `source-pulls/ad-account.md`, 13 ads at full media depth
