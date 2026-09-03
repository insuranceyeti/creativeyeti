---
brand: health-for-moms
doc: reddit
generated_on: 2026-09-03
refresh_by: 2026-10-03
sources_read: []
threads_read: 0
reddit_reachable: false
substitute_sources_read:
  - Facebook and Instagram ad comments, Meta ad account HealthForMoms, act 484897827497337, via Parker MCP search_facebook_ad_comments_sql. Eleven targeted string searches against the full 1,322-comment corpus on 2026-09-03, plus one wholeThread pull.
  - Parker MCP search_customer_reviews_sql, unfiltered, 2026-09-03. Returned totalReviews 0, re-confirming the dark surface live rather than carrying it from a note.
  - Parker MCP get_brand_persona, the full brand context document, read for the five stated ICPs and the brand's own account of its partner agencies.
  - Parker MCP search_chat_history, Slack thread 1788473402.812619 dated 2026-09-03, read to confirm the exact wording of the team's instruction that sanctions Reddit as a substitute source.
  - source-pulls/ad-comments.md, personas/voice-of-customer/voc-corpus-profile.md, running-notes/missing-context.md, running-notes/brand-rules.md.
data_limitations:
  - "Reddit is unreachable from this session, confirmed by three separate routes on 2026-09-03. WebFetch on https://www.reddit.com/r/HealthInsurance/ returned 'Claude Code is unable to fetch from www.reddit.com'. WebFetch on https://old.reddit.com/r/HealthInsurance/ returned the same refusal. WebSearch restricted to reddit.com returned 'API Error: 400 The following domains are not accessible to our user agent: [reddit.com]'. A third-party Reddit mirror was refused by this session's network egress proxy with EGRESS_BLOCKED."
  - "The block is not only this sandbox. General web search works from this session and returned live non-Reddit results for the same query. Reddit specifically is excluded from the search tool's crawler at the provider level, so a session with ordinary network access would hit the same wall. Closing this gap needs a different route: an authenticated Reddit API pull, a licensed data provider, or a human pasting thread text into the brain."
  - "Because no community was read, every mandated section below is a named blank for its Reddit lane. No identity, state, problem-frame, or trusted voice in this doc is sourced from unprompted community discussion, because none was available."
  - "The substitute evidence is Facebook ad comments sitting under the brand's own paid creative. That is a brand-controlled surface and the exact opposite of what this doc is built to read. It cannot perform this doc's central job, which is checking whether a signal is real pull or the brand hearing its own words come back. It is carried here only to show what the question looks like from inside the brand's own surface, and it is labelled as such on every claim."
  - "Exactly 1 of 1,322 comments (0.08%) mentions Reddit, and it is a pasted second-hand summary of Reddit threads, not a Reddit thread. Nothing in it was verified against a real post."
  - "Customer reviews and post-purchase surveys are both zero rows, re-verified live today. So this brand currently has no independent check on any persona signal from any surface."
  - "No get_current_time tool exists on this MCP surface. The 2026-09-03 date comes from the session clock and matches the date stamped across the rest of this build."
  - "refresh_by is set 30 days out rather than the 180-day persona-source cadence in parker-system/system/refresh-cadence.md. This doc is a blank waiting on access, not a photograph of a moving thing, so it should be re-run the moment a session can reach Reddit rather than waiting six months."
---

# Reddit — persona signal — Health For Moms

## What this run could and could not do

This doc is mostly empty, and the emptiness is the finding. I want to be exact about what was tried before anyone reads a blank as laziness.

Reddit was tested first, before any analysis, because the whole doc depends on it. Three routes, all refused on 2026-09-03. Fetching `https://www.reddit.com/r/HealthInsurance/` came back "Claude Code is unable to fetch from www.reddit.com." The old.reddit.com mirror of the same page came back the same way. Searching the web with results limited to reddit.com returned a hard 400: "The following domains are not accessible to our user agent: ['reddit.com']." A third-party Reddit mirror was then refused by this session's own network proxy with EGRESS_BLOCKED.

One detail matters more than the refusals themselves. General web search works fine from here. The same kind of query about health insurance for moms returned live pages from five different sites. So this is not a session that cannot reach the internet. It is a session that cannot reach Reddit specifically, and the search-side refusal names the crawler's user agent rather than this sandbox. A strategist should read that as a standing gap, not a one-time glitch. Getting Reddit into this brain needs a different door: the Reddit API with credentials, a paid data provider, or a person copying threads in by hand.

