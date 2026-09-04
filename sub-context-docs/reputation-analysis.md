---
brand: health-for-moms
doc: reputation-analysis
generated_on: 2026-09-04
refresh_by: 2026-12-05
consideration_level: considered
sources_pulled:
  - ad-comments — the full 1,322-comment Facebook and Instagram corpus, pulled live 2026-09-04 via Parker MCP, treated here as this brand's only live public reputation surface rather than as the light secondary read the prompt normally assigns it
  - reddit-blogs-web — public web search only, run live 2026-09-04. Reddit itself is unreachable
sources_missing:
  - customer-reviews — zero rows, re-verified live 2026-09-04 through Parker MCP search_customer_reviews_sql. totalReviews returned 0
  - reddit — unreachable from this session and from the search provider. Confirmed by three routes on 2026-09-03 and not retried today, since the block is at the crawler user-agent level rather than in this sandbox
  - organic-social — no discoverable creator or customer post corpus about this brand on any platform, and no brand-owned organic presence found beyond the Facebook page that carries the ads
  - post-purchase-survey — zero responses, no platform connected
  - marketplace-ratings — no marketplace, no Trustpilot, no Better Business Bureau profile, no app store. Nothing to rate
pass_status: partial
sources_read:
  - Parker MCP search_facebook_ad_comments_sql, brand aed0ff06-555d-4f4f-9bf8-31178e2fb977, four string cuts run 2026-09-04 — "pregnan", "out of pocket", "reddit", and a broad "a" cut sorted by like count
  - Parker MCP search_facebook_ad_comments_semantic, three passes run 2026-09-04, each reporting totalCommentsAnalyzed 1322
  - Parker MCP search_facebook_ads_sql, act 484897827497337 HealthForMoms, last 90 days 2026-06-05 to 2026-09-02, grouped by ad name with the engagement metric set
  - Parker MCP search_customer_reviews_sql, unfiltered, run 2026-09-04
  - Public web search run 2026-09-04, six queries — the brand name, the brand name with legit and scam and reviews, the operating entity with Better Business Bureau, brand press and news, the category search a buyer would actually run, and the FBI discount medical insurance alert
  - running-notes/missing-context.md, source-pulls/ad-comments.md, source-pulls/reddit.md, sub-context-docs/website-and-product-audit.md including its 2026-09-04 correction block, sub-context-docs/category-and-market-research.md
  - Method docs — customer-review-mining-method.md, creative-strategy-fundamentals.md, persona-research-and-creative-strategy-process.md, emotional-delivery-and-timing.md, expertise-routing.md
product_era_timeline: null
---

# Reputation analysis — Health For Moms

## How this pass was built, and what it can carry

A reputation read is supposed to be the easy one. You do what a customer does. You look the brand up and write down what comes back.

For this brand, almost nothing comes back, and that turned out to be the finding rather than an obstacle to it.

Here is exactly what was tried. Customer reviews were re-checked live today through Parker rather than carried forward from a note, and the tool returned `totalReviews: 0`. Post-purchase surveys are zero. Reddit is unreachable, and the refusal names the search provider's crawler rather than this sandbox, so it is a standing wall and not a glitch. WebFetch is blocked for essentially every primary source including the brand's own site. That means three of the four surfaces a normal reputation pass leans on are gone. This pass is **partial** and it says so in the frontmatter.

What is left is two things, and both are real. First, public web search works, so the actual first page a prospective customer sees was read directly today. Second, the brand's own comment corpus is live, large, and public: **1,322 comments on 112 ad IDs and 79 ad names, dated 2025-01-08 through 2026-09-03**, confirmed at that exact total by three separate semantic passes today. The prompt normally treats ad comments as a light supporting read. For this brand that ranking has to flip, and I want to be honest about why rather than quietly promoting it. A researching customer here does not reach a review site, because there is no review site. She reaches the comment section under the ad she just watched. So for Health For Moms the comment section is not a proxy for the reputation surface. It **is** the reputation surface, and it is the one the brand pays to create.

Two disciplines from the mining method govern every number below. A count is not significance, so every figure carries its denominator of 1,322 and its spread across distinct ads, because spread across many ads is stronger evidence than volume inside one. And the corpus is lopsided: roughly 60% of it sits on the `MOMS38 - 1` creative family and 38% was posted in April 2026 alone. Any rate here is a rate inside that skew.

One more discipline, and it is the one this doc type fails at most often. The brand's own positioning is sitting in my context, and the trap is to hand it back dressed as customer perception. So I held the two apart on purpose and forced the read toward the places where they **disagree**. There are five such places and they are the spine of this document.

I did not verify a single number by re-reading a sibling doc. Where an upstream figure and my own live pull differ, I report mine and say what the difference is.

---

## Headline reputation read

**The honest verdict is structurally invisible, and exposed inside the one room where it is visible.** Marked `inferred`, resting on the search read, the empty review and press surfaces, and the comment corpus below.

This brand has essentially no third-party reputation. Not a good one, not a bad one. Search its name and you get its own website and a wall of unrelated federal maternal-health content. Search its name with "reviews" or "scam" and you get consumer-protection literature from the FBI and the FTC about this category, not one word about this company. There is no press. There are no reviews anywhere, on any surface, verified live today. There is no Better Business Bureau profile for the operating entity. There is no discoverable organic social presence. In twenty months of advertising the brand has produced 1,322 public comments and zero findable independent coverage.

The prompt warns not to read that silence as safety, and in this category the warning is not theoretical. It is the concrete mechanism of the damage. When a mother cannot find anything about a health insurance company, the first page does not stay empty. It fills with the category's warning literature: the FBI's April 2025 alert on discount medical insurance scams, the FTC's "Spot Health Insurance Scams" consumer page, a state attorney general's health care scams guide. **The default answer to "I can't find anything about this company" in US health insurance in 2026 is a scam warning.** So invisibility here is not neutral. It converts into suspicion automatically, without anyone writing a bad word about the brand.

The brand's own customers already ran this exact test and reported the result under the ads. On 2025-08-07: *"How come when I search for this on Google, nothing comes up?"* On 2025-07-24: *"A Google search doesn't pull anything about this. Is it legit?"* On 2025-01-20: *"I tried to look at them through a regular internet browser and nothing comes up...the link only works through Facebook and they want all your information before they show you anything...sounds like a scam to me."* All three `verified` in the corpus.

