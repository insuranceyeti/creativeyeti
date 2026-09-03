---
brand: health-for-moms
doc: brand-identity-analysis
generated_on: 2026-09-03
refresh_by: 2027-03-03
sources_read:
  - "Brand context document via Parker MCP `get_brand_persona`, all 14 sections, ~50KB, read in full"
  - "Health for Moms Brand Guidelines.pdf — read only as summarized inside the brand context document, sections 7 and 8. The PDF itself was not reachable."
  - "Parker chat history via `search_chat_history` — 4 threads, 1 web and 3 Slack, all dated 2026-09-03. Two Slack threads read in full."
  - "Meta ad account `HealthForMoms`, act 484897827497337, via `search_facebook_ads_sql` — top 8 ads by 90-day spend with full transcripts; top 10 statics by lifetime spend with headline and body copy; four keyword sweeps across the 2,122-ad library"
  - "`source-pulls/ad-account.md`, the Phase-1 persona source pull, read in full — 13 ads read at full media depth with transcript, AI creative analysis, creator demographic and delivery split"
  - "`running-notes/missing-context.md`, `running-notes/brand-rules.md`, `running-notes/success-definition.md`, `BUILD-STATUS.md`"
  - "Attempted and blocked: healthformoms.com and healthformoms.co/save/"
data_limitations:
  - "The brand's own website could not be reached from this environment. WebFetch returned EGRESS_BLOCKED for both healthformoms.com and healthformoms.co, and a direct curl returned a 403 on the proxy tunnel for both. That means the home page, the about or our-story page, the product and collection pages, the mission page, the FAQ and any press section were never read first-hand. Every website-derived fact in this doc reaches me secondhand through the brand context document, which states it was compiled partly from 'brand website analysis.' All of it is marked stated, and none of it is marked verified."
  - "The site's visual register, its aesthetic and the kind of customer it visually speaks to could not be observed at all. The Website identity section below is largely a named blank for that reason."
  - "The Health for Moms Brand Guidelines PDF was not readable. The brand context document summarizes it and the team confirmed in Slack on 2026-09-03 that they uploaded it to Parker training. What I have is the summary, not the source, so every guideline quoted here is quoted at one remove."
  - "Customer reviews and post-purchase surveys are confirmed empty for this brand, and no competitors are tracked in the Parker app. Nothing in this doc is checked against what a real buyer or a rival says. That is correct for a brand-on-brand doc but it means every identity claim here stays a starting hypothesis."
  - "No `get_current_time` tool was available in this run. The date is taken from the session context, 2026-09-03, and cross-checked against the Phase 0 docs, which carry the same date."
  - "Parker's `keywords` filter matches across fields the response does not always return, including transcripts and AI analysis. Where a keyword sweep matched an ad but the matching text was not visible in any returned copy field, I say so rather than guessing where it sat."
---

# Brand identity analysis — Health For Moms

## How this read was built

This doc has one job: capture what Health For Moms thinks it is, in the brand's own terms, so a later step can reason about it without going back to the source. It is a presentation, not a verdict.

The plan was to start at the brand's website, because that is where a brand's self-conception is usually most complete. That failed. Both healthformoms.com and healthformoms.co are blocked by this environment's network proxy, confirmed twice, once through WebFetch and once through curl. So the spine of this doc became the brand context document that Parker holds, a roughly 50KB, 14-section record compiled from brand-provided training data, the brand's own website, the Health for Moms Brand Guidelines PDF and public research. That document carries the brand's positioning, its voice rules, its compliance rules, its ICPs, its testing history and its stated targets, much of it quoted verbatim from what the brand handed over.

Then I did three things the brand context document alone could not do.

First, I read the team's four Parker conversations, all from 2026-09-03. Three are Slack, one is web. Most of it is tooling talk about setting up this brain. But one thread carries a real correction to the brand's stated audience, and it changes how the Claimed personas section below has to be written.

Second, I went into the live Meta account, not to grade performance, which belongs to the ad-account read, but to see what the brand's own voice and its own claims actually look like when they are running. I pulled the top eight ads by 90-day spend with full transcripts, the top ten statics by lifetime spend with headlines and body copy, and I ran four keyword sweeps across the 2,122-ad library against the brand's own banned-word list. Under this prompt's rule, a claim about creative has to come from full media, not from an ad name, so every ad quoted below is quoted from its transcript, its headline or its body copy.

Third, I read the Phase-1 ad-account source pull, which had already read thirteen ads at full media depth with transcript, AI creative analysis, creator demographic and delivery split. That is a prior source doc that inspected the materials, so its creative reads carry here.

Two things shifted the read along the way. One is that the brand's stated audience has a live, hand-typed override sitting in Slack that contradicts the audience criteria written in its guidelines, and the brand's own canonical ICP list contains at least one profile that Parker wrote and the brand then adopted. The other is that the brand's single most non-negotiable claim rule, the one it marks in capital letters, is broken by copy carrying roughly two thirds of its lifetime static spend. Both are recorded plainly below and neither is resolved here, because this doc records rather than judges.

---

## What the brand is, who they are, what they sell

Health For Moms is a health insurance matching service built for mothers. It does not sell insurance. It collects a mom's details, checks whether she qualifies in her state, and hands her to a pre-vetted partner insurance agency whose licensed agent sells her a plan. `stated`, brand context document, section 1.

The brand's own plainest description of itself: "Health For Moms is dedicated to empowering mothers with better, more affordable health insurance options." `stated`, brand context document, section 1, quoted as given.

**The category and the model.** Health insurance lead generation, aimed at one demographic. The brand context document is explicit that "It is not an insurance carrier — it is a connector." There is no pricing page and no checkout, because the consumer never pays Health For Moms anything. `stated`, section 1. The account data agrees with the model: 4,336 leads and zero purchase events in the 90 days to 2026-09-02. `verified`, Parker MCP `search_facebook_ads_sql`, pulled 2026-09-03.

**The product it steers people toward.** Private health plans, deliberately not government marketplace plans. The emphasis is on premium savings and low or no deductible options. `stated`, section 1.

**The named mechanism.** The **MomSmart Coverage Method™**, described by the brand as "new tech that scans plans and matches each family with the right private health plan based on their needs, doctors, and budget. Using nationwide plan access, transparent pricing, and personal advisors, the MomSmart Coverage Method™ helps moms save up to 30% while gaining $0 deductible protection and freedom of choice." `stated`, brand guidelines as summarized in section 7, quoted verbatim.

**The three-step promise.** As the brand frames its own process:

1. **Connect** — "Answer a few simple questions so they can connect you with the right insurance provider."
2. **Speak with an agent** — partner agents are "like your Mom BFFs - friendly and approachable," so moms can ask questions "without feeling pressure."
3. **Get a better plan** — the agent reviews the current plan "to ensure the customer isn't overpaying for things they don't need or isn't covered where they thought they were."

`stated`, brand context document, section 1, website-derived and quoted as given there.

**The stated benefit set**, as the brand lists it in its guidelines:

- Nationwide coverage, see any doctor, anywhere in the U.S.
- $0 deductible options, "never worry about huge out-of-pocket bills"
- Up to 30% savings on premiums compared to traditional plans
- Freedom to choose your doctor or pediatrician, or keep your own when you switch
- "Real coverage that actually pays when it matters"
- "Fast, personal support from licensed advisors who speak human, not 'insurance'"

`stated`, section 1.

**The primary tagline.** "Better family health coverage for less." `stated`, section 7.

**How it positions against the alternatives a buyer already knows.** The brand casts the whole insurance system as the villain and itself as the challenger exposing it. Its own framing, quoted in section 1: "every 3 minutes a family in the United States goes bankrupt from medical bills when they HAD insurance," and "most think they're covered when they aren't." The brand context document describes this as challenger positioning that stays "warm and solution-oriented rather than fear-driven." `stated`.

The alternatives the brand sees itself sitting against, in its own words, are three layers deep: the government marketplace, which it will not name in creative and positions away from by choice; employer-provided insurance, which the document calls "the most common 'competitor' — the default option families already have"; and the big carriers, positioned as "faceless corporate entities with CEO salaries inflating costs." Generic lead-gen marketplaces like EverQuote and QuoteWizard are named in the document as direct competitive alternatives, but the brand itself supplied no competitor list. Section 6 says plainly: "The brand did not provide any specific competitors or competitor websites." `stated`.

**How clear is this self-positioning?** My observation, not the brand's: unusually clear for a brand at this stage. The positioning line, the mechanism, the benefit set, the villain and the tagline are all written down and they all agree with each other. Most young brands cannot produce that. The fuzziness is not in what the brand thinks it is. It is in what backs the claims, and in who the brand thinks it is for. Both of those are handled in their own sections below.

**Where it is based and how it reaches people.** Orlando, Florida. Digital-first, with acquisition driven by paid social into a state-by-state qualification funnel on the website. `stated`, section 1.

---

## Founder and origin story

**There is no founder story, and the brand says that on purpose.**

Section 13 of the brand context document is headed "Founder Story" and its entire content is this: "Is the founder story strategically important? **No.** The brand indicated the founder story is not important to the creative strategy. No founder narrative was provided." `stated`.

So this is a named blank the brand itself created rather than a gap in the research. Nothing in the brand context document, the four Parker conversations or the ad library names a founder, a founding date, or an origin moment. My observation: the founder is not a visible or recurring presence in the brand's content in anything I could reach. Across 13 ads read at full media depth in `source-pulls/ad-account.md` and 8 more read at transcript level here, every on-camera person is a mom, a spokesperson or a creator. None is presented as the founder. `inferred`, from the creative read, and it rests on 21 ads out of a 2,122-ad library, so it is thin as proof of absence.

**The channel story, which is the part only the brand can tell.** Health For Moms started and stayed direct-to-consumer online. It was never discovered on a shelf and there is no retail chapter. The brand context document describes the distribution model as "entirely online: paid social ads drive moms to the website's qualification funnel," and calls the brand "a digital-first platform with advertising-driven customer acquisition." `stated`, section 1.

The account backs the shape of that. The Meta library holds 2,122 ads and $743,218.09 of lifetime spend across video and statics, running as far back as December 2024. `verified`, from the Phase-1 ad-account pull and my own lifetime cuts on 2026-09-03. That is a brand whose whole existence has run through paid social.

**What to confirm with the brand.** When Health For Moms launched, who started it and why, and whether the founder's absence from the brand is a deliberate choice or simply a thing nobody has written down yet. The brand said the story is not strategically important, which answers whether to use it, not whether it exists.

---

## Claimed personas

This is the section where the brand's self-conception is least settled, and it is worth reading slowly because three different versions of the audience exist and they do not fully agree.

Under the persona method in `persona-research-and-creative-strategy-process.md`, everything here is the **stated** persona set, not the actual-buyer read. The actual-buyer read is impossible for this brand right now anyway: customer reviews are empty, post-purchase surveys are empty, and there is no purchase event in the account. On that doc's evidence ranking, which puts post-purchase survey data at the top and competitor signal at the bottom, this brand currently has none of the top three tiers. So every persona below is a hypothesis the brand holds, and I am not building personas here. Real personas get built elsewhere from buyer data.

### Version one — the five canonical ICPs

The brand context document carries five named ICPs, inserted verbatim from what the document calls "the canonical ICP document." `stated`, section 2.

- **Jen — The Family Safety Net.** "She's the one who reads the EOB statements, books all the appointments, and worries about what happens if something goes wrong. She wants to know her family is actually protected, not just technically enrolled. Responds strongly to the 'real coverage that actually pays when it matters' message." No age, no location, no family detail given. Four sentences long, against several paragraphs each for the other four.
- **Danielle — The Quietly Overwhelmed Planner.** 38, suburb outside Charlotte, husband Matt, two kids aged 5 and 8, project manager at a logistics company. Her trigger, in the document's words: "Matt's company just got acquired, and the benefits package is 'under review,' which she knows means it's about to get worse." Her stated behavior: "She'll research for two hours, get overwhelmed, and then circle back to it three weeks later when the anxiety spikes again."
- **Marissa — The One Holding It Together Alone.** 33, San Antonio, dental hygienist, son Eli aged 4, split from Eli's dad two years ago. She sits in the coverage gap: "she makes just enough to fall into that infuriating gap where she doesn't qualify for much help but can't comfortably afford what's available." Her trigger, per the document: "the fear that one ER trip could set her back months."
- **Courtney — The Accidental Entrepreneur.** 36, outside Denver, runs a Shopify pet-portrait business, husband James works IT at a hospital. She is not on his plan because "adding a spouse to James's employer plan costs an additional $480 a month," and she is on a short-term plan she is "about 60% sure it actually covers anything meaningful."
- **Nicole — The Second-Chapter Mom.** 41, suburbs of Atlanta, school counselor, first baby seven months ago, husband Andre drives for UPS. Her trigger is the coverage transition after childbirth: "She's gotten three different answers from HR about when her coverage resets."

Read against the persona method's own test, four of these five are trigger-anchored identities, which is the shape a real persona is supposed to have. The activating moment is named in each: a benefits package under review, a divorce, self-employment, a birth. Jen is the exception. She is described by a behavior, reading EOB statements and worrying, with no trigger and no situation attached. That matters, and the next section explains why.

### Version two — the guidelines criteria, and the correction that produced them

On 2026-09-03 at 21:05 UTC, in the Slack thread `1788469337.157819`, a member of the team told Parker that an earlier set of five ICPs was "very wrong," then uploaded the brand guidelines. `stated`, verbatim from the team.

Parker read the guidelines and reported back the audience criteria it found in them. Those criteria, as Parker stated them in that thread:

- Age **28-50**
- **Married or partnered**
- **1-3 kids**, babies to teens
- Suburban or small-city
- Household income **$50K-$150K+**
- "She is the primary decision-maker for family finances AND healthcare"
- The rule that knocked out one of the old profiles: "no pregnancy-only targeting either"