I did not reconstruct Reddit from memory, and there is no paraphrase of a remembered thread anywhere below. Everything quoted here was pulled live today through Parker.

What I did instead was ask a narrower question the available tools can actually answer: what does this brand's own comment corpus reveal about the community question, and what would Reddit settle that nothing else can? That produced a real partial contribution to one of the six sections and honest blanks in the rest.

Two things to hold while reading. First, the substitute surface is Facebook ad comments under the brand's own paid ads, which is a brand-controlled surface. This doc exists precisely to be the check on that surface, so using it here cannot close the loop. It can only show the shape of the hole. Second, this brand has no customer reviews and no post-purchase surveys, both re-verified live today at zero rows. Under the persona method's evidence ranking, survey data sits at the top and community comment sits near the bottom, and this brand holds nothing but the bottom rank of a single source. Reddit was the sanctioned way out of that, named by the team itself in Slack on 2026-09-03: "we don't have reviews but you can pull from competitor reviews or health insurance Reddit etc." That door is currently shut.

## Identity signals observed

**Blank. No identity signal was gathered, because no community was read.**

Zero communities, zero threads. I am not going to name an identity from a source I could not open, and I am not going to promote an identity out of `source-pulls/ad-comments.md` and relabel it as community signal. That would be laundering, and it would quietly destroy the one thing this doc is for.

What I can say is what the blank costs, and it is not small. The eight identities in `source-pulls/ad-comments.md` are all marked mixed or thin confidence, and every one of them carries the same caveat: nothing exists to check it against. The insured mom who is still broke, at 160 self-disclosed dollar figures across 17 ads. The employer-plan captive. The chronic-condition mom the underwriting screens out. The self-employed mom in the income gap. The insurance insider correcting the script. All of them are currently one-source reads from a public comment section. Reddit is the source that would have told us which of those are real people in the category and which are artifacts of who Meta served a cheap, wide-reaching ad. That test did not happen.

One narrow, honest observation about identity, marked **inferred**, and drawn from the substitute surface rather than from any community. The people in this brand's comment sections speak the category's language far better than the creative assumes. Across 1,322 comments, "deductible" appears in 207 (15.7%) and "out of pocket" in 74 (5.6%), and the full read classified 103 comments across 13 ads as people telling the brand it used the word wrong. Beyond the correction itself, commenters trade real technical terms without explaining them: guaranteed issue, medical underwriting, coinsurance, subsidy, certified application counselor, Direct Primary Care. One comment on 2026-08-21 reads: "Marketplace plans are guaranteed issue by law, meaning there is no medical underwriting, as long as he's eligible to enroll during a valid enrollment period. Marketplace plans cannot deny him coverage or charge him more because of a pre-existing condition." Nobody wrote that for a brand. She wrote it for another mom.

That is a hint about who is really in this category, and it is only a hint. It sits on a brand-controlled surface, under an ad that put the word "deductible" on screen and so invited the correction. Whether this fluency is native to the buyer or manufactured by the ad is exactly the question this doc was supposed to answer. Confidence: **thin**, and deliberately left unresolved.

## Behavioral-signal states observed

**Blank. No states were observed, because no discussion was read.**

The states in `source-pulls/ad-comments.md` stay where they are, as candidates. Deductible-reset dread that spikes at New Year. Open-enrollment lockout. An acute medical event already on the calendar. A benefits change in the household. Phone-call avoidance. Post-form burn. Geographic exclusion. Each of those was read off a comment section under a paid ad, which means each of them may be a state the ad provoked rather than a state the person was already in.

That distinction is the reason a state read matters at all. The emotional-delivery method draws a hard line between the state the creative produces and the state the viewer was already sitting in when it arrived, and says the distance between those two is where the cost per lead lives. A comment section can only show the first. An unprompted community shows the second, because people post there before any ad reaches them. So this brand currently has no read on the landing state at all, only on the reaction state. That is a real hole in the persona system and it stays open.

## How the community frames the problem

**Blank for the community. The native frame was not observed.**

This is the section the doc would have earned its keep on, and it is the one hit hardest. The point of reading a topical community is to hear how people describe the problem before a brand teaches them a way to say it. That read did not happen.