Then there is the second half of the verdict. Inside the one place the brand is visible, it does not hold the floor. The discourse under its own paid creative is owned by three groups that are not the brand: people correcting the hook's central claim, people warning others off the form, and rival agents selling against it. The brand has never replied. Not once in 1,322 comments, which I tested for directly and report below.

So the strongest single sentence for a strategist to carry: **this brand has manufactured its entire reputation surface with paid media and then left it unattended, in a category where regulators are actively teaching the audience to distrust exactly this kind of company.** Confidence: **strong** on the invisibility, since four independent surfaces are empty and I checked each one live. **Mixed** on the hostility, because a comment section skews negative by nature and there is no buyer source anywhere to weigh it against.

### The five places perception and positioning disagree

This is the part that makes it a reputation read rather than a summary of the About page.

| What the brand says | What the outside world shows | Mark |
|---|---|---|
| Ad headline on the account's top creative: *"Approved by thousands of Mom's across America"* | Zero reviews, zero press, zero Better Business Bureau profile, no testimonial surface found. Not one of those thousands is publicly visible | `verified` on both halves |
| Partner agents described as *"Mom BFFs"*, friendly and pressure-free | The most-liked comment about the brand's actual service, 33 likes on 2026-03-16, describes daily calls from unknown companies after one form fill | `verified` |
| The name Health For Moms | 38 comments across 15 ads say the product excludes pregnant women and women planning a pregnancy, and 9 of them use the brand's own name as the setup | `verified` |
| *"Nationwide coverage"* | Recurring reports of state-list rejection, including *"Why is this being shown in IL if it's not on the list???"* on 2026-09-02 | `verified` |
| Body copy on live ads: *"comprehensive health plans"* | The evidence in `website-and-product-audit.md` points to medically underwritten plans with pregnancy, health and possibly income screens. Selling non-comprehensive coverage as comprehensive is the exact conduct the FTC alleged in its April 2026 case against a Florida operator | `inferred`, and the legal read belongs to the brand's counsel, not to me |

An output that confirmed the About page would have missed every one of these.

---

## Sentiment trajectory

**Not yet available as a computed trajectory.** This is the first version of this doc, so there is no prior read to measure movement against. Marked `data-limited` and recorded below in a shape the next refresh can compute from.

What the corpus can show today is the internal shape of twenty months of comments, which is a baseline rather than a trend line. Four movements are visible and each is `verified` from the comment dates.

**The pregnancy objection is flat and persistent, not fading.** It runs 2025-07-01 to 2026-06-09 in the string cut, and it is alive on today's top-spending creative: on 2026-08-05, under `Moms43 - 4 - V3`, someone asked *"why don't any of the plans offer prenatal care?"* Fourteen months, every creative refresh, still landing. This one has not moved at all.

**The call-flood objection changed shape rather than volume.** In 2025 it reads as a first-hand report from someone who filled the form: *"Absolutely do not give them your info. You will receive calls and texts nonstop from an insane amount of reps"* on 2025-09-17, 6 likes. By mid-2026 it reads as fear from someone who has not: *"How many calls will I get if I try to see how this works?"* on 2026-05-17, 17 likes, which puts it inside the ten most-liked comments in the corpus. That shift matters. The warning has stopped being testimony and started being folklore, which means it now travels without anyone new being burned.

**The synthetic-talent objection faded.** 32 comments call the creative AI-made, but 25 of them sit on one 2025 ad and the objection has been near silent since April 2026. Read as a creative era passing rather than an audience changing its mind, and marked `thin` because one ad is one ad.

**Nothing has ever moved the legitimacy question, because nothing has ever been said about it publicly.** The single outside verdict that has reached this brand's world arrived on 2025-01-13 and has never been answered, matched, or displaced. That is twenty months of a static negative.

**What the next refresh should measure against this baseline**, so trajectory becomes computable: the pregnancy comment count and its ad spread against 38 and 15; the "out of pocket" correction count and spread against 74 and 12; brand replies against zero; findable third-party reviews against zero; press mentions against zero; and whether a Better Business Bureau profile has appeared.

**Era blindness, named as a limit.** The brand has supplied no timeline of material product changes, so `product_era_timeline` is null and no sentiment can be split by product era. Two era boundaries are visible from the outside and worth carrying: the creative moved from AI-presented spokeswomen in 2025 to live-creator and POV formats in 2026, and a second funnel domain at `quiz.healthformoms.com` went live on 2026-09-02. Neither is a product change, and whether the underlying plans have changed is unknown. Until the brand supplies that timeline, every sentiment read here averages across whatever the product has been for twenty months.

---

## Search-results read

This is the section that carries the verdict, and every result below was pulled live on 2026-09-04.

**Does the brand own its own name? No, and the reason is unusual.** A search for the brand plus its domain returns the brand's own site and Facebook page, and then falls straight into unrelated territory: a Wikipedia entry for Connect for Health Colorado, a Wikipedia entry for the Newborns' and Mothers' Health Protection Act, a Missouri state program called Healthy Moms Healthy Babies, and a rival called Better Health Plans For Moms at `betterhealthformoms.com`. The brand's name is made of four of the most common words in American health policy, so it cannot separate itself from a decade of government and nonprofit content that uses the same words. Marked `verified` from the result set.

That got worse in 2026. A press search for the brand returned, at the top, the HHS launch of **Moms.gov** on Mother's Day 2026, plus congressional maternal-health bills and national maternal-health polling. A federal website for mothers now sits on top of the words this brand built its identity from. Marked `verified` as reported by the search results, `inferred` as to the effect on the brand's findability.

**What sits in the purchase path.** This is the one that matters. The search a suspicious buyer actually runs is the brand name plus "legit" or "scam" or "reviews." Run today, that search returned, in order: the FBI's page on **Emerging Discount Medical Insurance Scams**, healthinsurance.org on how to avoid scams while shopping for health insurance, an Instagram tag page, the Tennessee Attorney General on health care scams, the FTC's **Spot Health Insurance Scams**, a Trustpilot page for a different company, the brand's own site, and an FTC blog post on avoiding fake healthcare plans.

Read what is missing from that list. There is no review of this brand. There is no complaint about this brand. There is no defense of this brand. There is no competitor comparison naming this brand. The search engine had nothing about the company, so it answered the intent instead, and the intent was "is this a scam." Marked `verified` as the live result set.