`stated`, sourced to that Slack thread, 2026-09-03. I could not read the guidelines PDF myself, so these criteria reach me at one remove. They are the brand's criteria as reported by Parker from the brand's own document, and they should be confirmed against the PDF before anything is built on the exact numbers.

Parker then proposed three buckets built from those criteria: **The Capable Manager**, a married mom aged 30-42 with two kids on an expensive or thin employer plan; **The Protective Planner**, aged 35-48 with kids from toddler to teen, who reads the EOB statements; and **The Value-Seeker**, aged 28-40 with one or two kids under five, who the savings number genuinely excites.

The team's reply, verbatim: "That sounds about right genrally those 3. I'm sure we can go granular as we go correct?"

So the three buckets are Parker's synthesis, endorsed by the brand. They are not independent brand knowledge. That distinction matters and it is the finding in the next block.

### The provenance finding — one canonical ICP is a Parker read the brand adopted

The description of **Jen** in the brand's canonical ICP document is word for word the description Parker wrote for **Bucket 2, The Protective Planner**, in that Slack thread on 2026-09-03.

Parker's Slack text: "She's the one who reads the EOB statements, books all the appointments, and worries about what happens if something goes wrong. She wants to know her family is actually protected, not just technically enrolled. Responds strongly to the 'real coverage that actually pays when it matters' message."

The brand context document's Jen entry: identical, character for character, with only Parker's opening demographic line "Married mom, 35-48, kids ranging from toddler to teen" removed.

`verified`, by direct comparison of the Slack thread text against section 2 of the brand context document, both pulled 2026-09-03.

This is why Jen has no trigger and no situation while the other four do. She was never a persona. She was a bucket label Parker generated from the brand's own guidelines, which the brand then adopted into its canonical list. The other four read like they came from somewhere else, because they carry the concrete texture that a generated bucket does not.

I am recording this rather than resolving it. What it means is that when a later step reads "the brand claims five personas," at least one of those claims is the brand agreeing with a machine read of its own guidelines, not the brand telling you something it independently knows. That changes how much weight the set can carry.

### Version three — the live override the team typed themselves

Immediately after endorsing the three buckets, the same team member added a constraint that contradicts the "married or partnered" criterion. Verbatim, Slack, 2026-09-03:

> "BEcause honestly single moms are fine just as long as we also use lingo about them not being broke if that makes sense"

`stated`, and it is the most recent thing the brand said about its own audience. Under this prompt's rule that the brand's own hand-corrected word wins, this override stands over the "married or partnered" line from the guidelines.

Read carefully, it is not a demographic widening. It is a **tone** constraint attached to a demographic. Single moms are in scope as long as the copy does not read as financially desperate. Parker's summary back in the thread, which the team did not dispute: single mom copy should carry "'I've got it handled, I just want a better deal' energy rather than anything that reads as financially desperate."

That reconciles the canonical set with the criteria. Marissa the single mother and Courtney the self-employed one sit outside "married or partnered" but inside the override, and the brand context document is careful to write both as careful rather than broke. Marissa "has a $900 emergency fund that she rebuilt twice after car repairs," and "She's not broke—she's careful."

### How wide the brand thinks its audience is

Wide in stated intent, narrow in stated criteria. Section 10 of the brand context document names the new audiences the brand wants to test, verbatim: "All different ages of moms with ages of kids." That is nearly the whole category of mothers. Against that sit the guidelines criteria, which fence the audience to a partnered, suburban, mid-to-upper-middle-income mom aged 28 to 50 with one to three children.

Two more stated fences, both from section 8, both framed by the brand as internal guardrails rather than legal limits:

- **"No pregnancy-only targeting — focus on moms with kids (not expectant mothers exclusively)."** Nicole at seven months postpartum sits inside this rule, not against it.
- **"No punching down at demographic groups."**

**What this doc does not do.** It does not add a demographic, a psychographic or a life detail the brand did not state, and it does not rank these personas. Under the persona method, several of the situational states in this brand's world are **behavioral or identity overlays** rather than personas: being in a coverage transition, being self-employed, being in an open-enrollment window, being deal-motivated. Any of the five ICPs could be in any of them. Sorting persona from overlay is the persona doc's job and it needs buyer data this brand does not yet have.

---

## Tone and voice

The brand has a written voice, states it in one line, and the line is a good one.

**The guiding principle, verbatim:** the brand "speaks mom-to-mom, not insurance-to-customer." `stated`, brand guidelines as summarized in section 7.

**The voice as the brand describes it**, quoted as given:

- "Warm, relatable, conversational — feels like talking to a trusted mom friend"
- "Balances empathy and empowerment: 'We get what you're going through — and we've got you'"
- "Light humor about mom life chaos is welcome"
- "Avoids corporate jargon and scare tactics"
- "Real, encouraging, slightly witty, and emotionally intelligent"

**More of this**, verbatim: "Warm, relatable, mom-to-mom, empowering, witty, real, reassuring, conversational, emotionally intelligent, sharing a secret."

**Less of this**, verbatim: "Corporate, clinical, jargon-heavy, salesy, condescending, sterile, insurance-speak."

**What it associates itself with**, verbatim: "Trusted mom friends, family dinner table, school pickup line, pediatrician visits, protecting your kids, financial peace of mind, everyday suburban life."

**What it refuses to associate with**, verbatim: "Call centers, fine print, government bureaucracy, corporate insurers, political debates, sales pressure."

**The taglines the brand offers itself.** The primary is "Better family health coverage for less." The alternates, all verbatim from the guidelines: "Health insurance that actually works for moms." / "Real coverage for real families." / "Finally, peace of mind for the one who holds it all together." / "Because moms shouldn't have to worry about coverage."

**The emotional promise, verbatim:** "Health for Moms gives mothers peace of mind knowing their family is protected and their finances are secure. It's not about policies — it's about protection, simplicity, and relief."

**The positioning statement, verbatim:** "Health for Moms helps busy mothers find affordable, reliable, and easy-to-understand health coverage that actually works — with the freedom to choose their doctor, save money, and protect their family without stress or surprises."

### The voice as it actually sounds when it runs

The section above is the brand labelling its voice. Here is the voice shown rather than labelled, quoted from live ad transcripts and body copy pulled from Parker MCP on 2026-09-03. All `verified` against the ad's own transcript or copy field.

The spoken register in the account's biggest ads is blunt, second-person and plain, and it does sound like a person rather than an insurer:

> "Listen, this is why you can't simply just say, 'Oh, I have insurance, I'm covered.' No. You need health insurance that has a zero dollar deductible without spending thousands."
> — `Moms43 - 4 - V3`, transcript at 0:18-0:23. This is the account's top-spending ad, $42,741.16 in the 90 days to 2026-09-02.

> "Can we stop acting like all health insurance is the same? Because having a plan and having a plan that actually helps you are two very different things."
> — `moms-63 2b`, transcript at 0:16-0:18.

> "I almost scrolled past this because I thought, 'I already have health insurance, this doesn't apply to me.' ... Worst case, you check and stick with what you have. Best case, you realize you've been paying way more than you needed to."
> — `moms-63 3e`, transcript at 0:11 and 0:40-0:43.