What did surface is a specific, checkable echo problem that Reddit would settle in one pass, and naming it precisely is the most useful thing this doc can do today.

The brand's best-performing creative, `MOMS38 - 1 - V1`, opens with the words "Health Insurance is a scam 🙄" on screen. The word "scam" then appears in 45 of 1,322 comments (3.4%), across 12 different ads. `voc-corpus-profile.md` already flagged this and marked it honestly: some of that is genuine customer language that predates the ad, some is the audience repeating the ad back, and the two cannot be separated inside this corpus. The same doc marked a second phrase as confirmed echo. The ad `MOMS39 - 2 - V2` overlays a tweet reading "My deductible is $6000... Make that make sense...." and commenters then write "Health care for moms but you don't qualify if your pregnant? Make that make sense." The brand handed the audience a sentence and the audience handed it back.

So the brand's voice bank currently holds at least one phrase that is definitely echo and one large cluster that might be. There is no way to tell from inside the brand's own surface, by definition. An unprompted community is the only instrument that reads this, and the test is simple: does a mom in a health insurance community call the category a scam when no ad has just said it for her? That question is unanswered.

One more piece of frame evidence, marked **stated** and carried carefully because it is second-hand. Exactly 1 of 1,322 comments mentions Reddit at all. On 2025-01-13, under the ad `IMG 6`, a commenter pasted what reads as a search summary of Reddit discussion about this brand. It drew 14 likes and 10 replies. Here is the load-bearing part of it, verbatim:

> "According to discussions on Reddit, "Health for Moms" insurance is generally considered not legitimate and likely a scam, as many users report extremely limited coverage, difficulty cancelling policies, and concerns about the company's practices not aligning with standard health insurance expectations; it's often advised to research and purchase health insurance through reputable sources like the Health Insurance Marketplace instead."

That is a commenter's summary of a forum nobody has verified, not a Reddit post, and I am not treating it as one. What it does establish is that Reddit already holds a verdict on this brand, that at least one person went there to check, and that what she found was hostile enough to paste under a live ad where 14 people agreed with it. That raises the value of a real Reddit pull rather than substituting for one.

## Trusted voices and recommendation paths

**Blank for the community's own trusted voices.** No community was read, so nobody's deference, warnings, or recommendations were observed in their native setting.

This is the one section where the substitute surface makes a genuine partial contribution, so I am carrying it with its denominators and a clear label. Everything below is Facebook ad comments under this brand's paid creative, pulled live on 2026-09-03 by string search across the full 1,322-comment corpus. It is not community evidence. It is a picture of what happens when a woman has nowhere else to ask.

**Where the audience actually points each other, counted against 1,322 comments.**

| What the comment names | Comments | Share of 1,322 |
|---|---|---|
| The Marketplace or healthcare.gov | 14 | 1.1% |
| Medicaid | 17 | 1.3% |
| A broker, named as a person to work with | 4 | 0.3% |
| A licensed agent, self-identified | 10 | 0.8% |
| Google, as the place to check the brand | 2 | 0.2% |
| Reddit | 1 | 0.08% |
| A friend's situation, cited as evidence | 3 | 0.2% |
| The word "recommend" in any form | 5 | 0.4% |
| The word "forum" | 0 | 0% |
| The word "group" | 0 | 0% |

Read the last two rows carefully. Not one comment in 1,322 uses the word "group" or "forum." For a brand whose entire audience is mothers on Facebook, where mom groups are the obvious peer channel, that absence is worth noticing. It is not proof the channel does not matter. It is proof this corpus cannot see it, which is a different thing and points at the same missing source.

**The peer-verification behavior, which is the sharpest thing in this section.** The highest-liked question in the whole corpus is not about price or eligibility. It is a request for a review. On 2026-03-20, under `MOMS38 - 1 - V1`, someone wrote:

> "Anyone actually have this and have insight?"

Fifteen likes and six replies, and I pulled the full thread. The brand did not answer. Other commenters did, and here is what they told her, in order:

> "April Crawford wondering the same. I filled out something like this years ago- and got spam phone calls every 10 minutes for months!" — 2026-03-29, 5 likes

> "That's exactly what will happen here. Their website says they are a third party agency to connect you to agents. You'll get hundreds of calls and the plans aren't great. Website says they don't guarantee coverage or plans. They are hoping you sign up for a "cheaper" plan on paper but really it doesn't cover anything." — 2026-04-01, 2 likes