The FBI alert is worth reading closely because it is now a fixture of this brand's search path. Issued 2025-04-30, it describes offers that promise reduced rates on medical insurance without providing actual coverage, reached through unsolicited contact, using time-limited pressure. Its recommended consumer check is to verify the provider with the state insurance department **or the Better Business Bureau**. Marked `verified` as reported via search.

I ran that check. A search for the operating entity, Insurance Yeti LLC in Orlando, returned no Better Business Bureau profile. It surfaced a different company, Yeti Insurance Agency LLC in Irving, Texas, which is not accredited and is not the same business. So the exact verification step the FBI tells a worried consumer to take is one this brand currently fails, not because anything bad is filed but because nothing is filed at all. Marked `verified` that no profile was found, and `data-limited` on whether one exists under another name.

**How the brand ranks against rivals on the search a buyer runs.** I ran the category query a real person would type: best health insurance for stay-at-home moms in 2026. Health For Moms did not appear anywhere in the results. HealthPlusLife did, and it is one of the four rivals the brand names in its own competitor list. So did NerdWallet, wealthysinglemommy.com and myprivatehealthinsurance.com. Marked `verified`. The brand has zero share of the organic search a buyer would actually use to find a company like it, while a named competitor holds a place on the first page.

**The pre-purchase questions surfacing in the research moment.** The web results themselves show what the category's research questions are, and they are all verification questions rather than product questions: is this company real, is it licensed, will my doctor take it, what is actually covered, will I get called. The corpus shows the same shape. The highest-liked question in all 1,322 comments is not about price or coverage. It is *"Anyone actually have this and have insight?"* on 2026-03-20, with 15 likes and 6 replies. Logged here as the objection set for the persona work to map, not acted on.

---

## Press and news sentiment

**Absent. A clean, named blank.**

There is no press about Health For Moms. Not positive, not negative, not routine, not paid. A dedicated press and news search run 2026-09-04 returned nothing about the company and instead returned federal and congressional maternal-health coverage that happens to share the words in the brand's name. Marked `verified` that the search returned nothing about the brand, and `data-limited` on whether coverage exists somewhere a search engine cannot reach.

The one place the brand and the press occupy the same space is unflattering and indirect. The category's press is enforcement press. `category-and-market-research.md` documented six verified trust events aimed at this exact layer of the industry, and today's pass adds a seventh that the earlier read did not have: the **FBI's April 2025 public service announcement on discount medical insurance scams**, which sits directly on the first page of results for this brand's own name plus "scam." Marked `verified` as reported via search on 2026-09-04.

Against the pay-to-play caution, there is nothing to weigh. There is no thin mention to distinguish from a real endorsement, because there is no mention.

**Contrast against rivals.** HealthPlusLife holds a first-page organic position on the category search. Whether that is earned press or search-optimized content is not knowable from the result alone, so it is marked `stated` at best. But the comparison stands: a rival appears in the buyer's research path and this brand does not.

**Unused press assets: none, because none exist.** The absence is the recommendation. There is no strong piece of coverage sitting unused. There is no coverage.

---

## Overall sentiment across social and community

**Read plainly: negative where it exists, and thin to nonexistent everywhere the brand does not pay for it.** Marked `inferred`, weighing the loud-and-negative bias explicitly below.

### The wider web and communities

**Reddit: blank.** Unreachable, and the block is at the search provider's crawler rather than in this session, so it is a standing gap. The only Reddit artifact that has ever entered this brand's world is second-hand and it is severe. On 2025-01-13, under the ad `IMG 6`, a commenter pasted what reads as a search summary of Reddit discussion. I pulled it fresh today and it is exactly one comment out of 1,322, at **14 likes and 10 replies**. The load-bearing sentence, verbatim:

> *"According to discussions on Reddit, 'Health for Moms' insurance is generally considered not legitimate and likely a scam, as many users report extremely limited coverage, difficulty cancelling policies, and concerns about the company's practices not aligning with standard health insurance expectations; it's often advised to research and purchase health insurance through reputable sources like the Health Insurance Marketplace instead."*

Marked `stated`, firmly, and not promoted. This is a commenter's summary of a forum nobody has verified. It carries no subreddit, no thread, no post, no date for the underlying discussion. It settles nothing about whether the brand is legitimate. What it does establish is smaller and still important: a verdict on this brand exists somewhere the brain cannot see, at least one prospective customer went looking for it, what she found was hostile, and fourteen people agreed with her under a live ad. One comment out of 1,322 is 0.08%, which is as thin as a count gets. It is logged because it is the **only** outside verdict that has ever reached this brand, not because one comment supports a pattern.

**Blogs and long-form: blank.** No comparison article, no review blog, no "is Health For Moms worth it" content surfaced in any of the six searches run today.

### Organic social

**Blank on the brand's own presence, and blank on conversation about it.** A dedicated search for the brand's Instagram and TikTok presence returned nothing about the company. The only brand-owned surface that surfaced anywhere is the Facebook page at `facebook.com/p/Health-For-Moms-61569029311372/`, listed in Orlando FL, which is the page the ads run from. Marked `verified` that the search found nothing further, `data-limited` on whether accounts exist that search cannot see.

One number from today's ad pull sharpens the outside impression that page leaves. The account's top ad, `Moms43 - 4 - V3`, delivered **1,972,848 impressions** in the last 90 days and earned **114 page likes**. That is 0.0058% of impressions. Marked `verified`, Parker MCP ad pull, 2026-06-05 to 2026-09-02. Nearly two million views of this brand's creative produced almost no interest in following the brand. For a researching customer clicking through to check the page, the impression is of a company that runs ads and does not otherwise exist.

There is no creator or customer post corpus about this product anywhere I could reach. The nearest thing is the category conversation in the brand's own TikTok mining library, and that is about the category rather than about Health For Moms.

### The comment corpus, which is the only live surface

This is where the sentiment actually lives, so it gets the weight, with the mining method's discipline applied to every count.

Three patterns clear the bar of appearing across many different ads over many months, which is the only kind of durability a single-source corpus can demonstrate.