> "I'm so thankful for the mom that told me about this."
> — `moms-53 3`, transcript at 0:00. This is the clearest "mom-to-mom" line in the account and it is the exact register the guidelines describe.

The written register in the account's long-running body copy is warmer, more lyrical and much less plain:

> "Moms, we're not just caregivers—we're protectors of futures. We know the power of a gentle hand on a feverish forehead or a hug that says, 'It's going to be okay.' ... Let's make one that counts. Click below to explore plans built for the women who hold it all together."
> — shared body copy across the account's highest-spending statics and several videos, including `B1 samar- Copy` at $35,219.98 lifetime.

One line closes several of the winners and it is worth flagging because it hits three of the brand's own approved words at once:

> "Finally, insurance that actually feels like it has our back."

"Finally," "actually" and the plain-speech register are all on the brand's own "words we use" list. `verified`, transcript of `Moms43 - 4 - V3` at 0:46 and `MOMS34 - N1 - 3a` at 0:27.

**My observation, held lightly and marked as mine.** The spoken voice and the written body copy are two different voices. The spoken lines are short, direct and unpolished, which is what the guidelines ask for. The body copy is longer, more ornamental and closer to greeting-card writing than to a mom talking. The brand states one voice. Its running work carries two registers. I am recording that, not judging which is right.

---

## Credibility markers

Everything the brand offers as validation, sorted by what kind of marker it is.

**Volume claims about people served.** Three different numbers exist and they do not agree.

| Claim | Where it appears | Standing |
|---|---|---|
| "over 5,000 moms nationwide" | website, per brand context document section 1 | `stated`, no backing found |
| "Approved by thousands of Mom's across America" | used as the `ad_title` on many live ads including `B2 - 10TH JUNE - Copy 16` at $15,660.83 lifetime | `verified` that it runs; the claim itself has no backing found |
| "250,000 families this year" | reported in section 6 as appearing "in some scripts" | `data-limited`, see below |

I ran a keyword sweep of the full ad library for "250,000 families." Four ads matched, holding $236.18 of lifetime spend between them, and the phrase did not appear in any copy field those ads returned, so I could not confirm where it sits or whether the match was exact. The brand context document already names this gap itself, in section 6: "Any gap between on-site and in-ad claims could undermine credibility."

**The trademark.** The MomSmart Coverage Method™ carries a trademark symbol wherever the brand writes it. `stated`. I could not check any trademark register from this environment. Flag to the brand.

**Trust language about the partner network.** The brand describes its partner agencies as "pre-vetted," "honest and trustworthy," and staffed by "licensed advisors" and "licensed agents." `stated`, sections 1 and 7. No agency is named anywhere in anything I could reach.

**Third-party recognition.** None found. No awards, no press hits, no as-seen-in section, no certifications, no named partnerships or collaborations, and no reviews. Confirmed empty rather than unreached for reviews, which returned zero rows in the Phase 0 surface test.

**Craft references the brand cites.** The guidelines name a standing set of reference frameworks: Great Leads by Masterson, Ca$hvertising, Scientific Advertising by Hopkins, Ogilvy on Advertising, a Hook and Hold guide, Schwartz awareness levels, and Kahneman and Tversky's loss aversion. `stated`, section 7. These are not credibility markers for buyers. They are the brand telling a creative team what canon its work is judged against, and they belong to the rulebook section below. I list them here only so the full set is visible.

**The plain fact about this marker set**, which is a fact about the markers and not a judgment about strategy: every single credibility marker Health For Moms carries is **owned and self-asserted**. Not one is borrowed from a named partner and not one is third-party recognition. The brand context document flags the consequence itself, in section 14: "Search data suggests consumers are checking whether the brand is legitimate," and it reports people searching "is Health for Moms insurance legit."

---

## Website identity

**Mostly a named blank. I could not reach the site.**

Both healthformoms.com and healthformoms.co are blocked by this environment's network proxy. WebFetch returned EGRESS_BLOCKED for both and a direct curl returned a 403 on the proxy tunnel for both. So I never saw the home page, the about page, the product pages, the FAQ or any press section.

That means the things this section is supposed to own could not be observed at all:

- The site's visual register and aesthetic — **not available**
- The kind of customer it visually speaks to — **not available**
- Whether the visual identity and the stated identity point in the same direction — **not available**
- Photography style, colour, type, layout — **not available**

**What I can carry, all of it secondhand or from the account.**

The brand runs two live destinations, both named in the ad library's `landing_url` field: `https://www.healthformoms.co/save/`, which carries every one of the top ten statics by lifetime spend, and `quiz.healthformoms.com/#/indvfam`, named in the Phase-1 ad-account pull. `verified`, from the account.

The funnel shape, as the brand describes it: paid social drives moms to a qualification funnel where "they answer questions about their state and family situation, then are matched with a licensed advisor who contacts them." `stated`, section 1. The brand frames the low friction of that funnel as a product benefit in itself, and its own line for it is "easier than convincing your little one to wear matching socks — and with way fewer negotiations." `stated`, section 3.

The post-conversion line the brand uses on-site, verbatim: "Now you can cross this off your never ending to-do list!" `stated`, section 4. And the end-state line: "Rest easier at night knowing you're covered."

**What to do about this blank.** Someone with unblocked network access should read the home page, the about page and the FAQ, and describe the site's register and aesthetic. That is a small job and it closes the largest hole in this doc.

---

## Brand guidelines

The brand hands over a written rulebook and it is unusually detailed for a brand this young. But it is lopsided. The verbal rules are thick and specific. The visual rules, as far as I can see them, do not exist.

Everything below is quoted from the Health for Moms Brand Guidelines PDF as summarized inside the brand context document. I could not read the PDF itself, so all of it is `stated` at one remove.

### The visual rulebook — a named blank

**No visual guidelines were found.** Nothing in the brand context document's summary of the guidelines names a rule about the logo, colour, type, imagery or layout. No usage rules, no do-not rules, no palette, no typeface, no photography direction.

I want to be careful about what this means. It may be that the PDF contains visual rules and the summary dropped them, or it may be that the PDF genuinely has none. I cannot tell from here. Either way, a creative team working from what Parker currently holds has **no visual rulebook to check against**, and that is the fact a later step needs.

### The verbal rulebook — thick and specific

**Vocabulary, framed as firm rules.**

- **Words the brand uses:** Real, protect, relief, freedom, peace of mind, actually, finally, guide, family, match, find.
- **Words the brand does not use:** cheap, discount, policy, ACA, exclusions, guaranteed.

That second list is repeated in section 8 under the compliance heading as "Words never used in creative," which is how the brand signals it is a hard rule rather than a preference.

One small thing worth recording, and it is my observation. The brand's own emotional promise contains a banned word: "It's not about **policies** — it's about protection, simplicity, and relief." The word is used to reject the concept, which is probably the intent, but the rule as written does not carve that out.

**Tone rules, framed by the brand as preferences.** Section 7 lists what the brand "would never say" and then labels the list explicitly: "Per brand voice (stylistic preferences, not compliance rules)." The list: anything that sounds like a corporate insurance company; anything condescending or that talks down to the audience; clinical or sterile language; high-pressure sales tactics; anything that sounds like a call center script.