> "I was connected to a very helpful agent. They weren't able to find a lower price for our particular situation but he was very kind and helpful and respectful." — 2026-04-01, 1 like

> "April Crawford I was told I don't qualify 🤷" — 2026-04-02, 1 like

> "Jamie Abernethy Same" — 2026-04-07, 1 like

My read, marked **inferred**: that thread is a review section forming on its own inside an ad. She asked the question you ask on Reddit, in the only room she had, and five strangers ran the verification for her. Four of the five answers were negative or neutral. Two other commenters had already tried the other obvious route and found nothing: "How come when I search for this on Google, nothing comes up?" on 2025-08-07, and "A Google search doesn't pull anything about this. Is it legit?" on 2025-07-24.

So the verification path for this brand runs through peers, and right now it runs through peers inside the brand's own paid media, where the brand is not participating and the answers are mostly bad. Confidence: **mixed**. The behavior is verified and the thread is real, but it is one thread, and one thread is a candidate, never a pattern.

**Two more paths worth logging.** The community teaches each other things the brand never says. On 2026-05-05 a commenter explained to another commenter that "if it's an employer insurance, you don't have to sign up with that employer insurance you can decline the coverage and go out and find your own insurance carrier." On 2026-04-04 another simply asked, "Ingrid Zagers have you checked marketplace? There has got to be better coverage. That's insane," and drew 4 likes. And on 2026-03-28 one commenter routed another to a professional: "I highly recommend you call insurance sales person. There is a possibility that you may be able to find a cheaper option for yourself with no deductible."

Then there is the path that points away. 39 comments across 10 ads are rival agents and brokers pitching their own offers under this brand's creative, per `source-pulls/ad-comments.md`. One on 2026-05-20 makes the pitch as a philosophy rather than a link: "Affordable insurance that actually works still exists in plenty avenues even for those with high income. You just have to work with brokers that care and are knowledgeable enough to show you the right products." Of the five comments in the whole corpus using the word "recommend," three are negative or point elsewhere, including "I got pushed around and given to a side insurance company. I had already done all of that and then some and tried this, so no I DO NOT RECOMMEND!" from 2026-02-04, with 4 likes.

The honest summary: inside the surface the brand pays for, the recommendation flow points at the Marketplace, at Medicaid, at independent brokers, and at rival agents. It does not point at Health For Moms. Whether that also holds in a real community is unknown and is the single most valuable thing a Reddit pull would tell this brand.

## Corroboration and contradiction

This is the section the doc exists for, and it is the one that must be reported as a failure rather than dressed up.

**Nothing was corroborated. Nothing was contradicted. No independent test was run.**

Say it plainly for the synthesis: as of today, every persona signal Health For Moms holds comes from one brand-controlled surface, and there is no unprompted source anywhere in the brain to check it against. Customer reviews are zero rows, re-verified live today. Post-purchase surveys are zero rows. No competitor brands are tracked, so there is not even a category baseline. Reddit was the sanctioned substitute and it is unreachable. That means the confidence ceiling across the whole persona system stays at **mixed**, and the synthesis should not round any identity up past that no matter how many times a phrase recurs in the comments. Recurrence inside one noisy source is still one source.

**What would have been tested, named precisely, so a later run knows exactly what to look for.** These are the four signals from the brand-controlled surfaces most at risk of being the brand hearing itself:

1. **"Insurance is a scam."** The winning ad puts it on screen; 45 of 1,322 comments use the word. The test: do moms in health insurance communities reach for "scam" unprompted, or only after an ad hands it to them?
2. **"Make that make sense."** Already confirmed as echo in `voc-corpus-profile.md`, since the brand's own tweet-style creative used it first. It must not enter the voice bank as customer language. Reddit would show whether the phrase has any independent life in the category.
3. **The deductible correction.** 103 comments across 13 ads say the ad describes an out-of-pocket maximum, not a deductible. This one looks least likely to be echo, since self-identified brokers and medical billers are among the correctors, but it has never been checked outside the brand's own ads.
4. **The pregnancy exclusion.** 42 comments across 15 ads over fourteen months, the widest objection in the corpus, and it is not on the brand's own stated objection list at all. Whether it also travels outside the ad section is unknown.