**One. The product excludes pregnant women, and the brand's name is the setup for the complaint.** My own string cut today on "pregnan" returns **38 of 1,322 comments, 2.9%, spread across 15 distinct ad names, dated 2025-07-01 to 2026-06-09.** The upstream figure of 42 across 15 comes from a wider classification that also catches maternity phrasing without the root word, and both readings agree on the spread. Rate is the wrong measure here and the mining method says so: these carry unusually high likes, they recur for fourteen months, and they name the brand's own promise back at it. Exact, with dates:

- 2026-04-01, 7 likes, `MOMS38 - 1 - V3`: *"Ours is 2,500 but we pay $1700 a month and pay $25 for reg appts and $75 for special drs. Its freaking nuts but your insurance says im not eligible because im pregnant 😂 huh.. so much for being for Moms 😂"*
- 2025-07-24, 5 likes, `B1 samar- Copy`: *"It seems they don't have coverage for expecting mothers. I am currently pregnant and received information from them that they currently do not have coverage for me as well."*
- 2026-04-08, 4 likes, `MOMS39 - 2 - V2`: *"Plans not available for those that don't plan or can't get pregnant anymore bc of an unexpected hysterectomy last year - yet have kids already… (health for moms) makes sense 👍🏼"*
- 2026-02-03, `MOMS30 - 1 - V20`: *"Health for Moms, but only if your babies are out of the womb. I was denied for being pregnant. Scam."*
- 2025-11-23, `B1 samar- Copy`: *"Marketing towards mothers while not covering pregnancy is a disgusting tactic."*
- 2026-08-05, `Moms43 - 4 - V3`, the account's top-spending live creative: *"why don't any of the plans offer prenatal care?"*

Confidence: **strong** that the pattern is real and current, resting on spread across 15 ads and a live example last month. **Mixed** on how much it costs, since nothing here connects a comment to a lead.

**Two. The audience publicly corrects the hook's central word.** My own string cut on "out of pocket" returns **74 of 1,322, 5.6%, across 12 distinct ad names.** The upstream figure of 103 across 13 uses a wider classification that also catches corrections phrased without that exact string, and the direction is identical. This is the largest single conversation in the corpus after the deductible disclosures themselves. Exact:

- 2026-04-07, `MOMS38 - 1 - V1`: *"As a licensed insurance broker this is VERY misleading in the beginning. The first half is talking about a medical maximum out of pocket. A deductible is something you pay before your insurance kicks in with co insurance."*
- 2026-03-29, 2 likes, `MOMS38 - 1 - V5`: *"That's not a deductible that's a medical maximum out of pocket. You should educate people, not misinform!!"*
- 2026-03-31, `MOMS38 - 1 - V5`: *"I'm a licensed insurance brokers."*
- 2026-03-25, `MOMS38 - 1 - V1`: *"As someone that bills medical claims to insurances, and adores my offices patients, I find it all nauseating."*
- 2026-05-01, `MOMS38 - 1 - V1`: *"Deductible is different than maximum out of pocket 😃 -an insurance agent"*

The reputation angle is not that the brand made a technical error. It is who is watching. Self-identified brokers, agents and medical billers are reading these ads and saying in public that the brand's biggest claim is wrong, on the account's highest-spend creative, and the brand never answers. Confidence: **strong** that the pattern exists, on 74 comments across 12 ads against 1,322.

**Three. People warn each other off the form.** This is the negative viral coefficient and it gets its own section below.

**Weighing the negative bias honestly.** Comment sections attract annoyed people, and a cold-traffic insurance ad attracts a large volume of general venting about American health care that has nothing to do with this brand. That is real and it deflates part of what looks damning. Two of the three patterns above survive the deflation cleanly, because they are first-hand accounts of this brand's own funnel rather than opinions about insurance. The scam word is the one that needs the discount: 45 of 1,322 comments use it, and reading them, most are aimed at the category. Brand-directed use runs at roughly 1.2%. That is not a wall.

**What is genuinely missing from the sentiment picture, and it is not a small thing.** In 1,322 comments there are exactly two accounts of the service working, and both describe an agent who could not help and was thanked anyway. On 2026-04-17, 2 likes: *"Best advice I have gotten from an insurance agent! She didn't have anything that fit but pointed me in the right direction!"* On 2026-04-01: *"I was connected to a very helpful agent. They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful."* Two out of 1,322 is 0.15%. The asymmetry between documented friction and documented satisfaction is itself the read, and it is exactly the gap a first-party review surface would close.

---

## Marketplace ratings and standing

**Blank across every surface, and the blank is total.**

There is no marketplace for this product. It is a free lead-matching service, so there is no retail listing, no Amazon page, no app store rating, no third-party seller profile. That much is structural rather than a failing.

What is a failing is that the surfaces that **do** exist for a service business are all empty too. Verified live 2026-09-04:

- **First-party reviews:** zero. Parker returned `totalReviews: 0`.
- **Post-purchase survey:** zero responses, no platform connected.
- **Better Business Bureau:** no profile found for Insurance Yeti LLC, the entity named on the brand's own terms page.
- **Trustpilot or comparable aggregator:** none found. The Trustpilot result that surfaced belongs to healthinsurance.com, a different company.
- **Google or Facebook page ratings:** not readable from this session, since Facebook is blocked to WebFetch. Marked `data-limited`.

There is no online-versus-retail split to read, because there is no retail. There is no strong or weak rating to report, because there is no rating anywhere.

Per the mining method's source-coverage discipline: this pass is missing the entire review layer, so **no sentiment share in this document is statistically representative**. Everything here is directional and single-source.

Standing up a first-party review surface is the single highest-value data move available to this brand, and it is the second time this build has reached that conclusion from a different direction.

---

## Authority and endorsements

**The log is empty, and there is one owned claim standing in for it.**

Searched and not found on 2026-09-04: press features, awards, television or podcast appearances, founder media moments, named carrier partners, named partner agencies, third-party certifications, industry recognition, comparison-article placements. Marked `verified` that six searches surfaced none of these, `data-limited` on anything a search engine cannot reach.

The category's equivalent of a gift-guide placement is the "best health insurance for moms" comparison article, and those exist in volume. HealthPlusLife, wealthysinglemommy.com, myprivatehealthinsurance.com and NerdWallet all hold positions on that search. Health For Moms holds none. **That is the gap, and the gap is itself the recommendation:** a brand built entirely on one audience is absent from every published list serving that audience, while a rival it names as a competitor is on the first page.