That labelling is useful and I am carrying it exactly as the brand framed it. The brand draws its own line between a preference and a rule, and it puts tone on the preference side and claims on the rule side.

**Creative architecture principles, framed as rules.** Verbatim from section 7:

- **Hook-to-body contract:** "the hook's promise must be paid off by the body. Mismatched hook/body is a top failure mode."
- **Direct response:** "Scripts tend to do better with direct response principles."
- **Audience-awareness calibration:** "don't over-explain concepts the audience already understands (e.g., what a deductible is) — assume problem-awareness and reframe the cause instead."
- **Pool-pricing mechanic:** "this is the causal explanation for why deductibles are high. The education beat should explain *why*, not define terms — this sets up the private-plan pivot logically."
- **Specificity reads as credibility:** "odd, specific numbers (e.g., $587) are more believable than round ones ($600)."
- **Open loops must withhold resolution:** "hooks that deliver their own payoff collapse viewer motivation to keep watching. Prioritize mystery, tension, incomplete story, transformation, and countdown loops over closed-loop hooks."

Read against the craft canon, this is a brand that has genuinely absorbed Schwartz. The awareness-calibration rule is a direct application of the awareness levels, aimed squarely at the problem-aware and solution-aware bands, and the pool-pricing rule is a market-sophistication move: it refuses to define the term and instead explains the cause, which is what a category does once the simple claim has been made too many times.

**The CTA architecture, framed as the three sanctioned ways to ask for the click.** Verbatim structure from section 7:

1. **The Mechanism CTA** — names the MomSmart Coverage Method™, transfers the burden, justifies the click. Framings: Tech/Scan, Human Expert, Insider/Access, Simple. The brand states it is "Best for warm/solution-aware audiences (Schwartz Level 3–4) and retargeting."
2. **The "Moms is the solution" CTA** — positions the brand as the answer and stacks benefits fast. Framings: Straight Reveal, Straight Reveal with Agent, FOMO, Discovery, Anti-Insurance. The brand calls this "The workhorse/default CTA."
3. **The State Angle CTA** — geographic exclusivity creating an open loop the viewer must close. Framings: Select States Classic, which the guidelines mark as one that "converts WELL!", plus New Plan Rollouts, New Website, The Unfair Advantage, The Reverse Gate. The brand states it is "Best for cold audiences and pattern-interrupt hooks."

Named against the hook taxonomy, the State Angle is a **demographic hook** stacked with a geographic qualifier, and it works the way that format is supposed to work: self-selection, tribal identity and a relevance filter, all in one line. "If you're a mom and you live in one of these states" calls out the identity and then gates it. The information gap sits in the gate itself, because the viewer has to keep watching to find her state on the list.

**The UGC production standard, framed as a rule.** Verbatim: "Scripts must be speakable — natural speech patterns over polished copy. Read aloud before finalizing and add some human words, stutters, etc. or sentences that aren't perfect grammar."

**Distinctive elements the brand names as its own.** The mom-to-mom register, "copy that reads like a friend sharing a secret, not a company advertising a product." Light humour grounded in real mom life, and the brand's own examples are matching socks, never-ending to-do lists and negotiating with toddlers. System-villain framing where "the broken insurance system is always the antagonist, never a specific company or person." Geographic specificity as a creative device. And the MomSmart Coverage Method™ as a named proprietary mechanism. `stated`, section 7.

---

## Claim substantiation

Every claim the brand makes about itself or its product, with what the brand offers as backing, and each one's standing. I am recording here, not deciding what is legally permissible.

The headline finding first, because it is the one a later reader most needs: **almost nothing here is substantiated.** The brand makes many specific, checkable, numerical claims and I found no study, no test result, no certification, no methodology and no primary record behind any of them in anything I could reach. Every claim below except the ones marked otherwise is **stated-but-unsubstantiated**, meaning the brand asserts it and provides no backing I can find. That is recorded as the brand's assertion and never as a proven fact.

### The core product claims

| Claim, in the brand's exact words | Backing the brand offers | Standing |
|---|---|---|
| "Save up to 30% on premiums with $0 / low deductible options." | None found. No comparison basis, no methodology, no sample. | stated-but-unsubstantiated |
| "$0 deductible options" / "options with no deductibles" | None found. The brand's rule requires the word "option," and its own live scripts hold that framing. | stated-but-unsubstantiated |
| "Nationwide coverage — see any doctor, anywhere in the U.S." | None found. | stated-but-unsubstantiated |
| "Freedom to choose your doctor or pediatrician" | None found. | stated-but-unsubstantiated |
| "Real coverage that actually pays when it matters" | None found. This is a felt claim, not a measurable one. | stated-but-unsubstantiated |
| The MomSmart Coverage Method™ is "new tech that scans plans" | A description of what it does. No demonstration, no technical account, no registration record I could check. | stated-but-unsubstantiated |

**A tension inside the claim set worth recording rather than resolving.** The brand's stated benefit is nationwide coverage, "see any doctor, anywhere in the U.S." The mechanism that closes nearly every ad in the account says the opposite about availability. From `Moms43 - 4 - V3`, transcript at 0:28, `verified`: "you can only get that if you are a mom and you live in one of these states." From `moms-63 2b`, at 0:34: "Just remember that you have to live in one of those states, otherwise it's not gonna work." The Phase-1 ad-account pull, which read 13 ads at full media depth, found the on-screen Approved State List running to 32 to 34 states in every one of them. So "nationwide" describes the plan network and the state list describes where the offer is available. Both can be true at once. But the brand's own materials never say which is which, and a mom reading the benefit list and then hitting the state gate has to reconcile that herself.

### The statistics the brand quotes

Four statistics run through the brand's positioning and none carries a citation in anything I could reach.

- "every 3 minutes a family in the United States goes bankrupt from medical bills when they HAD insurance" — **stated-but-unsubstantiated**. This one matters most, because it is the lead line of the brand's challenger positioning and because the brand's own compliance rule bars "fabricated statistics."
- "Women in the United States make approximately 80% of the health care decisions for their families" — **stated-but-unsubstantiated**.
- "Since 2008, the general annual deductible for workers has increased eight times as fast as wages" — **stated-but-unsubstantiated**.
- "nearly half of all women in one study lost health coverage for at least 1 month in the first 6 months after giving birth" — **stated-but-unsubstantiated**. The brand's own phrasing names "one study" without naming the study.

### The claims the brand says are off-limits, and where the running work departs

The brand marks one claim rule as absolutely firm and its own creative does not hold it. This belongs in this doc because it is a rulebook-versus-substantiation fact, not a performance read.

**The rule, verbatim from section 8, in a section the brand heads "THIS SECTION IS NON-NEGOTIABLE":**

> "Savings claims: always 'up to 30%' — never drop the 'up to'"