**The one contradiction available today, and it is a fragment.** Marked **stated**, carried as a flag rather than a finding. The brand context document describes Health For Moms as working "exclusively with partner agencies described as honest and trustworthy," and describes those agents as "like your Mom BFFs - friendly and approachable." The only outside verdict that has ever reached this corpus says the opposite: that the brand is "generally considered not legitimate and likely a scam," with "difficulty cancelling policies" and plans that "may not comply with Affordable Care Act (ACA) standards."

Those two accounts cannot both be right as stated. The prompt's own source-side bias says that when an unprompted source and a brand-controlled source disagree, the unprompted one is more trustworthy. I am not applying that rule here, and I want to be clear about why. What reached the corpus is not an unprompted source. It is a commenter's pasted summary of one, unverified, second-hand, from January 2025. It carries no thread, no subreddit, no date, and no post. So it settles nothing. What it does is raise the stakes: there is a live verdict on this brand sitting somewhere the brain cannot currently see, it is bad, and at least one prospective customer already found it.

## Recurrence and spread

The plain accounting, so the denominator is never guessed at downstream.

**Communities read: 0. Threads read: 0. Comments read inside communities: 0.** No subreddit was opened. No cross-community recurrence check was possible, and cross-community agreement is the strongest evidence this doc can normally produce, so its absence is total rather than partial.

**What was read instead, with its denominators.** The full Facebook ad comment corpus for this brand, 1,322 comments, is the base for every count in this doc. It spans 2025-01-08 to 2026-09-03, sits on 112 distinct ad IDs and 79 distinct ad names, and is heavily skewed: 846 of 1,322 (64.0%) were posted in March and April 2026, and 795 of 1,322 (60.1%) sit on the single `MOMS38 - 1` creative family. Any rate quoted from it is a rate inside that skew.

Against that base I ran eleven targeted string searches live today and one full-thread pull. The results, each verified by the tool's own total: reddit 1, forum 0, group 0, broker 4, marketplace 14, legit 4, google 2, recommend 5, friend 3, "anyone actually" 1. Two further counts were carried from `voc-corpus-profile.md`: medicaid 17 and agent 10.

**Spread of the one Reddit-touching signal: a single comment, on a single ad, on a single day.** `IMG 6`, 2025-01-13, comment_id `f55ae3d8-afcd-1903-3bcb-6e2de2bc0bbb`, 14 likes, 10 replies. One comment out of 1,322 is 0.08%, which is as thin as evidence gets. It is logged because it is the only Reddit artifact that exists in this brain, not because one comment supports anything.

**Spread of the peer-verification behavior: one thread, six comments.** `MOMS38 - 1 - V1`, opened 2026-03-20, replies running through 2026-04-07. One thread is a candidate, not a pattern, and it is marked that way above.

**What no amount of work on the available surfaces can produce.** Which identities populate health insurance communities. How those communities frame the cost problem before a brand teaches them. Whom they trust and warn against among themselves. Whether any signal this brand holds is real pull or its own echo. All four need the source that is blocked.

## Open loops

Five loops came out of this run. The blocked access itself is not one of them, because a tooling and source gap routes to `data_limitations` under the rubric, and it is recorded there in full. Every question below is one a reachable Reddit session could answer, and none of them needs data only the brand holds.

**1. There is a verdict on this brand in a place the brain cannot see, and it is bad.**

One comment in 1,322, pasted on 2025-01-13 under the ad `IMG 6`, summarizes Reddit discussion as calling Health For Moms "generally considered not legitimate and likely a scam," citing minimal coverage, trouble cancelling, and possible ACA non-compliance. It drew 14 likes and 10 replies. The brand's own context document describes its partner agencies as honest and trustworthy and its agents as "Mom BFFs." Two other commenters said a Google search for the brand turns up nothing at all.

Pull: **Tension.** The brand's account of itself and the only outside account that has ever reached its comment sections cannot both be true as stated, and the outside one arrived with fourteen people agreeing.

Question: What do people in health insurance communities say about this brand when nobody from the brand is in the thread?

Why it matters: if the outside verdict is as harsh as the one fragment suggests, then the legitimacy objection the brand already knows it has is being decided somewhere other than its ads, and creative alone will not move it. If the verdict is thin or stale, the brand is worrying about a ghost and the real work stays in the funnel.

Territory: **Messaging.**

**2. She asked for a review inside the ad, because she had nowhere else to ask.**