**The one authority claim the brand does make, and why it needs attention.** Today's ad pull shows the headline field on the account's top creative reads *"Approved by thousands of Mom's across America."* It runs on `Moms43 - 4 - V3`, `Moms43 - 5 - V1`, `Moms43 - 4 - V1`, `Moms43 - 4 - V4` and `moms-63 2b`, which together spent **$71,643.33** in the 90 days to 2026-09-02, or 72.9% of the window's $98,276.81. Marked `verified`, Parker MCP ad pull.

That is a third-party validation claim. It is also, on every surface checkable from outside, unsupported: zero reviews, zero press, no ratings profile, and 1,322 public comments containing two pieces of praise. I am not saying the claim is false. Thousands of moms may well have used the service and liked it. I am saying that **nobody outside the company can see a single one of them**, and that a claim of mass approval running on nearly three quarters of live spend, in a category where the FTC sent warning letters to 21 health plan marketers and lead generators about deceptive claims in December 2024, is exposure rather than authority. Marked `verified` on the spend and the empty surfaces, `inferred` on the exposure, and routed to the brand and its counsel rather than resolved here.

The same ads' body copy calls the plans *"comprehensive health plans"* and promises *"saving you 20% or more."* Set against the underwriting evidence in `website-and-product-audit.md` and against the FTC's April 2026 case, which alleges a Florida operation sold what were described as comprehensive PPO plans and were, per the complaint, limited benefit products, that word deserves a compliance read before the November ramp. Marked `stated` as to the FTC allegation, which is an allegation and not a finding, and `inferred` as to this brand's exposure.

**Genuine authority assets the brand could build and currently has none of:** a named carrier, a named partner agency, a licensed agent on camera, a state license number, a review corpus, a Better Business Bureau listing. Every one of these is a thing a suspicious mother can check, and the FBI's own consumer guidance tells her to check two of them.

---

## Retail distribution footprint

**One channel. Everything runs through paid Meta, and nothing else exists.** Marked `verified` from today's account pull and from the search results.

Where a customer can encounter this brand:

- **Paid Meta, which is effectively the whole business.** Last 90 days, 2026-06-05 to 2026-09-02: $98,276.81 of spend, 4,276,473 impressions, 117 ad-name groups, 4,336 leads at a $22.67 cost per lead, zero purchases by design. Delivery ran 95.2% female, 81.2% aged 25 to 44, 99.5% mobile, and split 60.2% Facebook to 39.2% Instagram. Lifetime the account has spent $161,685.48 for 7,451 leads at $21.70.
- **The brand's own site**, reachable in practice only by clicking an ad, since the brand does not rank for the searches its buyer runs. Three destinations appear: `healthformoms.co/save/` as the workhorse, a `/save-cw` variant, and the brand-new `quiz.healthformoms.com` test that went live 2026-09-02.
- **A Facebook page** that carries the ads and attracts almost no follows.

Where a customer cannot encounter it: organic search, comparison articles, review sites, press, Reddit, discoverable organic social, retail, or any marketplace.

**This brand leans direct, and more narrowly than that phrase usually means. It leans on one rented channel.** The reputation consequence is the point of putting this section here. A retail-heavy brand has much of its result invisible to digital measurement. Health For Moms has the opposite problem. Every impression, every comment and every piece of public sentiment about it lives inside a platform it does not own, on a page it does not moderate. If Meta restricts this category further, and `category-and-market-research.md` names two DISAPPROVED ads already sitting in the account with no visible reason, the brand does not have a second surface to fall back to. Marked `inferred` from the footprint.

---

## Ad-comment responder coverage

**There is no responder. Not a thin one. None.** This is a `verified` finding and I tested for it directly rather than assuming.

The corpus holds **1,322 comments, of which 299 are replies**, on 112 ad IDs, over twenty months. I ran two semantic searches designed to surface a brand voice: one phrased as a standard support reply offering to check eligibility by direct message, and one phrased as a brand apology pointing to plans by state. The first returned **zero results** at a 0.45 similarity floor. The second, run at a loosened 0.35 floor to be sure, returned 25 results, and every single one is a customer complaint or a rival agent's pitch. Not one is the brand.

Comment volume is not trivial. The top ad alone drew 84 comments in the last 90 days against $42,741.16 of spend. The corpus has grown continuously since January 2025 and ten comments landed in the first three days of September 2026.

Here is what fills the silence, and this is the cost of it.

**Someone asks the brand's most important question and five strangers answer instead.** On 2026-03-20, under `MOMS38 - 1 - V1`, a commenter wrote *"Anyone actually have this and have insight?"* It drew **15 likes and 6 replies**, the highest-liked question in the entire corpus. The brand never replied. What she got instead, in order: a warning about spam calls from a past form, a stranger reading the brand's own website terms back at the thread and concluding the plans do not cover much, one positive note about a kind agent who could not help, and two people saying they did not qualify. Four of the five answers were negative or neutral.

**Rival agents work the room the brand paid for.** Verified live today. On 2026-05-20, under `Moms43 - 4 - V4`, a competing broker posted a full pitch that drew **6 likes and 5 replies**, which is more engagement than almost anything the brand's own audience produced: *"I have plans that start as low as $60 a month for those under 40 and $70 a month for those over. You arent constricted to a network, can use the policies internationally and get cash pay pricing still. Affordable insurance that actually works still exists in plenty avenues even for those with high income. You just have to work with brokers that care and are knowledgeable enough to show you the right products."* On 2026-07-16, under the account's top-spending live ad, a self-identified licensed advisor combined a warning and a pitch: *"As a licensed health insurance advisor, never put your info online unless you want 100 calls a day about health insurance... DM and I can help you look at the plans available in your state."* On 2026-04-11, under `MOMS38 - 1 - V1`: *"New innovated healthcare plans are available. If you are a business owner or self employed, As a Health Insurance Advisor, I can find a plan that covers cost of the deductible! Inbox me."* And on 2025-07-25, twice within thirty seconds under `B1 samar- Copy`, one operator left a phone number and a company name while agreeing with the criticism: *"my team can assist you if and when you need it. I think it's odd to market to moms but not offer anything dor maternity...682-307-0039 Health Insurance Confidant Consulting."*

The upstream count of 39 poaching comments across 10 ads is consistent with what I found and with the shape of it, though the exact classification is a semantic read rather than a string count. What today's pull adds is that the poaching is **still live**, it sits on the current top-spending ad, and one of these comments outperformed almost every organic comment in the corpus on engagement.