**What actually ran.** Of the ten highest-spending statics in the account by lifetime spend, **nine carry a flat savings claim with no "up to" in the body copy**. Those nine hold **$116,622.92** of lifetime spend, which is **69.0% of the $168,907.73 the account has ever spent on statics**. `verified`, Parker MCP `search_facebook_ads_sql`, `adType: static`, `metricsMode: lifetime_only`, pulled 2026-09-03; the tenth returned no body copy so I excluded it rather than assume.

The exact wording, quoted from the ads' own `ad_content` fields:

> "comprehensive health plans that cover traditional care, embrace holistic wellness, and put your family's needs first—all while **saving you 20% or more**."

> "And with **savings of 20% or more**, you only pay for what you use—so you can focus on the things that really matter."

Two more instances, both flat and both more specific:

- Headline, verbatim: **"Left my big insurance company for a mom-focused one. 24% cheaper and I choose my own doctor 😌"** — appears on three ads holding **$29,814.72** of lifetime spend. Two of those three carry a Meta `effective_status` of **DISAPPROVED**. `verified` for the status; I cannot see Meta's stated reason and I am not claiming the claim caused it.
- Headline, verbatim: **"Moms, save 20% on your health insurance"** — ad `IMG 2`, $495.16 lifetime, created 2024-12-10.

This is not confined to old statics. The same "saving you 20% or more" body copy sits on 2026 video ads too, including `Moms43 - 4 - V4` at $23,986.38 lifetime and `MOMS32 - N1 - V10` at $739.70. It reads like a default body copy block that has been carried forward across the account for two years.

**Standing: off-limits by the brand's own rule.** The brand states it cannot make a flat savings claim. It has made one, at scale, and is still carrying it. Two facts also sit against the rule and are worth recording: the flat number is **20%**, not 30%, and the "24% cheaper" line is a specific figure attributed to a first-person testimonial. None of the three numbers, 20%, 24% or 30%, has a stated basis of comparison anywhere I could find.

**Where the live winners do hold the rule.** This is the other half of the picture and it is genuinely good news. Every one of the eight top-spending ads I pulled with full transcripts holds the qualifiers correctly. `verified`, from the transcripts:

- "letting Health for Moms save you **up to 30%** for better coverage like $0 deductibles" — `Moms43 - 5 - V1`, 0:18
- "Check your family's options with Health for Moms today and **save up to 30%**" — the closing voiceover on `Moms43 - 5 - V1`, `moms-63 2b` and `moms-63 3e`
- "you **may be able to** get a $0 deductible plan with better premium rates" — `moms-63 2b`, 0:24
- "you **may qualify for** a health plan with a $0 deductible and potentially better premium rates" — `moms-63 3e`, 0:28
- "see if you **qualify for** lower premiums and a $0 deductible" — `moms-53 3`, 0:12

So the currently-scaling video creative is compliant with the brand's own claim rules and the legacy body copy is not. That is a clean split and it is the kind of thing a later reader needs to know before they reach for any existing asset as a reference.

### The claims that need the brand to resolve them

Per this prompt's instruction, I am flagging rather than deciding. For each of these the legal standing is not established by anything the brand provided, and each would matter in advertising:

1. What "up to 30%" compares against, and whether any real case has reached it.
2. What "nationwide coverage" means for a mom whose state is not on the Approved State List.
3. Whether the "20% or more" and "24% cheaper" copy is approved, grandfathered, or an oversight that should be pulled.
4. The source behind each of the four statistics above, particularly the bankruptcy line.
5. Whether MomSmart Coverage Method™ is a registered mark, and what the underlying mechanism actually is.

---

## Compliance and legal guardrails

Recorder's role only. What follows is what the brand itself states about the rules it operates under, kept in the brand's own framing. I am not inferring legal limits the brand has not stated and I am not deciding whether any claim is permissible.

### The brand's own framing of firmness

The brand draws the line itself. Section 8 opens with: **"THIS SECTION IS NON-NEGOTIABLE. Every constraint listed here is a hard rule."** Section 7's tone list is labelled the opposite way: "stylistic preferences, not compliance rules." I am carrying that distinction exactly as given.

**Risk tolerance: 75**, on a scale the brand context document reads as "moderate-to-high tolerance for direct response approaches, while remaining within clear guardrails." `stated`.

### Restricted claims, verbatim

From the brand-provided compliance data:

- **"Dont give any HARD guarantees"**

From the guidelines, marked non-negotiable and specific to this brand:

- **"Savings claims: always 'up to 30%' — never drop the 'up to'"**
- **"Deductible claims: always '$0 deductible option' or 'options with no deductibles' — never state it as a flat/guaranteed outcome"**
- **"No fabricated statistics; no named competitor attacks; no government/ACA references"**
- **"No scare tactics, no political or partisan language, no punching down at demographic groups"**
- **"The villain in any narrative is always the system/mechanism — never a named company or individual"**
- **"A doctor character in a script requires either a real licensed physician or adjusted language that doesn't imply a false credential"**

### Required disclaimers

**None specified.** The brand context document says plainly: "No specific disclaimer text was provided." It notes that the two claim qualifiers function as de facto disclaimers instead. Any savings claim must carry "up to," and any deductible claim must be framed as an option. `stated`.

The Phase-1 ad-account pull observed an on-screen dramatization disclaimer in the winning scripts. That is one disclaimer the brand does carry in practice even though it never wrote it down as a requirement.

### Platform restrictions

**The brand reports none, and the account contradicts that.**

The brand context document says: "No specific platform rejection history or known triggers were provided." `stated`.

But at least two ads in the live library carry a Meta `effective_status` of **DISAPPROVED**, both variants of `B1 - Copy 7`, holding $8,553.74 and $5,048.37 of lifetime spend. `verified`, Parker MCP, pulled 2026-09-03. I cannot see Meta's reason and I am not attributing it. What I can say is that the brand's own record of its platform history is incomplete, and the account holds the evidence.

This matters more than it might for a normal category. Health insurance is a policed advertising category, and platform moderation runs in four layers rather than one: automated filters, human reviewers, engagement signals and policy enforcement. On Meta specifically, human reviewers are in the loop, so the durable posture is legitimate framing and full compliance rather than clever wording. The brand's instinct here is already right. Its villain rule keeps the system as the antagonist rather than a named carrier, which is exactly the framing that survives review, and its qualifier rules are the accurate-claims discipline that no amount of good creative substitutes for. The gap is not the posture. The gap is that nobody has written down what has already been rejected and why.

### Internal guardrails the brand set for itself

These are things the brand has decided not to do even where it might be allowed to. All verbatim from section 8:

- **"No political or partisan framing"** — the document notes the brand "deliberately avoids taking sides," and section 9 records the brand's own testing verdict on this in its own words: **"Anything political doesnt work."**
- **"No pregnancy-only targeting — focus on moms with kids (not expectant mothers exclusively)"**
- **"Avoid corporate or overly clinical tone"**
- **"Avoid scare-heavy copy"** — the brand says it "can use direct response principles but should focus on reassurance and clarity"
- **"No named competitor attacks — the system is the villain, never a specific company"**
- **"No government/ACA references"** — the brand "positions itself in the private market space and avoids any association with government programs"
- **"Words never used in creative: cheap, discount, policy, ACA, exclusions, guaranteed"**