"Anyone actually have this and have insight?" is the highest-liked question in the entire 1,322-comment corpus, at 15 likes on 2026-03-20. The brand never replied. Five other commenters did, and four of the five answers were negative or neutral, including one that read the brand's own website back to the thread and one that reported spam calls.

Pull: **Pattern.** The same behavior keeps showing up: someone tries to verify this offer through peers, first on Google, then in the comments, and the answers come from strangers rather than from the brand.

Question: Where does a mom actually go to check whether a health insurance offer is real before she hands over her phone number?

Why it matters: it names the step in the buyer journey where this brand is losing people, and that step sits before the form rather than inside it. If verification runs through communities and search, then showing up there is a growth lever the brand has never pulled, and no amount of creative testing substitutes for it.

Territory: **Product.**

**3. The brand may be listening to its own hook come back.**

The account's best ad puts "Health Insurance is a scam 🙄" on screen, and "scam" then appears in 45 of 1,322 comments (3.4%) across 12 ads. `voc-corpus-profile.md` already confirmed a second phrase, "make that make sense," is echo, since the brand's creative used it first. Inside a brand-controlled surface the two cannot be separated.

Pull: **Tension.** The scam cluster is either the customer's own language or the ad's language wearing the customer's clothes, and both readings currently have the same evidence behind them.

Question: How does this buyer describe health insurance in her own words when no ad has just said it for her?

Why it matters: the voice bank is being built right now, and a phrase that is really the brand's own will feel true in testing and teach the brand nothing. It also decides whether the "insurance is a scam" hook is meeting the audience where she already is or handing her an argument that recruits the people who then decline the product.

Territory: **Messaging.**

**4. The audience knows more about insurance than the creative assumes.**

103 comments across 13 ads correct the ad's use of the word "deductible," and self-identified brokers, agents, and medical billers are among them. Beyond the correction, commenters trade real technical terms with each other unprompted: guaranteed issue, medical underwriting, coinsurance, subsidy, certified application counselor. The creative is written for a mom who does not understand her plan.

Pull: **Surprise.** Given a creative built on explaining a confusing number, the volume of people who already understand the number better than the script does is not what the setup would predict.

Question: How much does the woman this brand targets already know about health insurance before an ad reaches her?

Why it matters: it decides the whole register of the creative. Talking down to a fluent audience reads as either misleading or amateur, and both cost credibility on the account's highest-spend ad. Talking up to a confused one loses her entirely. Right now nobody knows which mistake the brand is making.

Territory: **Personas.**

**5. The category's credible voice is a licensed professional, and the brand casts a frustrated mom.**

The only people in 1,322 comments who speak with authority are brokers and agents, and they show up across 13 different ads. Some correct the script. Some pitch their own book of business, 39 comments across 10 ads. Meanwhile the brand's own creator mix across the 20 ads read in `source-pulls/ad-comments.md` is almost entirely women filming themselves at home and venting about a bill.

Pull: **Pattern.** The same kind of person keeps appearing across independent ads and months as the one the thread defers to, and it is never the person the brand cast.

Question: Who does this audience treat as a credible voice on health insurance?

Why it matters: if the category's trust runs through licensed professionals rather than peers, the brand has a casting gap sitting on top of a credibility problem, and its partner agents are an on-camera asset it has never used. If trust really does run through peers, the current casting is right and the fix is accuracy rather than talent.

Territory: **Creators and talent.**

## What a session with Reddit access would add

Recording this so the next run does not start from scratch.

The pull is worth doing across several distinct communities rather than one, because a signal that crosses communities is the only kind this doc can call strong. The obvious starting points are the health insurance community itself, the personal finance and money communities where cost questions land, the parenting and mom communities where the life stage lives, the self-employed and small business communities where ICP Courtney sits, and the disability and chronic illness communities where the loudest pain in the ad comments comes from.

Five specific things to look for, in priority order. Whether "scam" is native language for this category or the brand's own hook coming back. Whether the pregnancy and pre-existing condition exclusions get discussed outside this brand's ads. What people say about Health For Moms by name, since a verdict already exists and one commenter already found it. Where community members send each other when someone asks how to get covered. And who gets deferred to in those threads, since the credible-voice question decides casting.

Until that happens, the synthesis should treat the persona picture for this brand as one source deep, mark it mixed confidence, and say so out loud rather than presenting it as settled.