**The reputation read on this, marked `inferred`.** The absence of a responder for a brand with this comment volume would be a finding on its own. In this category it is worse than that. The binding constraint here is trust, not attention, and the comment section is the only public place where anyone asks whether this company is real. The brand is present in that room in every way except the one that matters. It pays for the room, it fills it with people, and then it says nothing while critics, correctors and competitors answer for it.

---

## Negative viral coefficient scan

**Present, verified, and it is the sharpest brand-risk finding in this document.**

The test is whether the brand's own customers are not merely complaining but actively telling other prospective customers not to buy. They are, in plain imperative language, and they have been doing it for twenty months. Every quote below is `verified` in the corpus with its date and ad.

- 2025-09-17, 6 likes, `B1 samar- Copy`: *"Absolutely do not give them your info. You will receive calls and texts nonstop from an insane amount of reps."*
- 2025-08-27, 5 likes: *"They don't cover preexisting conditions. Don't waste your time"*
- 2025-08-14, `B1 samar- Copy`: *"Don't bother looking into it if you're diabetic . I'll be uninsured until I die."*
- 2025-07-23, `B1 samar- Copy`, from a commenter identifying as a certified marketplace application counselor: *"I wouldn't waste my time on this page."*
- 2025-08-20, `B1 samar- Copy`: *"Health for Moms is not a health care company. They sell your info to other companies. Within 5 min of requesting info, I had received multiple texts, phone calls, and emails from a range of companies."*
- 2025-10-06, `B2 - 10TH JUNE - Copy 16`: *"They just sell your info. I did the form, and immediately got multiple calls and texts from different, unrelated insurance agents."*
- 2026-02-04, 4 likes: *"I got pushed around and given to a side insurance company. I had already done all of that and then some and tried this, so no I DO NOT RECOMMEND!"*
- 2025-07-29, **15 likes**, `B1 samar- Copy`: *"Markets to moms. Provides zero plans for moms. 🚩 Makes perfect sense."*

And the loudest one, at **33 likes on 2026-03-16 under `MOMS38 - 1 - V3`**, which is the third-most-liked comment in the whole corpus and the single most-liked comment about this brand's actual service:

> *"Filled it out and have been getting calls everyday from all sorts of companies which are mostly India based. Also, the harassment from whomever keeps calling me about Medicare (India again). This is the ONLY form I've filled out since getting my new phone number 3 months ago so it came from this site!"*

For scale, here is the top of the corpus by like count, read from a cut of 1,098 of the 1,322 comments sorted by likes on 2026-09-04: 47 likes for a deductible disclosure, 36 for a political read on the ACA, **33 for that warning**, then 24 and 21 for political one-liners. The most-liked thing anyone has ever said about this company's actual service is a warning not to give it your phone number. Marked `verified` within that cut, and the small share of the corpus the cut did not reach is unlikely to hold anything above 24 likes.

**The root cause, per the prompt's three candidates.** It is two of them at once, and they are not equally weighted.

**The primary root cause is a customer-service and handoff failure.** The strongest, most-liked, most action-shaped warnings all describe the same event: she filled the form and was called by many companies she did not choose. Two separate commenters say the page made an explicit promise about not being contacted by random agents that was then broken. On 2025-11-28: *"I filled this out because it literally says we won't be contacted by random agents. That's a lie. I immediately received 5 text messages from 5 different agents claiming to be from 5 different companies."* On 2026-01-28: *"It listed no selling my number to scammers but it's been just a few hours and I've had multiple numbers contact me with different agency type names."* This is the promise-breaking kind of damage rather than the honest-limit kind, and it happens downstream at the partner agencies where the brand has the least visibility and the least control. Marked `verified` on the pattern, `data-limited` on the cause, since whether the lead is sold to several buyers or one agency over-dials cannot be seen from outside. Worth carrying: the FCC's one-to-one consent rule that would have stopped exactly this was vacated on 2025-01-24 and formally repealed in September 2025, so no regulation is coming to fix it.

**The secondary root cause is a real product limit: the eligibility gate.** Pregnancy, pre-existing conditions, the state list and a possible income floor each turn away women the advertising invited. These produce dissuasion too, but a different flavor of it. They read as *"don't waste your time, it isn't for you,"* which costs the brand traffic. The call-flood reads as *"do not give them your information,"* which costs the brand trust. The second is the more expensive kind.

**Not shipping or fulfilment**, which does not apply to a lead-generation service.

**Weighing it against the negative bias.** These dissuasion comments are a minority of the corpus and they should not be inflated into the brand's whole reputation. What earns them weight is three things the mining method treats as significance rather than volume: they carry the highest like counts in the corpus, meaning many readers agreed without typing; they recur across many different ads over fourteen months rather than clustering in one place; and they are first-hand accounts of the brand's own funnel rather than opinions about health insurance. Confidence: **strong** that the pattern is real and durable. **Mixed** on how many leads it costs, which nothing here can measure.

One number from today's pull that belongs in this section and cannot be resolved. `Moms43 - 4 - V3` earned **326 shares** in the last 90 days against 84 comments. In a comment section this hostile, a share is not automatically an endorsement. It could be a mom sending the offer to her sister, or it could be a mom sending the ad to a friend with a comment about the pregnancy exclusion. Marked `data-limited` on valence, and it is one of the open loops below.

---

## Persona signals

These are signals, not personas, and none of them is a persona until the persona work validates it against buyer data that does not exist yet. Per the evidence ranking in the persona method, this brand holds only the weakest tier, community comment, and holds none of the stronger ones. Every demographic read below is `inferred` and must not harden into a claim.

**The audience knows this category better than the creative assumes.** 74 of 1,322 comments use the phrase "out of pocket," and self-identified brokers, agents and medical billers are among the correctors. Beyond the correction, commenters trade real technical vocabulary with each other unprompted: guaranteed issue, medical underwriting, coinsurance, subsidy, certified application counselor. That is a sophistication signal and it points at the register the creative should use. `Inferred`, confidence **mixed**, because the ad itself put the word "deductible" on screen and may have recruited the correctors.

**The person researching this brand verifies through peers and search, in that order, and finds nothing.** Three comments describe running a Google search and coming up empty. The corpus's highest-liked question is a request for a peer review. That is a buyer-journey signal about where trust is decided, and it is decided before the form rather than inside it. `Inferred`, confidence **mixed** on one thread and three search reports.