### What I checked against the running work, and what I found

I ran keyword sweeps of the full 2,122-ad library against the brand's own banned-word list, on 2026-09-03. Recording the results rather than judging them:

**The villain rule holds.** The account's most aggressive hooks keep the antagonist as the category, never a named company. Verbatim text hooks: "Health Insurance is a scam 🙄", "Big Health Insurance is a scam!!!", "American health insurance is a scam", "Insurance companies PREY on moms, Watch what happens to this one...". Not one names a carrier. `verified`, from the ads' own hook fields.

**"Guaranteed" — one match, unconfirmed.** One ad out of 2,122 matched the keyword, `MOMS32 - N1 - V10` at $739.70 lifetime. The word did not appear in any copy field the response returned, so I could not confirm which field carried it or whether the match was exact. `data-limited`.

**"Discount" — no brand copy match found.** Eleven ads matched, but in every case I could inspect, the match sat in Parker's own AI-generated `angle` field, such as "Direct financial savings (20% discount)," not in brand copy. `verified` for the ones I could read.

**"Marketplace" — 20 matches, unconfirmed.** Twenty ads matched, holding $5,053.16 of lifetime spend combined. The word did not appear in any returned copy field on the five I inspected, so it likely sits in transcripts or AI analysis. I could not confirm. `data-limited`, and worth a look given the brand's no-government-references rule.

**Government-adjacent framing in a small paused set.** Three ads in the `MOMS25 - 5TH DEC - Y1` set, holding $436.08 of lifetime spend between them and all paused or in paused ad sets, carry framing that brushes the brand's own rules. Verbatim verbal hooks: "This is what happens when you stop paying for everyone else's healthcare" and "making over 50k just disqualified this family from affordable healthcare, but it secretly qualified them for something way better." `verified`, from the ads' own hook fields. The first reads as subsidy resentment, which is close to the political line the brand bars. The second is a near-direct reference to government eligibility, which the no-ACA rule bars. Both are tiny in spend and both are off. I am recording them so nobody pulls them forward as references.

### What to route to the brand

Per the prompt's instruction, these are the compliance questions I am not resolving:

1. Whether the "20% or more" and "24% cheaper" copy was approved at the time, and whether it should be pulled from every asset that still carries it.
2. Meta's stated reason for the two disapproved ads.
3. Whether "marketplace" appears in any spoken script, and if so whether it trips the no-government rule.
4. What the required disclaimer text is, if one exists, since the brand states none was provided.
5. Whether the on-screen dramatization disclaimer the account already runs is a formal requirement or an ad-hoc habit.

---

## Open loops

Four. Each one is a thing this pass genuinely could not resolve that would change what the brand does if it were answered. All four route to the brand, because all four live inside the business and leave no public trace.

**1. What the savings number is measured against.**

Every claim this brand makes about value rests on one figure, "up to 30%," and I found nothing anywhere that says what it compares to, how it was calculated, or whether any real family has hit it. At the same time the account has carried a flat "20% or more" across roughly two thirds of its lifetime static spend, and a "24% cheaper" testimonial headline on another $29,814.72, while the brand's own guidelines call a flat savings claim non-negotiable and forbidden.

*Pull: Tension.* The brand's own hard rule and the brand's own running copy cannot both be right, and neither one names a basis for the number.

*Question:* What does the "up to 30%" savings figure actually compare against?

*Why it is a loop:* This number is the brand's central promise and the thing every ad ends on. If it compares against a specific baseline the brand can name, the claim gets stronger and more specific, which is exactly what the brand's own specificity principle asks for. If nothing sits behind it, the brand's biggest claim is its most exposed one and every asset carrying a flat version of it is a live risk.

*Territory: Messaging.* **Routed to the brand.**

**2. What "nationwide" means for a mom whose state is not on the list.**

The brand's stated benefit list opens with "Nationwide coverage — see any doctor, anywhere in the U.S." The mechanism that closes nearly every ad says the opposite about availability: "you have to live in one of those states, otherwise it's not gonna work." The Approved State List runs to 32 to 34 states in all thirteen ads read at full media depth.

*Pull: Tension.* The brand's headline benefit and the brand's own qualifier point in different directions, and nothing in the brand's materials reconciles them.

*Question:* What does Health For Moms have to offer a mom whose state is not on the Approved State List?

*Why it is a loop:* The state gate is the brand's best-known creative device and its answer to a compliance requirement at the same time. If there is a real offer behind the gate for the other states, that is a whole audience the brand currently turns away at the door. If there is not, then "nationwide" is describing something other than availability and the brand needs to say which.

*Territory: Product.* **Routed to the brand.**

**3. Who this brand's team actually believes it serves.**

The brand carries five canonical ICPs. At least one of them, Jen, is word for word a bucket description Parker wrote in a Slack thread on 2026-09-03 from the brand's own guidelines, which the brand then adopted into its canonical list. The demographic criteria behind those buckets, 28 to 50, married or partnered, one to three kids, $50K to $150K+, reach me only through Parker's report of the guidelines, not from the guidelines themselves. And the most recent thing the team typed contradicts one of those criteria outright: "honestly single moms are fine just as long as we also use lingo about them not being broke."

*Pull: Surprise.* I expected the brand's claimed personas to be the brand's own independent knowledge. At least one of them is the brand agreeing with a read Parker handed back to it, which is not the same thing at all.

*Question:* Who does this brand's team actually believe it serves?

*Why it is a loop:* Persona routes everything downstream. If the brand's stated audience is partly a mirror of a machine read, then a later step that treats the five ICPs as brand knowledge is building on something softer than it looks. And the single-mom override is a real, recent, hand-typed change to the audience that has not been folded into the canonical list yet.

*Territory: Personas.* **Routed to the brand.**

**4. What the MomSmart Coverage Method actually is.**

The brand's whole differentiation rests on a named, trademarked mechanism it calls "new tech that scans plans and matches each family with the right private health plan based on their needs, doctors, and budget." That description is the only account of it anywhere I could reach. The guidelines also build one of three sanctioned CTA frameworks on top of it, the Mechanism CTA, with a Tech/Scan framing.

*Pull: Curiosity.* A trademark symbol and a named method imply something specific exists, and nothing in the brand's own materials says what.

*Question:* What is the MomSmart Coverage Method made of?

*Why it is a loop:* A named mechanism is one of the strongest assets a brand in a crowded category can have, and it is also one of the easiest to overclaim. If there is real matching technology behind it, the brand can lead with it and get specific, which is what its own guidelines ask for. If it is a name on a routing form, then the Mechanism CTA is asking creative to promise something that cannot be shown, and the brand should know that before it builds a third of its CTA architecture on it.

*Territory: Product.* **Routed to the brand.**

*Creators and talent* is genuinely clean for this doc. The brand states one talent rule, that a doctor character requires a real licensed physician or adjusted language, and it is a settled rule rather than an open question. Casting questions for this account exist and they are real, but they live in the ad-account read where the creative evidence sits, not here.

---

## Appendix - Parker media links

Every media handle available during this run, grouped by source so a strategist can reopen the exact material.