**The brand's advertising reaches well past the person it names.** Men, women whose children are grown, women with no children, and a 64-year-old all appear asking whether they qualify. Delivery ran 95.2% female and 81.2% aged 25 to 44 in the last 90 days, but delivery shows who Meta found, not who could buy. `Verified` on the delivery split, `inferred` and unresolved on what it means.

**The emotional state the creative lands in works against identification.** Reading the corpus through the emotional-delivery lens, the dominant landing state is high-intensity negative, which narrows attention and suppresses the reflective processing identification needs. Recognition in this corpus runs under 1%. Argument runs far higher. `Inferred`, and it is a messaging signal more than a persona one, carried here because it shapes who the creative can actually reach.

**Do not read a persona out of any of this.** It is one noisy, brand-controlled source with no buyer data behind it.

---

## Open loops

**1. The brand's own name may be the reason nobody can check it out.**

Search "Health For Moms" and you get a federal website launched in May 2026 called Moms.gov, a Missouri state program, a Wikipedia article about a 1996 maternity law, and a rival at `betterhealthformoms.com`. Search the brand plus "legit" and you get the FBI and the FTC warning about health insurance scams, and nothing about this company. Three of the brand's own commenters say they searched and found nothing, including one who concluded from that alone: *"sounds like a scam to me."*

Pull: **Surprise.** A brand can be small and still be findable. This one is unfindable in a specific way I did not expect, because its name is made of words that a decade of government and nonprofit health content already owns.

Question: What does this brand's name do to a mother who tries to look the company up before she gives it her phone number?

Why it matters: if the name itself is what makes the brand uncheckable, then no amount of creative testing touches the problem, and the answer is a searchable identity rather than a better hook. If the name is fine and the brand is simply young, then the work is publishing enough that a search finds something, which is a much smaller job.

Territory: **Messaging.**

**2. The ads claim thousands of moms approved this, and not one of them is visible anywhere.**

The headline on the account's top creative reads *"Approved by thousands of Mom's across America,"* and it runs on ads carrying $71,643.33 of the last 90 days' $98,276.81. Verified against every checkable surface today: zero reviews, zero press, no Better Business Bureau profile, and two pieces of praise in 1,322 public comments.

Pull: **Tension.** The brand asserts mass third-party approval and every independent surface is empty, and both of those cannot be the whole truth.

Question: Where could a customer actually see the approval the ads claim?

Why it matters: it decides whether this brand has an unused proof asset sitting in its partner agencies' call logs, or an unsupported claim running on nearly three quarters of live spend in a category where the FTC has warned twenty-one companies in this exact business about deceptive claims. Those two situations call for opposite actions.

Territory: **Messaging.** Only the brand can answer this one, since it needs whatever customer record sits behind the claim.

**3. People are sharing these ads more than they are commenting on them, and nobody knows why.**

In the last 90 days `Moms43 - 4 - V3` earned 326 shares against 84 comments, on $42,741.16 of spend. The comment section under that same creative contains the pregnancy objection, the correction thread, and a live rival-agent pitch.

Pull: **Curiosity.** A share is normally a good sign and a hostile comment section is normally a bad one, and here they are sitting on the same ad, which the rest of this brain cannot explain.

Question: Why are people sharing these ads?

Why it matters: if shares are mothers passing a real offer to a friend, that is the brand's only piece of organic advocacy and it is completely unmeasured. If shares are mothers passing along the joke about a company called Health For Moms that will not cover pregnancy, then the brand is paying to distribute its own worst objection.

Territory: **Messaging.**

**4. The brand has never spoken in the only public room where anyone asks whether it is real.**

Zero brand replies in 1,322 comments across twenty months and 112 ads, confirmed by two semantic searches today, one of which was deliberately loosened and still returned only customers and rival agents. Meanwhile the highest-liked question in the corpus, *"Anyone actually have this and have insight?"*, drew fifteen likes and six answers from strangers, four of them negative.

Pull: **Gap.** There is obvious, sustained, high-stakes activity here and nothing has ever been done about it.

Question: What is happening to the women who read those threads before they decide whether to fill out the form?

Why it matters: this brand's binding constraint is trust rather than attention, its hook rates are healthy, and the comment section is the last thing many people see before the click. If the unanswered threads are where leads are lost, then moderation is a performance lever and not housekeeping, and it is cheaper than any creative round.

Territory: **Messaging.**

---

## Appendix - Parker media links

All links and paths preserved exactly as returned by Parker MCP or by web search on 2026-09-04.

**Brand:** Health For Moms, brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`. **Ad account:** `HealthForMoms`, act `484897827497337`.

### Ads carrying the authority claim, 72.9% of 90-day spend

- `Moms43 - 4 - V3`, $42,741.16 in window, headline "Approved by thousands of Mom's across America", 326 shares, 84 comments
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4
- `Moms43 - 5 - V1`, $10,020.57 in window
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120243987355020519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0fe2980848d12fe1c6fd107a759e68fe37d8776c34235b5fab3c15e751af171d.mp4
  - Landing page: https://www.healthformoms.co/save/
- `Moms43 - 4 - V1`, $6,993.31 in window
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380110519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/f18c5a15a13e4412e35f654034f63f147ca73e40b35538419d22500d143b670d.mp4
- `Moms43 - 4 - V4`, $6,360.53 in window, carries the 2026-05-20 rival-agent pitch at 6 likes
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380050519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/985c6a8045a5bcfb5e7450ad0f3a00ca783b996f4ba3633337e8c84e1aac8a39.mp4
- `moms-63 2b`, $5,527.76 in window, $13.29 cost per lead
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
  - Landing page: https://www.healthformoms.co/save/

### Ads carrying the reputation evidence quoted in this doc

- `MOMS38 - 1 - V1`, the corpus's most-commented creative, carries the peer-verification thread and most of the correction thread
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120233032588900519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- `moms54-3`, highest attention in the 90-day window
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063711860519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/5a62b11062812d9509cb2cd8c95e89777a15d1a6ac1cdb1f6e9a92eb77f93a9d.mp4
- `IMG 6`, the 2025 static carrying the Reddit verdict comment
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120212962324800519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/14f1fb45d1b0308a5b25ce5cfdb6b2b7f9116c569643058dc4ba2d6965e51a55.jpg

### Comment corpus

Comments carry no permalink in the Parker response, so they are cited throughout by exact text, date, ad name and like count. Corpus of 1,322 comments spanning 2025-01-08 to 2026-09-03, brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`. Cuts run live 2026-09-04 with their totals:

- `pregnan` — 38 of 1,322, 2.9%, across 15 distinct ad names
- `out of pocket` — 74 of 1,322, 5.6%, across 12 distinct ad names
- `reddit` — 1 of 1,322, 0.08%
- Broad cut sorted by like count, top of corpus: 47, 36, 33, 24, 21, 19, 17, 15, 15, 14, 14

Comment ids for the load-bearing quotes:

- The Reddit verdict, 14 likes and 10 replies, 2025-01-13, `IMG 6` — `f55ae3d8-afcd-1903-3bcb-6e2de2bc0bbb`
- Daily calls after the form fill, 33 likes, 2026-03-16, `MOMS38 - 1 - V3` — `3e6adba4-f376-7605-39dc-2dba27b2a2a5`
- "Anyone actually have this and have insight?", 15 likes and 6 replies, 2026-03-20, `MOMS38 - 1 - V1` — `7d74447b-bc85-97f5-c3ec-39d711ff885b`
- "Markets to moms. Provides zero plans for moms. 🚩", 15 likes, 2025-07-29, `B1 samar- Copy` — `184aaf10-b07b-3145-feae-4376d3f497de`
- "How many calls will I get if I try to see how this works?", 17 likes, 2026-05-17 — `3707bfa1-c0bd-2629-63b4-6987e500f611`
- Pregnancy denial, 7 likes, 2026-04-01, `MOMS38 - 1 - V3` — `f9ace9e7-79d5-9a87-149c-15af9eea7fdd`
- "not eligible... currently pregnant", 5 likes, 2025-07-24, `B1 samar- Copy` — `2f6760b9-7a5f-2a0b-c58c-c5279f36831d`
- Licensed broker correcting the hook, 2026-04-07, `MOMS38 - 1 - V1` — `efb760eb-07c9-633d-d536-f92c0ac05bc4`
- "educate people, not misinform!!", 2 likes, 2026-03-29, `MOMS38 - 1 - V5` — `c0a3c689-ecb4-a5a8-ae30-3176267bcc34`
- Rival broker pitch, 6 likes and 5 replies, 2026-05-20, `Moms43 - 4 - V4` — `f33fe6c3-e576-5a4a-acc1-adc07c56ddc0`
- Rival advisor warning and pitch, 2026-07-16, `Moms43 - 4 - V3` — `53605ce2-d6ad-5ce9-9f93-29f4ef3694cc`
- "Inbox me" pitch, 2026-04-11, `MOMS38 - 1 - V1` — `8f1cf1b0-c63a-5eb1-8f74-15c8d3fefac6`
- Agent praise despite being told no, 2 likes, 2026-04-17, `Moms Nahuel WV#1 - V9` — `1869c324-0e1b-5b8d-935f-dac29e34854b`
- "why don't any of the plans offer prenatal care?", 2026-08-05, `Moms43 - 4 - V3` — `d104fd21-cf8d-5971-b643-2b1fcf440544`

### Public web sources read this run

The brand's own surfaces:

- https://healthformoms.co/
- https://healthformoms.co/home
- https://healthformoms.co/privacy-policy-acn-9365-1408-4908
- https://www.facebook.com/p/Health-For-Moms-61569029311372/
- https://www.facebook.com/61569029311372/posts/moms-were-the-heartbeat-of-our-families-protecting-their-health-isnt-just-a-jobi/122110526318634310/

What sits in the buyer's path when she searches the brand plus "legit" or "scam":

- https://www.fbi.gov/investigate/cyber/alerts/2025/emerging-discount-medical-insurance-scams
- https://www.ic3.gov/PSA/2025/PSA250430
- https://consumer.ftc.gov/articles/spot-health-insurance-scams
- https://consumer.ftc.gov/blog/2018/11/rest-insured-you-can-avoid-fake-healthcare-plans
- https://www.healthinsurance.org/obamacare/avoid-scams-while-shopping-for-insurance/
- https://www.tn.gov/attorneygeneral/working-for-tennessee/consumer/resources/materials/healthcare-scams.html
- https://www.consumeraffairs.com/news/fbi-warns-about-discount-medical-insurance-scams-050225.html

What outranks the brand on its own name:

- https://www.hhs.gov/press-room/trump-administration-launches-moms-gov-for-new-and-expecting-mothers.html
- https://www.deseret.com/politics/2026/05/13/white-house-launches-moms-dot-gov-over-rising-concerns-on-maternal-health/
- https://healthymomsbabies.mo.gov/moms-babies/healthcare/
- https://en.wikipedia.org/wiki/Newborns%27_and_Mothers%27_Health_Protection_Act
- https://en.wikipedia.org/wiki/Connect_for_Health_Colorado
- https://betterhealthformoms.com/

What ranks on the category search the buyer actually runs, where the brand does not appear:

- https://healthpluslife.com/health-insurance/stay-at-home-moms-your-best-health-insurance-options-without-employer-coverage/
- https://www.wealthysinglemommy.com/health-insurance-single-moms/
- https://myprivatehealthinsurance.com/private-health-insurance-for-stay-at-home-moms/
- https://www.nerdwallet.com/insurance/health/missouri-health-insurance

Verification surfaces checked and found empty for this brand:

- https://www.bbb.org/us/fl/orlando/category/health-insurance/accredited
- https://www.bbb.org/us/fl/orlando/category/sales-lead-generation
- https://www.bbb.org/us/tx/irving/profile/insurance-agency/yeti-insurance-agency-llc-0875-91138881 — a different company, not the operator of this brand
- https://www.trustpilot.com/review/healthinsurance.com — a different company

Sources attempted and blocked, carried forward from the 2026-09-03 tests and not retried today:

- https://www.reddit.com/r/HealthInsurance/
- https://old.reddit.com/r/HealthInsurance/
- https://www.healthformoms.co/save/
- https://quiz.healthformoms.com/#/indvfam
- https://www.facebook.com/business/help/298000447747885
- https://transparency.meta.com/policies/ad-standards/restricted-goods-services/health-wellness/