### Top-spending video ads read at transcript level, 90 days to 2026-09-02

**`Moms43 - 4 - V3`** — account top spender, $42,741.16 in window
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

**`Moms43 - 5 - V1`** — grievance opener, $10,020.57 in window
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120243987355020519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0fe2980848d12fe1c6fd107a759e68fe37d8776c34235b5fab3c15e751af171d.mp4

**`Moms43 - 4 - V1`** — $6,993.31 in window
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380110519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/f18c5a15a13e4412e35f654034f63f147ca73e40b35538419d22500d143b670d.mp4

**`Moms43 - 4 - V4`** — carries the flat "saving you 20% or more" body copy, $23,986.38 lifetime
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380050519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/985c6a8045a5bcfb5e7450ad0f3a00ca783b996f4ba3633337e8c84e1aac8a39.mp4

**`moms-63 2b`** — holds the "up to 30%" and "may be able to" qualifiers correctly
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4

**`MOMS34 - N1 - 3a`** — carries "Finally, insurance that actually feels like it has our back"
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238654140050519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1c501ac53c00f4e6b9f3ee87626968c02aa9861c6958bcf6c338644cbaf1fa8d.mp4

**`moms-63 3e`** — objection pre-empt, holds "may qualify for" correctly
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4

**`moms-53 3`** — the clearest mom-to-mom register in the account
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4

### Statics carrying the flat savings claim

**`B1 samar- Copy`** — $35,219.98 lifetime, headline "Didn't know I could ditch my job's health plan… until I did."
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227092765930519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b219b0aa7f7e7ed8d83fa471803f4b6c96ad98b2de118b2a8e68038439e759a9.jpg

**`B1 - Copy 7`** — $16,212.61 lifetime, headline "Left my big insurance company for a mom-focused one. 24% cheaper and I choose my own doctor 😌"
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120216241083030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/7e3133fccf8b205622146f7297669b76296123fb46177e5262ee89f0040ca8ba.jpg

**`B1 - Copy 7`, Parenting - New ad set — DISAPPROVED by Meta**, $8,553.74 lifetime, same 24% headline
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120216241083360519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

**`B1 - Copy 7`, Parenting B1 ad set — DISAPPROVED by Meta**, $5,048.37 lifetime, same 24% headline
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120216241083390519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

**`B2 - 10TH JUNE - Copy 16`** — $15,660.83 lifetime, ad title "Approved by thousands of Mom's across America"
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120224683440990519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/2196cede33edbb670d810d017aa0c57568dc50db2e8c71b7b7a608410b0c0aae.jpg

**`B1 samar- Copy 1`** — $14,633.08 lifetime
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227092759640519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

**`B1 samar- Copy`, Broad | B1 - Copy 32** — $14,202.08 lifetime, headline "I changed our health plan, got $0 deductible options, and picked our doctors with no networks."
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120227093054710519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/4c9b4f3dd99bdcfcc853b3db5657e2e14e78af6c7ca04c93bb85db49bb62f034.jpg

**`OMC-Health for Moms-[B3-C11-V7]`** — $10,947.56 lifetime
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120232855500240519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

**`5TH APR - Copy 29`** — $7,188.80 lifetime, headline "One ER visit could've wiped us out."
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120219260803030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/45224b0b0e41a9bf1b7f5d5615b382462b10f5e321ab7875df4adcbb3870f17c.jpg

**`IMG 6`** — $4,616.70 lifetime, headline "Moms, your health insurance should cover preventative care..."
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120212962324900519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/14f1fb45d1b0308a5b25ce5cfdb6b2b7f9116c569643058dc4ba2d6965e51a55.jpg

**`IMG 2`** — $495.16 lifetime, headline "Moms, save 20% on your health insurance"
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120212331320610519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/c3494f4c333ffc0e47145ddd9044bea5f1491268a803c829466655b8ef1414e7.jpg

### Ads carrying banned-word or guardrail-adjacent copy

**`MOMS32 - N1 - V10`** — the single "guaranteed" keyword match, $739.70 lifetime
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238096464200519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/f3871878bcd74c7bf59adf0d62f59a777d196b79a6a07cde5eec0ffdf63428cc.mp4

**`MOMS25 - 5TH DEC - Y1 - Copy 6`** — "This is what happens when you stop paying for everyone else's healthcare," $209.46 lifetime
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120235426345340519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/a01892290fc6576daeeb9211ec13689cbca0d4f7cc96db73c89ddf63c9aa35cb.mp4

**`MOMS25 - 5TH DEC - Y1 - Copy 5`** — "making over 50k just disqualified this family from affordable healthcare," $92.60 lifetime
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120235426343210519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/c9fc4d3728ca9cdd2c6ce4059f93365dbac70700a7dff0b04e2f88f969068516.mp4

**`MOMS25 - 5TH DEC - Y1 - Copy 4`** — "I feel like I unlocked a cheat code for the American health care system," $134.02 lifetime
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120235426339240519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/cfdf4257bd8375968e71dcfba8e6cdc4426b51c7980669627d118d043ed5bc8f.mp4

**`MOMS 29 - 4 - H4 - B1 - C3`** — "American health insurance is a scam," villain kept on the system
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120236999054070519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/02723b36b67b45bf2fe166382a8b72d7df1837a1b8f73fdddf571b318cfa37b5.mp4

**`MOMS32 - N5 - V16`** — "Insurance companies PREY on moms," $556.54 lifetime
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238542309300519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/7dd42a615bd64b6bdf12cf05bb0711fd781cf9899f62a75f25674761173ab6b3.mp4

**`B2 - 10TH JUNE - Copy 1`** — headline "If you're self-employed, between jobs, or just tired of paying too much...", $1,819.83 lifetime
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120224684049440519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/45c5cbc54f430c3c07a32a71077cdc97e1329a6f91856c6fbce9fef811164548.jpg

**`MOMS32 - N2 - V28`** — "The Perfect Health Insurance doesn't exi... 🤯", $63.01 lifetime
- Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238260786060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/86553c6b60822e3a73c9d0fc507009b7f8a19954f5ade69f3572d74738e0ee7a.mp4

### Brand-owned destinations

- Primary landing page on every top static: https://www.healthformoms.co/save/
- Quiz funnel named in the Phase-1 ad-account pull: https://quiz.healthformoms.com/#/indvfam
- Brand site attempted and blocked by this environment's network proxy: https://healthformoms.com

### Team conversation sources

- Parker web thread `b4aa53c3-f10e-4ecb-9612-c40f39803f6a`, "Parker Brain setup," 2026-09-03. Tooling only, no brand content.
- Parker Slack thread `1788469337.157819`, 2026-09-03. Carries the ICP correction, the guidelines criteria, and the single-mom override.
- Parker Slack thread `1788473402.812619`, 2026-09-03. Carries the confirmation that no customer reviews exist.
- Parker Slack thread `1788469337.613099`, 2026-09-03. Ad account overview request.

### Prior source docs read

- `source-pulls/ad-account.md` — 13 ads read at full media depth with transcript, AI creative analysis, creator demographic and delivery split.
