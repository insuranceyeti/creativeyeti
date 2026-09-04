---
brand: health-for-moms
doc: personas-profile
generated_on: 2026-09-04
refresh_by: 2026-10-04
sources_synced:
  - customer-reviews: 2026-09-04 — zero rows, re-verified live in this run
  - ad-account: 2026-09-04 — Meta account HealthForMoms, act 484897827497337, re-pulled live in this run
  - ad-comments: 2026-09-04 — 1,342 comments, corpus end re-pinned live in this run
  - post-purchase-surveys: 2026-09-04 — zero responses, re-verified live in this run
  - brand-reputation: 2026-09-04
  - reddit: 2026-09-03 — unreachable, no threads read
  - other-reviews: not available, no surface exists
  - voc-corpus-profile: 2026-09-03 — built on the 1,322 denominator, superseded here by 1,342
persona_count: 3
flagship_persona: pays-and-still-owes
confidence_ceiling: mixed
verified_personas: 0
companion_docs:
  - persona-voice-library: personas/persona-voice-library.md
  - lifecycle-journey-maps: personas/lifecycle-journey-maps.md
  - cross-persona-bias-notes: personas/cross-persona-bias-notes.md
knowledge_docs_read:
  - parker-system/creative-strategy-context/expertise-routing.md — the routing map for this doc type
  - parker-system/creative-strategy-context/persona-research-and-creative-strategy-process.md — identity-first doctrine, the served-versus-buyer read, the evidence ladder, the persona-versus-overlay split
  - parker-system/creative-strategy-context/emotional-delivery-and-timing.md — the canonical TEEP definition and the emotional landing state, required for the content angle maps below
  - parker-system/creative-strategy-context/advertising-to-older-audiences.md — the brand-fit modifier behind Persona 2, whose whole case is an audience aged roughly 45 and up
live_pulls_run_on: 2026-09-04. Every number marked re-pinned below came from a Parker MCP call made in this run, not carried from a sibling doc.
data_limitations:
  - This brand has no independent check on any persona signal from any surface. Customer reviews returned zero rows live today. Post-purchase surveys returned zero responses live today. Reddit is unreachable by every route including the search provider's own crawler policy. The competitor library returned zero tracked brands live today and the branch is deferred by the user. The only first-party corpus is Facebook and Instagram ad comments under the brand's own paid creative.
  - author_name and author_id are null on all 1,342 comment rows, re-verified live today. There is no way to count unique commenters, dedupe by person, or attach a name to any signal. No claim in this doc is about people. Every claim is about comments.
  - No commenter is confirmed to have bought anything. There is no purchase event in the account at all. So no persona here rests on a confirmed buyer, and none can be marked verified.
  - The corpus denominator moved. Sibling docs ran on 1,322. An offset probe at 1,340 returned exactly 2 rows today, which pins the corpus at 1,342. Counts I recomputed use 1,342. Counts carried from a sibling doc keep their 1,322 denominator and say so.
  - The brand's five stated ICPs are contaminated evidence, not ground truth. One of them, Jen, is character-for-character Parker's own Slack text, verified by exact substring match at offset 4268 in this run. The brand's Customer Language section returns zero hits for every phrase across the whole corpus.
  - The comment corpus is lopsided. Roughly 60% sits on the MOMS38 - 1 creative family and 64% was posted in March and April 2026, both carried on the 1,322 denominator. Ad spread is carried on every load-bearing count because spread survives that skew and raw count does not.
  - Lead quality is invisible. The brand's own winner definition is two gates, cost per lead then lead quality, and gate two lives with the partner agencies. Every efficiency number here clears gate one only.
  - Northbeam is not connected. All attribution is Meta-reported.
  - There is no get_current_time tool on this MCP surface. The date comes from the session clock and matches the stamp on the newest sibling docs in this build.
  - refresh_by is set 30 days out rather than the 180-day persona cadence in parker-system/system/refresh-cadence.md. Two triggers have already fired: the corpus grew by 20 rows in a single day, and the prompt calls this the most volatile of the three one-pagers.
---

# Personas — Health For Moms

## How to read this doc

Read this sentence before you read anything else, because it governs every claim below.

**Nothing in this document is about a customer. Everything in it is about a comment.**

Health For Moms has no customer reviews. It has no post-purchase surveys. Both returned zero live today, checked through the Parker tools rather than trusted from a note. Reddit cannot be reached by any route, and the refusal names the search provider's own crawler rather than this session, so it is a standing wall and not a glitch. No competitor brands are tracked, so there is no category baseline either. The one place a real person's words exist for this brand is 1,342 Facebook and Instagram ad comments sitting directly underneath the brand's own paid ads. I re-pinned that number myself today: an offset probe at 1,340 returned exactly 2 rows, and the sibling docs' figure of 1,322 is now behind.

On every one of those 1,342 rows, `author_name` is null. I confirmed it again in this run. That means nobody can count how many people are in this corpus, nobody can tell whether one woman posted five times, and nobody can attach a name to a single signal. So the honest unit here is the comment, never the person.

**The sentence to use downstream is "commenters under the brand's paid ads said." Never "customers said."** If you find yourself writing the second one, you have quietly promoted a comment into a buyer, and the whole persona system inherits the error.

Two more things follow from that, and they are structural rather than cautious.

**Every persona in this doc is capped at mixed confidence, and none of them can ever be verified on the evidence that exists today.** This is not hedging. The persona method ranks customer evidence strongest first: post-purchase surveys, then first-party reviews, then order data, then retail reviews, then community comments, then category signal. Health For Moms holds rung five of six, and only rung five. The rule that earns a claim the word *verified* is agreement across several kinds of source, and this brand has exactly one kind. Recurrence inside one noisy source is still one source. A phrase appearing 207 times does not become verified by repeating; it becomes a well-counted single-source signal. Nothing below is marked strong or verified about an identity, no matter how big the count is.

**The brand's own list of five customers cannot be used as a check.** One of the five, Jen, is word for word a paragraph Parker itself wrote in a Slack message on 2026-09-03, which the brand then adopted into its context document. I verified that in this run by exact substring match, and it sits at character offset 4268. The brand's Customer Language section, the part of the document that reads like a record of how customers talk, returns zero hits for every single phrase across all 1,342 comments. So the stated ICP list is contaminated evidence. It is a useful record of what the team believes and a worthless check on whether the team is right. The bias section below handles this properly.

What this doc still does well, despite all of that: a public comment section is a genuinely good place to read who shows up and what stops them. People come under an insurance ad to argue, to correct, to warn strangers, and to be seen agreeing. That selection bias would wreck a read of what customers love. It is close to ideal for reading doubt, grievance, and who the algorithm actually found. So the personas below are honest reads of a real and rich surface, held at the confidence that surface can carry.

Three personas are named. That is a small set on purpose. Where the evidence does not support a fourth, this doc names the gap instead of inventing someone to fill the slot.

## Cross-persona bias notes

This section comes before the personas because a reader who skips it will misuse everything after it. The full treatment lives in `personas/cross-persona-bias-notes.md`; what follows is the part that changes how the personas themselves should be read.

### The brand is quoting itself back as its customer

The brand context document has a section called Customer Language, laid out as quotes with customers speaking. Every phrase in it was run as a substring search against the whole corpus. **Every one returns either zero hits or a single hit that turns out to be someone else talking about something else.**

The document also gives itself away in four places. It calls the same lines "the brand's own articulation," "the outcome language the brand cultivates (and that customers ideally echo)," and "the brand's own language for the end-state" in one section, then lists them under a customer heading in another. "I finally understand my insurance," "My family is covered, no matter what," "I made a smart choice," and "No more worrying every time my kid gets sick" all return zero across 1,342.

This matters most for the writer who trusts a heading. That section is the single most likely thing in the whole brand document for someone to lift as customer voice, and it is the least supported thing in it. Treat all of Section 4 as unverified brand copy until a first-party source says otherwise.

### One of the five stated ICPs is Parker's own text

Jen, "The Family Safety Net," is four sentences long. The other four stated ICPs run several hundred words each, with a city, a spouse, an age, a job, and a dollar figure. Jen has none of that.

The reason is now known. On 2026-09-03 at 21:07 UTC, Parker wrote a message in the brand's Slack channel proposing three ICP buckets after reading the brand guidelines. Its Bucket 2 read: "Married mom, kids ranging from toddler to teen. She's the one who reads the EOB statements, books all the appointments, and worries about what happens if something goes wrong. She wants to know her family is actually protected, not just technically enrolled. Responds strongly to the 'real coverage that actually pays when it matters' message."

The brand context document's Jen entry is the same text with the opening sentence removed. I checked it as an exact substring match rather than by eye, and it matched, at offset 4268. **Verified** in this run.

The consequence is precise. Any downstream doc treating the five ICPs as five independent things the brand knows is counting this one twice, because it is the brand agreeing with a machine's read of its own guidelines. It is not a fifth data point. It is an echo with an extra turn in it. And because persona routes everything downstream, this is the highest-stakes echo in the whole build.

### The loudest voices in the corpus are mostly not buyers

Four groups take up a large share of the comment volume and none of them is a lost sale.

Rival agents pitching a competing offer under the brand's own paid creative: 39 comments across 10 ads, carried on 1,322. One operator posted the same script at least nine times under the account's highest-spend ad on a single day.

People arguing the category should be abandoned entirely: 33 comments across 10 ads, carried on 1,322. She will never buy insurance from anyone.

People routing the complaint to a political cause: 54 comments across 14 ads, carried on 1,322, and they carry some of the highest like counts in the corpus. This is reaction, not persona signal.

People correcting the ad's vocabulary: 103 comments across 13 ads, carried on 1,322, including self-identified brokers, agents and medical billers. This is a credibility problem sitting on the account's biggest ad, and it is a real read on how much this audience already knows, but it is not an audience to target.

Together that is a large fraction of the noise. None of it became a persona below, and the count of any theme should be read knowing these four are in the denominator.

### Where the loudest pain belongs to someone the product cannot serve

The most emotionally intense comments in the corpus come from families with cancer, multiple sclerosis, autoimmune disease, a child in the neonatal unit, and prescriptions running thousands of dollars per fill. The plans are medically underwritten, and 55 comments across 17 ads, carried on 1,322, say the screen turned them away. The pregnancy exclusion runs wider still: 42 comments across 15 ads over fourteen months, and nine of those open by quoting the brand's own name back at it.

The persona method says volume and emotional intensity are two separate rankings that must not be flattened. Here they point at two different people, and the intense one is ineligible. So neither the chronic-condition family nor the expecting mother is written up as a persona below, because **a persona requires a buyer** and the product cannot sell to either. They appear instead as a named cost in the diagnosis. Promoting them would produce creative aimed at people the funnel rejects in public, using the brand's own name as the punchline.

### What the brand echo picture looks like in the other direction

Worth saying, because it is the one genuinely good finding here. The language actually carrying the account is not echo. It runs the healthy way. The word "scam" appears in customer comments under this brand's ads from 2025-01-13, fourteen months before the earliest ad carrying that hook launched on 2026-03-10. The deductible complaint appears in a customer's own arithmetic on 2025-11-28, months before the tweet-overlay ad. The brand took the customer's word, not the reverse.

So the shape is: the ads listen, and the written record talks to itself. Both halves matter downstream.

## Served-versus-actual diagnosis

This is the center of the document. It is built in the order the method requires: who the creative serves first, then who shows up, then the gap.

### Who the creative serves

Read from the creative itself and from Meta delivery, never from ad names.

The account's money goes to one woman. The top spending ad group, `Moms43 - 4 - V3`, opens on a mother and an infant in white bedding in soft beige light with an acoustic track, no dialogue, and a text block reading "POV: Telling your husband you found better health insurance, saved $400 a month, AND the deductible is zero. Wife of the year energy. 💕" There is a husband to report the win to. There is a household budget she controls. There are small children in a calm, clean, well-lit house. The reward on offer is not relief from fear. It is credit.

That family and its siblings carried 67.8% of the trailing quarter's spend and 72% of its leads. Parker's own emotion tag on the lead ad is Pride. Re-pinned live today, the POV format across its lifetime holds $121,820.19 of spend on 84 tagged ads and delivers 45.2% of that money to women aged 25 to 34 and 40.9% to 35 to 44.

Not one of the thirteen scripts read at full media depth in `source-pulls/ad-account.md` asks whether the viewer has insurance. Every one assumes she does and reframes it as a bad deal. So the served buyer is an insured, partnered mother of small children who can be persuaded she is overpaying. The insured part is verified from the scripts. The partnered part is inferred from the creative and is mine to own, because Meta reports age, gender, platform and device, and does not report marital status.

### Who shows up

Three things about the comment corpus contradict that picture, and each was re-checked live in this run.

**She is not uninsured, and she is not close.** The word "uninsured" appears in **2 of 1,342 comments, or 0.15%**, re-pinned live today. The word "deductible" appears in **207 of 1,342, or 15.4%**, also re-pinned live. She is not a woman without coverage. She is a woman with coverage that does not do anything.

**She answers the ad's number with a bigger one.** The string "mine is" appears in **82 of 1,342 comments, or 6.1%**, re-pinned live today. An upstream pass read all 82 in full: 76 post a specific dollar figure for their own plan, and **64 of those 76, or 84%, name a number higher than the $6,000 the ad states.** The behavior is not a quirk of that one creative either. On 2025-07-28, under a different ad naming a $600 premium, someone wrote "600? Try 1000+, then this ad would be more realistic."

**A recurring group says she cannot act at all.** She does not choose her plan; her employer does. "nope. My job picks the plan that they offer," 2026-03-30. "Mine is $6k per person too but since it's thru my job I don't really have a choice," 2026-03-17. "Mine is $9,200/individual, $17,500/family and that's the only plan my employer offers 😬," 2026-03-27. The ad's entire premise is that she can switch.

### The gap, named plainly

**The dominant commenter is not the uninsured shopper the creative addresses. She already has insurance and is still broke.**

That is the first half of the diagnosis and it is the one that reroutes the most work. The creative sells a rescue to someone who does not need rescuing; she needs an escape from something she is already paying for. The two are different scripts, different proof, and different objections.

The second half is stranger and it is the finding with the most money attached.

**The account serves two women, not one, and nobody chose that.**

Warm aspirational openers and grievance openers deliver to meaningfully different ages, on the same offer, behind the same state list. The whole variable is the first ten seconds. Ads that open on a warm montage put 7% to 12% of their spend on women 45 and over. Ads that open on a distressed face and a screenshot of a stranger's complaint put 30% to 38% there. That split was confirmed across nine separate per-ad delivery breakdowns upstream, which is why it survives as a pattern rather than a quirk.

I tested the same thing a second way in this run, through format rather than opener, and it reproduces. Re-pinned live today, in the trailing 90-day window:

| Format, 90 days to 2026-09-03 | Spend | 45-54 share | 55-64 share | 45+ share |
|---|---|---|---|---|
| Skit | $712.20 | **34.8%** | 12.4% | **48.2%** |
| POV | $70,598.29 | **9.4%** | 1.7% | **11.5%** |

And across the account's whole life, where the denominators are far heavier:

| Format, lifetime | Spend | 45-54 share | 55-64 share | 45+ share |
|---|---|---|---|---|
| Skit | $32,935.04 | 23.9% | 6.8% | **31.5%** |
| POV | $121,820.19 | 8.6% | 1.6% | **10.6%** |

Read those two tables together, because the honest version needs both. The 90-day Skit figure of 34.8% sits on only $712.20 of spend, which is far too little to lean on by itself. The lifetime cut is the trustworthy one, and it still shows Skit delivering roughly three times the share of women over 45 that POV does, on $32,935.04. So the direction is solid and the sharpest single number is not. **Format acts as an unintended age lever**, and the size of the lever is somewhere around three times, not the four and a half times the thin 90-day cut suggests.

She is also, by a wide margin, the most attentive audience the account has. Hold rate on the aspirational POV family runs 2.4% to 4.3%. On the grievance ads it runs 7.6% to 17.1%, and the skit family reaches 24.48%, the highest in the account's history. The craft bar for hold rate is 12% and up. **The account's biggest spender fails that bar at 3.28%, re-pinned live today, and the creative that clears it is watched three to five times longer and gets a fifth of the money.**

So the diagnosis, in one line a strategist can carry:

**The account spends two thirds of its budget on a warm aspirational picture that reaches a younger woman who does not watch it, while a grievance register that reaches a meaningfully older woman holds her three to five times longer, costs more per lead, and has never had a single ad built for her on purpose.**

That diagnosis disqualifies things, which is the test. It disqualifies more variations of the bedroom montage. It disqualifies pregnancy creative. It disqualifies any brief that assumes the viewer has no coverage. And it does not greenlight everything, because it says nothing in favor of the chronic-condition lane or the expecting mother, both of which the product cannot serve.

One caution the method demands and I am applying. A gap in a comment section is not proof of a gap in the buyer base. There is no actual-buyer source anywhere to check this against. Every line above is a hypothesis with real evidence under it, not a settled finding, and the thing that would settle it is named in the open loops.

## Framework architecture

The shared vocabulary the companion docs must reuse. Full definitions sit in the libraries near the end of this doc; this is the map.

- **Identity slugs** — the three durable personas: `pays-and-still-owes`, `already-knows`, `built-it-herself`. Fixed in each persona's name and identity block below.
- **Behavioral-signal slugs** — the ten rotating situational states, fixed in the persona signal blocks and collected in the behavioral overlays library.
- **Entry-door triggers** — the moments that move a persona from passive to active.
- **Identity overlays** — stable labels that sit on a persona without becoming one.
- **Voices** — who can persuade in a way the brand cannot.
- **Message signals** — the canonical angle names the creative team compares across personas.

The rule that keeps this coherent: a persona is who she still is in five years. A behavioral signal is what is true this month. If a thing you want to name would stop describing her once a situation passed, it belongs in the signal block, not in the persona list.

## Persona reference matrix

| | Persona 1 `pays-and-still-owes` | Persona 2 `already-knows` | Persona 3 `built-it-herself` |
|---|---|---|---|
| **Standing** | Flagship | Secondary | Emerging |
| **The one line** | She pays every month and still owes everything | She has managed this for twenty years and the ad talks down to her | She works for herself and every dollar already has a job |
| **Identity driver** | Duty betrayed | Earned knowledge, unacknowledged | Control over a life she built |
| **Age, inferred** | Roughly 28 to 44 | Roughly 45 to 60 | Roughly 32 to 45 |
| **Strongest evidence** | "deductible" 207 of 1,342 against "uninsured" at 2; 82 rows post their own figure, 84% above the ad's number | Format age lever: Skit delivers 31.5% of lifetime spend to 45+, POV 10.6%; hold rate 7.6-24.5% against 2.4-4.3% | Matches a stated ICP and has independent comment corroboration |
| **Volume rank** | 1 | 2 | 3 |
| **Emotional intensity rank** | 2 | 1 | 3 |
| **Confidence** | **mixed** | **mixed** | **thin** |
| **Share of spend today** | Roughly 68% through the spousal-win family | Roughly 19% through the grievance family, none of it built for her | Roughly 0.25% of lifetime |
| **Has creative built for her** | Yes, and aimed at the wrong premise | **No** | Barely |

Volume and emotional intensity are ranked separately on purpose, because they do not agree. Persona 1 is the biggest by comment volume. Persona 2 is the most engaged by a wide margin and the most likely to carry advocacy and message testing. Flattening those two rankings into one would hide the whole diagnosis.

---

## Persona 1: The One Who Pays and Still Owes — flagship

`pays-and-still-owes`

### Identity

**Core identities, the durable self-conceptions.**

**She is the one in her household who handles the insurance.** Not a role she chose, and one she will still hold in five years. She is the one who reads the statement, books the appointment, knows which card is in the folder. The corpus shows her doing it for people beyond herself: "With income restrictions? Also I'm a mom but I carry the insurance for my whole family, including dad. Can he get on this magical plan?" from 2026-04-23. Sixteen comments across 12 ads ask about a husband, a son or an ex, carried on 1,322, and they are mostly asked by women on behalf of a man. `inferred`, from the shape of who is asking on whose behalf.

**She is a payer, and being a payer is part of how she sees herself.** This is the load-bearing identity and it is the one the creative gets wrong. She is not a person who fell through a gap. She is a person who did the responsible thing, month after month, and got nothing back for it. The evidence is a contrast rather than a count: "uninsured" appears in 2 of 1,342 comments and "deductible" in 207, both re-pinned live today. One comment says the whole identity in nine words: "Why we have insurance and still have a damn bill when we go to the doctor," 2026-04-15. `inferred` on the identity, `verified` on the two counts underneath it.

**She keeps score, and she knows her number to the dollar.** Not a mood, a habit. 82 of 1,342 comments open with "mine is," and 76 of those name a specific figure. She does not say "my deductible is high." She says "$11,000." That precision is a durable trait and it tells you she has already done the arithmetic the ad is about to do for her.

**Contextual identities**, surfacing only under a named condition. Under the condition of a bill she cannot pay, she becomes an advocate who fights the carrier on the phone for hours. Under the condition of a stranger asking in the thread, she becomes a teacher: on 2026-05-05 a commenter explained to another commenter that "if it's an employer insurance, you don't have to sign up with that employer insurance you can decline the coverage and go out and find your own insurance carrier." The brand never says that sentence. A customer did.

**Outward versus real.** The gap here is sharp and it is the closest thing this brand has to the cashmere problem. Publicly she performs competence. The brand's own creative sells her the moment she gets to tell her husband she fixed it, and that phrase carries roughly 68% of the spend. In the corpus, the literal string "wife of the year" appears in **0 of 1,342 comments**. Not one person has ever said it back. What she actually posts under those ads is her own deductible, in dollars, unprompted, and sometimes an apology-free admission that she is losing: "I still pay full price for everything all year until I pay $6k which has been never." The outward self is the woman who has it handled. The purchase self is the woman keeping a number she is ashamed of. `inferred`, and the zero count is the evidence.

### Behavioral signals (currently observed)

Five rotating states. Each can attach to another persona too; what is captured here is how *this* persona expresses it.

**`found-out-the-number`** — She has just learned or re-learned what her plan actually costs her, and she is processing it rather than shopping. 82 of 1,342 comments post a figure unprompted, across 8 distinct ad names. **Implication:** she answers a number with a number. Leading with a specific figure invites her to top it and quietly disqualify the offer as unrealistic.

**`employer-plan-locked`** — Her coverage comes through a job, hers or her husband's, and she believes she has no choice. 24 comments contain "employer" and 7 contain "my job", both carried on 1,322. This is the most durable signal in the corpus: it keeps appearing from March through August while nearly everything else went quiet after May. **Implication:** she is reachable by the ad and unreachable by the offer until someone tells her declining employer coverage is allowed. That is one sentence and no ad in the account says it. **This is the highest commercial value item in the whole doc, and it is deliberately filed here as a state rather than promoted to a persona.** The whitespace audit called her the account's highest-value persona. I disagree on the label and agree on the money. Being locked into an employer plan is a situation that ends when she changes jobs, so it fails the durability test the prompt sets. The two statics built for it returned 2,580 leads at an $11.96 cost per lead lifetime, the cheapest at real scale in the account's history, and neither has run in months.

**`deductible-reset-dread`** — A calendar state that fires in December and January. "And then it's the end of the year, and we start all over. I literally hate NYE for this reason!" 2026-04-04, 6 likes. Roughly 5 comments carry it. **Implication:** seasonal by nature, and a corpus that is 64% March and April almost certainly undercounts it.

**`phone-number-guarding`** — She treats her contact details as an asset under siege. 15 comments across 10 ads, carried on 1,322, and the sharpest drew 33 likes, third highest in the corpus: "Filled it out and have been getting calls everyday from all sorts of companies which are mostly India based... This is the ONLY form I've filled out since getting my new phone number 3 months ago so it came from this site!" She had already changed her number once to escape calls. **Implication:** this sits closest to the click of any objection in the corpus, and the only thing the ad asks her to give is the exact thing she is guarding.

**`post-form-burn`** — She already went through the funnel and is now warning strangers under live creative. The shape changed over time: in 2025 it is a report from someone who did it, and by 2026 it is fear from someone who has not. **Implication:** the brand's negative word of mouth is running inside the media it pays for.

### Voice signature

Clipped, numeric, and sardonic. She leads with a figure and ends with a shrug. "Lucky! Mine is $11,000." "6k....try 13k!" "Total. Scam." "Cuz this makes sense." She uses the category's real vocabulary without explaining it, and she does not soften.

The emotion that most often moves her is not fear and it is not hope. It is **indignation at having been dutiful for nothing**. The full quote bank lives in `personas/persona-voice-library.md` under `pays-and-still-owes`; do not rebuild it here.

### Day-in-the-life

Held loosely and marked `inferred`, because this corpus supports a situation far better than it supports a day. What the comments actually show is a woman typing under an ad on a phone at a moment of grievance, not a woman narrating a routine. Delivery is 99.5% mobile in the trailing quarter, re-pinned live. Beyond that, a detailed daily narrative would be padding, and padding a persona with unbacked detail invites false confidence. Named as a gap rather than written.

### What activates purchase

**The revealed trigger pattern.** She is not shopping. She is grieving a bill and looking for someone to agree with her. The clearest single evidence is what the comment section did with the ad's own number: it treated $6,000 as an opening bid rather than a pain point. Reading that through the TEEP model in `emotional-delivery-and-timing.md`, she is sitting hard in **Trigger**, the phase where a need has just become conscious and she is still making sense of it. Nearly every funded script is written for **Evaluation**, where a specific plan is being compared. That mismatch is visible in the behavior itself: she answers the ad's number instead of the ad's offer.

**Stated versus revealed.** The stated reason, from the brand's own document, is that she wants to save money and get peace of mind. The revealed reason is that she wants the arrangement named out loud as unfair before anyone sells her anything. The load-bearing side for marketing is the revealed one, and there is a piece of account evidence for it: the only ad in the account that opens by voicing her hesitation rather than correcting her, `moms-63 3e` with "I almost scrolled past this because I thought, 'I already have health insurance, this doesn't apply to me,'" ran a $15.46 cost per lead against a roughly $22.63 account average. One ad is not proof. It is the best single piece of evidence in this doc that naming the hesitation beats adding pressure, which is exactly what the emotional-delivery method predicts for Evaluation.

**Friction at the close.** The phone number. Not price, which the ad never names. She wants to see something before she hands over the thing she is guarding: "Just give some pricing without making people sign up 🙄," 3 likes. "Really wish you could see plans without adding all your personal information to get even more telemarketing calls than we already do."

### What we believe vs what we observed

**High-confidence claims, appearing across three or more source types.** There are none, and the blank is the finding. This brand has one source type. Recording the blank so no later pass writes a number into it.

**Single-source claims that need corroboration, with the source named.** All of them, and all from ad comments. That she is insured rather than uninsured, on 207 against 2. That she posts her own figure, on 82 of 1,342. That she guards her phone number, on 15 comments across 10 ads. That she is locked into an employer plan, on 24 comments containing "employer."

**Team assumptions the data does not support.** Three, and each is checkable.

The team believes she says "I wish I'd known about this sooner" and "My friend told me about this and I'm so glad she did." Both return zero. The word "wish" appears in 4 comments and never in that form; "friend" appears in 3 and never as a referral to this brand.

The team believes timing is a main objection, naming "I should just wait for open enrollment" as one of five. The phrase "open enrollment" appears in **1 of 1,342 comments**, and "enrollment" in any form in 2.

The team's biggest creative bet is "Wife of the year energy," carrying roughly 68% of spend. It appears in **0 of 1,342 comments**. That is not echo and it is not organic. It is a phrase the brand has paid to say millions of times that nobody has ever said back.

### Awareness and market sophistication

**Awareness: Problem Aware, arriving at Solution Aware.** She knows the problem intimately and knows solutions exist; what she does not know is whether this one is real. Parker's own tags put 60.9% of lifetime spend on Problem Aware and 28.6% on Solution Aware, re-pinned live today, with 0.1% at Most Aware and essentially nothing Unaware. That matches her.

**Sophistication: high, and higher than the creative assumes.** This is the sharpest read in the section. She is not confused about insurance. 103 comments across 13 ads, carried on 1,322, correct the ad's use of the word "deductible," and self-identified brokers, agents and medical billers are among them. Commenters trade guaranteed issue, medical underwriting, coinsurance, subsidy and certified application counselor without explaining any of them. Explaining the category to this audience would be doing the wrong thing well. What she rewards instead is a specific receipt, because in a category where every brand claims savings, precision is the only thing that separates them.

### Message signals, frequency-ranked

Ranked by how often the underlying idea recurs in her own language, not by how much the brand spends on it. The inversion is the point.

1. **`paying-twice`** — she pays a premium and still owes everything. The most recurrent idea in the corpus by a distance, underneath the 207 deductible mentions and the 82 self-disclosures.
2. **`not-allowed-to-leave`** — she does not know she can decline an employer plan. Most durable signal across months; carries the cheapest leads in the account's history.
3. **`what-happens-to-my-number`** — the highest-liked objection near the click.
4. **`say-it-right`** — she wants the terms used correctly, and hands the brand better vocabulary than it uses.
5. **`the-win-i-get-to-report`** — the brand's biggest bet, ranked last, with zero uptake in her language.

The brand over-indexes on number five and under-indexes on numbers one and two. That is the message-level version of the whole diagnosis.

### T-E-E-P content angle map

Reasoned through `emotional-delivery-and-timing.md`. The point is what kind of work each phase needs, not a list of ads.

**Trigger.** This is where she actually is, and the account has almost nothing built for it. The work is to mirror her internal state back with precision before introducing anything. That means naming the experience rather than the figure, because a figure invites her to top it. Low intensity, honest, no pressure.

**Exploration.** She is comparing, and the cognitive work is differentiation. What lands is the brand's point of view and the emotional texture of being a customer, not features. The account has essentially nothing here, and this is the quiet, empathetic register the emotional-delivery method says most brands underinvest in.

**Evaluation.** She is resolving one specific objection, and it is the phone number. The work is naming that hesitation out loud rather than over-explaining the offer. The one ad doing this runs the cheapest funded cost per lead in the account.

**Purchase.** Subtract rather than add. She has decided; the job is a clear path and no new claims. The state list already does this work as a qualifier.

### Attribution

**Sources that contributed evidence.** Ad comments, 2026-09-04, 1,342 rows, the whole corpus. Ad account creative and delivery, 2026-09-04, re-pulled live. Brand context document, 2026-09-04, read as stated input and treated as contaminated where the bias notes say so.

**Sources available but unused.** None were available and skipped. Customer reviews, post-purchase surveys, other reviews, Reddit and competitor libraries are all empty or unreachable, each re-verified live where a tool exists to check it.

**The meaningful absence.** There is no surface anywhere in which a confirmed Health For Moms customer both states a reason and reveals a behavior. That is not a thin signal. It does not exist.

**Confidence: mixed.** Earned by count and by ad spread inside one source. Capped below verified because that mark requires agreement across source types and this brand has one.

---

## Persona 2: The Woman Who Already Knows — secondary

`already-knows`

### Identity

She is the finding this build almost missed, and she is the reason the diagnosis says two women rather than one.

**Core identities.**

**She has been managing this problem for a long time and she is good at it.** Her knowledge is earned rather than researched. She is the woman who has watched a deductible climb across a decade and can tell you what it used to be. "OK, this is great for mom's of young children. What about the rest of us? ... What about those of us whose children are grown and moved out of the house now? My deductible used to be reasonable, now it's almost $7000 a year," 2026-04-26, 2 likes. `inferred` on the identity, from the shape of the question and from delivery data.

**She is still a mother, and she suspects the brand has stopped counting her.** This is the identity injury and it is specific to this brand's name. Sixteen comments across 7 ads, carried on 1,322, ask politely whether she still qualifies. "What if your kids are over 18, do I still qualify as a Mom?" 2026-04-29. "What if I'm a mom, but my son is in college 🤔 i pay more $ to take care of him now than ever before ijs," 2026-03-28. The tone is the tell. She is not complaining. She is asking, and nobody answers on the thread.

**She is done being talked down to.** She is the layer of the audience that corrects the ad's vocabulary, and she does it because she knows better, not to be difficult. Reading this through `advertising-to-older-audiences.md`, the mindset is "just tell me what it does and whether it works," and cleverness reads as noise rather than craft.

**Contextual identity.** Under the condition of a stranger asking for help in the thread, she becomes the credentialed guard. "Quick tip for anyone with private health insurance. Ask about ancillary products... From a former insurance agent who is only offering advice since I am no longer selling," 2026-04-13. She is not a failed buyer. Several say plainly they would never buy. They are there because somebody should say something.

**Outward versus real.** She presents as patient and asks her eligibility question politely. What her behavior reveals is that she is the most engaged person in the audience by a wide margin, watching three to five times longer than anyone the account is actually courting. The politeness reads as low interest. The watch time says the opposite.

### Behavioral signals (currently observed)

**`aged-past-the-word-mom`** — She has concluded the brand's central word no longer includes her. 16 comments across 7 ads, carried on 1,322. **Implication:** the word "mom" is doing two jobs. The brand means it as an identity and she hears it as an eligibility rule. One sentence would fix it and no ad says it.

**`deductible-climbed-with-age`** — Her costs got worse as she got older, which is the opposite of the arc the aspirational creative implies. **Implication:** she is often healthy enough to pass underwriting and expensive enough to care, which makes her closer to the product's real buyer than a 28-year-old with a newborn.

**`found-out-the-number`** — Shared with Persona 1, expressed differently. Persona 1 posts the figure as a shock. She posts it as evidence in an argument she has been having for years.

**`enrollment-lockout`** — She wants to act and is told to wait. "Does this work in Louisiana? Because they wouldnt let me apply for good insurance here until November," 2026-05-27.

**`procedure-on-the-calendar`** — The highest-intent state in the corpus and the one the product can least serve. "how can I get that because I pay $1000 a month for my insurance and tomorrow I have surgery," 2026-05-04. **Implication:** the moment she is most motivated is the moment no plan can start in time, and no creative speaks to the window before it.

### Voice signature

Longer sentences than Persona 1, and more complete ones. She explains rather than snaps. She uses correct terms and expects them back. When she is annoyed she says so once and moves on rather than escalating. The full bank sits in `personas/persona-voice-library.md` under `already-knows`.

The emotion that most often moves her is **being taken seriously**. Per `advertising-to-older-audiences.md` the levers that work on this group are trust, reassurance, and identification through an explicit callout that tells her the ad is for her. Subtlety underperforms here; she needs to be told plainly that she is included.

### Day-in-the-life

Named as a gap, same as Persona 1 and for the same reason. Delivery data gives her age band and her platform. It does not give her a day, and inventing one would be padding.

One real thing the data does say: she is heavily on Facebook rather than Instagram. The skit family that reaches her delivered 87.7% of its trailing-quarter spend to Facebook, re-pinned live today, against roughly 60% for the account overall.

### What activates purchase

**The revealed trigger pattern.** She activates on recognition, not on a number. The only creative in the entire corpus that earns agreement instead of argument is the `MOMS38 - 2` skit family, where one woman plays both a frustrated mom and an insurance rep denying a claim because it happened "in a different hallway." Nearly every one of the roughly 12 clear recognitions in the corpus sits there. "'It's out of network' 'But it's in the same building!' 'In a different hallway' 🤣🤣🤣🤣🤣 whoever came up with this ad deserves a raise!! Love this!" 2026-04-03. "TRUTH! A SAD TRUTH." "Had a similar conversation recently with my soon to be former insurance company."

That is a different emotional doorway from the deductible figure. The skit lets her laugh, which is low intensity and positive, and per the emotional-delivery method that is exactly the quadrant that builds identification and the one most brands underinvest in.

**Stated versus revealed.** Nothing is stated, because the brand has never named her. The revealed pattern is that she rewards an experience she has lived over a number she can dispute. The load-bearing side is the revealed one by default.

**Friction at the close.** She assumes she is not eligible and stops before the form. That is a cheaper problem to fix than any of Persona 1's, because it is a line of copy rather than a trust rebuild.

### What we believe vs what we observed

**High-confidence claims across three or more source types.** None. One source type exists.

**Single-source claims needing corroboration.** That she is aged out by the word "mom," on 16 comments across 7 ads. That she recognizes herself in the denial skit, on roughly 12 recognitions clustered on one family.

**The claim that is not single-source, and it is the strongest thing in this persona.** The age split does not come from comments at all. It comes from Meta delivery, which is a genuinely different instrument from the comment corpus, and it reproduces two independent ways: by opener type across nine per-ad breakdowns upstream, and by format tag in my own live pull today. That does not make it verified about a *person*, because delivery reports who was served rather than who bought. It does make it the most robust signal in this document.

**Team assumptions the data does not support.** The brand states it wants to reach "All different ages of moms with ages of kids" as a testing priority. Across 13 ads read at full media depth upstream, the children on screen are infants and toddlers with almost no exception, and no teenager appears. One ad exists led by a woman in her mid-fifties, "At 55, I don't want complicated. I want clear, trustworthy, and done." It received $34.21 and is paused.

### Awareness and market sophistication

**Awareness: Problem Aware, and long past Solution Aware on the category.** She knows the whole landscape. What she does not know is whether this specific company is real.

**Sophistication: the highest in the audience.** This is where `advertising-to-older-audiences.md` bites hardest. In a category where every brand claims savings, she rewards a credible source over a claim, and the source she trusts is an authority or something that looks like a report, not a trend. The doc's line is that "the news are their influencers." The account currently casts a frustrated peer filming herself, and the only people in 1,342 comments who speak with recognized authority are brokers and agents, several of whom are pitching against the brand.

### Message signals, frequency-ranked

1. **`a-mom-is-still-a-mom`** — say plainly that a mom is a mom whether her kid is four or twenty-four. Zero ads say it; 16 comments ask for it.
2. **`the-fight-not-the-figure`** — dramatize the denial, the phone call, the hallway. The one thing that earns agreement.
3. **`say-it-right`** — shared with Persona 1 and felt more sharply here.
4. **`paying-twice`** — shared, expressed as a long grievance rather than a shock.
5. **`the-win-i-get-to-report`** — actively wrong for her. The status reward reads as someone else's life.

### T-E-E-P content angle map

**Trigger.** She has been in Trigger for years, which makes her unusual. The work is recognition, and the account has proof it works: the skit family. Slower cuts and a longer setup are the right build, because per the older-audience method she will follow a longer story rather than bail at three seconds.

**Exploration.** The work is credibility, and the format that carries it is something that looks like a report or an authority explaining, not a trend. The brand has a compliant version of this available: its partner agents are real, licensed, and already inside the funnel.

**Evaluation.** Her objection is eligibility, not trust in the category. The work is one explicit line telling her she is included. Direct callouts pull relevance for this group; subtlety underperforms.

**Purchase.** Legibility. Big text, high contrast, one thing on screen. The value spelled out plainly rather than through urgency, because this group is value-conscious and reads hype as a reason to distrust.

### Attribution

**Sources that contributed.** Meta delivery data by opener and by format tag, 2026-09-04, re-pulled live, and this is her primary evidence. Ad comments, 2026-09-04. Ad creative read at full media depth, carried from `source-pulls/ad-account.md`.

**Sources available but unused.** None available.

**The meaningful absence, and it is a real signal.** She is almost silent in the comment corpus relative to how much she watches. Sixteen comments against a body of viewers absorbing 30% to 38% of grievance-ad spend. That may mean she watches and does not type, which would be consistent with the older-audience method's picture of an audience that follows a longer story rather than performing in a thread. It may also mean the comment corpus simply cannot see her. Either way, judging her size from comment volume alone would badly undercount her.

**Confidence: mixed.** Held here rather than lower because the delivery evidence is a second instrument and it reproduces. Held here rather than higher because delivery shows who was served, not who bought, and there is no buyer source anywhere.

---

## Persona 3: The One Who Built It Herself — emerging

`built-it-herself`

### Identity

**Core identities.**

**She works for herself, and that shapes every dollar.** Self-employment is closer to a durable identity than a situation, because it changes how she buys everything, not just insurance. The brand's own stated ICP Courtney describes her as 36, running her own business outside Denver, priced out of her husband's employer plan by an extra $480 a month, on a short-term plan she found by Googling at midnight and is about 60% sure covers anything. That is `stated` brand input and it is one of the four ICPs not contaminated by the Jen problem.

**She earns too much for help and too little to pay full price, and she experiences that as unfairness rather than hardship.** "There is no middle class on the marketplace unfortunately. You either pay next to nothing or almost all of it with no subsidy," 2025-08-09. "I don't make very much, just more than medicaid allows (which is far below poverty level)," 2025-08-03. "Well you being a teacher is why. I'm self employed and can't find anything that doesn't have at least $5k deductible," 2026-04-02, 7 likes.

**She reads everything before she talks to anyone.** The brand's own document says she "will read every FAQ on a website before she picks up the phone." The account gives her nothing to read. This is the one identity where a stated ICP and the comment evidence point at the same person, which per the method is a genuinely different and useful result from surfacing a new one.

**Outward versus real.** She presents as fine, because presenting as fine is part of running a business. What she reveals is that she is uninsured or barely insured by choice and telling herself she is young enough for it not to matter yet.

### Behavioral signals (currently observed)

**`priced-out-of-the-spouse-plan`** — Adding her to her husband's employer plan costs more than a separate plan would. `stated` by the brand, and the corpus does not independently carry it.

**`income-gap-rejection`** — She is turned away from help for earning too much and from plans for earning too little. "But if you make under 30k a year you don't qualify smh," 2026-09-01.

**`reads-before-she-calls`** — A friction state that maps badly onto a funnel with no prices and no plan details.

**`phone-number-guarding`** — Shared with Persona 1 and expressed more sharply, because a self-employed woman's phone is her business line.

Only four signals are named. The prompt's own guidance is that fewer than three usually means undercaptured; four on an emerging persona with this little evidence is honest rather than thorough.

### Voice signature

Explanatory and structural. She describes the mechanism that traps her rather than her feelings about it. She says "there is no middle class on the marketplace," not "this is unfair." Bank in `personas/persona-voice-library.md` under `built-it-herself`, and it is thin there because it is thin here.

The emotion that moves her is **wanting a number she can plan against.** Not relief, not pride. Predictability.

### Day-in-the-life

Named as a gap. What exists is the brand's stated portrait of Courtney, which is vivid and is `stated` rather than observed. Repeating it here as though the corpus produced it would launder brand input into evidence, which is exactly what the bias notes above exist to prevent.

### What activates purchase

**The revealed trigger pattern.** `inferred` and thin. The brand states her trigger is a good month or finishing her taxes, any moment that proves the business is stable enough to insure. The corpus does not corroborate that and does not contradict it.

**Stated versus revealed.** Cannot be run. There is no revealed behavior for her anywhere, because there is no buyer source and her comment volume is a handful of rows.

**Friction at the close.** She will not call before she has read, and there is nothing to read.

### What we believe vs what we observed

**High-confidence claims.** None.

**Single-source claims needing corroboration.** All of them, and the source is thinner than for the other two. The string "self employed" returns only 2 comments in the whole corpus and one of those is a rival agent's sales pitch. So there is exactly one genuine self-identification, plus a handful of adjacent comments about the income gap.

**Team assumptions the data does not support.** None found. This is the one persona where the brand's stated picture and the comment evidence agree, which is why she is named at all despite the thin count.

### Awareness and market sophistication

**Awareness: Solution Aware.** She has already shopped, already found a short-term plan, already knows the landscape.

**Sophistication: high, and specifically she knows the trap she is in.** She does not need the problem explained. She needs a comparison she can finish alone.

### Message signals, frequency-ranked

1. **`too-much-for-help-too-little-to-pay`** — the income gap named in her own words.
2. **`a-number-i-can-plan-against`** — predictability over savings.
3. **`something-to-read-before-i-call`** — the friction fix.

A hard constraint sits on message one and the brand should see it plainly. Her whole story is a comparison between two things the brand's own compliance rules forbid naming. Section 8 of the brand context document bans government and ACA references outright and puts "ACA" on a list of words never used in creative. Seventeen comments name Medicaid and fourteen name the marketplace, both carried on 1,322. Write her story without those two nouns and most of it survives: the income figure, the cliff, the plan that costs more than the house note. Write it with them and it is sharper and against the rules. That reconciliation belongs to the brand.

### T-E-E-P content angle map

**Trigger.** She is past it. Skip the problem setup.

**Exploration.** This is where she lives, and the account has nothing for her. The work is a comparison she can complete without a phone call.

**Evaluation.** Her objection is that she cannot see anything before committing her number. Naming a price range would move her more than any hook.

**Purchase.** Subtract. She has already decided by the time she calls.

### What would move this persona up

Evidence thresholds, not calendar time.

**To secondary:** ten or more distinct comments across at least three separate ad names in which a commenter self-identifies as self-employed or as sitting in the income gap. Today that stands at roughly one clean self-identification plus a handful of adjacent rows.

**To secondary on the account side instead:** a funded test of the self-employment angle at real spend clearing the brand's good band. The one static that exists returned $16.77 per lead on $1,878.04, inside the good band on a volume too thin to call.

**To anything above mixed:** impossible on current sources for the same reason as everyone else here.

### Attribution

**Sources that contributed.** Brand context document, `stated`, Section 2. Ad comments, roughly six relevant rows.

**Sources available but unused.** None available.

**The meaningful absence.** Her near-total silence in the comment corpus, against a stated ICP built around her. She may not be in this audience at all, or she may be in it and not the type to argue under an ad. Nothing available can separate those two.

**Confidence: thin.** Named because a stated ICP and independent comment evidence agree, which is worth something. Not promoted, because six rows is a candidate and never a pattern.

---

## Entry-door trigger library

The moments that move a persona from passive to active. Canonical names; companion docs must reuse them.

| Trigger | What it is | Recurrence | Which personas |
|---|---|---|---|
| `the-number-lands` | She learns or re-learns what her plan actually costs her | 82 of 1,342 post a figure | 1, 2 |
| `the-yearly-reset` | Deductible resets in December and January and the climb starts over | roughly 5 comments; seasonal, undercounted by a spring-heavy corpus | 1, 2 |
| `procedure-scheduled` | A surgery or diagnosis with a date on it | "surgery" in 6 of 1,342 | 2, 1 |
| `the-claim-fight` | A denial, or hours on the phone losing an argument | the source of nearly every recognition in the corpus | 2 |
| `benefits-change-at-home` | A rehire, an acquisition, a package "under review" | 24 comments name an employer, carried on 1,322 | 1 |
| `the-enrollment-window` | November 1 arrives, or she is told to wait for it | "open enrollment" in 1 of 1,342 | 2, 1 |
| `a-good-month` | The business feels stable enough to insure | `stated` by the brand, not corroborated | 3 |

A note on the last two. The enrollment window is the brand's stated most important date on its calendar, and it is nearly invisible in the corpus. That is a real tension and it is an open loop, not a resolved finding.

## Behavioral overlays

Situational states that cut across personas. None of these is a persona, and promoting one would be the exact failure the method warns about.

| Overlay | One line | Cuts across |
|---|---|---|
| `found-out-the-number` | Processing a figure, not shopping | 1, 2 |
| `employer-plan-locked` | Her job picks the plan and she thinks she is stuck | 1, 2 |
| `deductible-reset-dread` | Calendar dread, December and January | 1, 2 |
| `procedure-on-the-calendar` | A medical event with a date, highest intent, lowest servability | 1, 2 |
| `phone-number-guarding` | Treats her contact details as an asset under siege | 1, 2, 3 |
| `post-form-burn` | Already in the funnel, already unhappy, warning strangers | 1, 2 |
| `state-list-rejection` | Served the ad in a state the offer does not cover | 1, 2, 3 |
| `enrollment-lockout` | Wants to act and is told to wait | 1, 2 |
| `aged-past-the-word-mom` | Believes the brand's central word no longer includes her | 2 |
| `income-gap-rejection` | Earns too much for help, too little to pay full price | 3 |

`employer-plan-locked` deserves one more line because of how it was almost mislabeled. It is the most commercially valuable item in this entire document and it is not a persona. The distinction matters practically, not just tidily: treating it as a persona would aim a whole creative lane at a state that ends when she changes jobs, and it would hide that the same state sits on Persona 2 as well.

## Identity overlays

Stable labels that look like distinct identities but reduce to the same purchase behavior. Note them; do not split personas on them.

**The single mother.** The team said in Slack on 2026-09-03: "honestly single moms are fine just as long as we also use lingo about them not being broke if that makes sense." That is an overlay, not a persona. A single mother in this audience behaves like Persona 1 with a tighter budget and a sharper phone-number objection. The team's "not broke" rule is a real constraint on how the money trigger gets written and should travel with the overlay.

**The household's insurance buyer for a man.** Sixteen comments across 12 ads ask about a husband, son or ex, carried on 1,322. This is a scope attribute on Persona 1, not a new buyer.

**The industry insider.** 103 comments across 13 ads correcting the ad's vocabulary. Not an audience. A read on how sophisticated the delivered audience is, and a credibility problem sitting on the highest-spend creative.

**The chronic-condition family.** The most emotionally intense identity in the corpus and one the product screens out. Held as an overlay and explicitly **not** a persona, because a persona requires a buyer. Named in the watch list as a recruitment cost.

**The expecting or brand-new mother.** The widest and longest-running objection in the corpus, 42 comments across 15 ads over fourteen months, carried on 1,322. Also screened out. Same treatment, same reason.

## Voices that speak for the brand

Who can persuade in a way the brand cannot. Ranked by what the evidence supports, which for this brand is unusually little.

**The peer who has lived it.** The strongest evidence in the corpus. Nearly every recognition sits on the skit where a woman plays both the mom and the claims rep. Best fit for Persona 2 and for the Trigger phase.

**The licensed partner agent.** The most under-used asset the brand has. Two comments out of 1,342 report a good experience, and both praise an agent who could not help them and was thanked anyway. "Best advice I have gotten from an insurance agent! She didn't have anything that fit but pointed me in the right direction!" Both people were told no and left praise. That is unusual enough to name. It is also the only authority available that is compliant by construction, since Section 8 requires a real licensed professional for any credentialed character. Best fit for Persona 2 and the Exploration phase.

**The customer.** Currently unavailable. There is no confirmed customer voice anywhere for this brand, and the audience has already noticed: "If you are using a fake person for your testimonial, it unintentionally sends a message to people that no real actual person would say this about your service."

**The institution.** Constrained. The brand's own rules forbid government and ACA references, which removes the most obvious institutional anchor in this category.

**Voices that actively work against the brand, named so nobody casts them.** The rival agent, 39 comments across 10 ads. The self-insurer, 33 across 10. The political reactor, 54 across 14.

## Messaging signals library

Canonical angle names for cross-persona comparison. Ordered by the weight of the evidence behind them, not by current spend.

| Signal | The idea | Evidence weight | Personas | Current spend |
|---|---|---|---|---|
| `paying-twice` | She pays a premium and still owes everything | Strongest in the corpus | 1, 2 | Heavy, and framed as a number rather than an experience |
| `not-allowed-to-leave` | She can decline her employer's plan | Cheapest leads in account history at $11.96 lifetime across 2,580 leads | 1, 2 | None recent |
| `the-fight-not-the-figure` | Dramatize the denial, not the deductible | Only creative earning agreement; best hold rate in the account at 24.48% | 2 | Under 1% |
| `a-mom-is-still-a-mom` | Say the word includes her | 16 comments across 7 ads asking | 2 | Zero |
| `what-happens-to-my-number` | Name the call flood before she asks | Highest-liked objection near the click | 1, 2, 3 | Zero |
| `say-it-right` | Use the correct term | 103 comments across 13 ads correcting | 1, 2 | Zero, and running backward |
| `too-much-for-help-too-little-to-pay` | The income gap | Corroborated, thin, and compliance-constrained | 3 | 0.02% lifetime |
| `the-win-i-get-to-report` | Wife of the year energy | Zero uptake in customer language | 1, nominally | Roughly 68% |

Read the first and last rows together. The signal with the strongest evidence and the signal with the most spend are not the same signal.

## Companion-doc routing

This document is the canonical home of the identity slugs, the behavioral-signal slugs, the entry-door triggers, the identity overlays, the voices and the message signals. Companion docs reuse these names rather than inventing parallel ones.

- **Exact customer language** lives in `personas/persona-voice-library.md`, categorized by the three identity slugs and the ten behavioral-signal slugs above. Phrase banks are not rebuilt here.
- **The lifecycle and journey reads** live in `personas/lifecycle-journey-maps.md`, keyed to the entry-door triggers and the TEEP maps in each persona.
- **The full bias treatment** lives in `personas/cross-persona-bias-notes.md`. The section above is the part that changes how the personas read; the complete echo, vocal-minority and stated-versus-revealed work belongs there.
- **The measured language spine** lives in `personas/voice-of-customer/`, and note that those docs run on the 1,322 denominator while this one runs on 1,342.

## What we're watching

**New signals emerging in the recent window.** Eligibility questions and state complaints now dominate the newest comments, where March through May was raw cost grief. Of the 207 comments containing "deductible," only about 5 came after 2026-06-01. The corpus has gone quiet on pain and loud on qualification. That is a change in what the current creative invites, and it is worth watching because comments are this brand's only listening post.

**Signals fading.** The distrust of AI-presented creative. 32 comments across 7 ads, but 25 of them sit on one 2025 ad and it has been near-silent since April 2026. Do not treat it as solved without checking why it stopped.

**Identity clusters forming that fit no existing persona.** The woman leaving the category entirely. 33 comments across 10 ads, and the category feed says the same thing at enormous scale, with a former nurse explaining three years uninsured holding 872,100 plays. She is not a persona because she is not a buyer for this product. She is watched because the brand's own best hook, "Health Insurance is a scam," argues her case for her before asking her to buy insurance.

**Personas suspected to be bias artifacts, flagged for downgrade or retirement.**

*Jen, the brand's stated ICP.* Retire as evidence. She is Parker's own text, verified by exact match at offset 4268. Keep her as a record of what the team believes; never count her as an independent data point.

*The uninsured mom.* Downgrade sharply. She is a stated ICP and a real piece of creative, and she is 2 of 1,342 comments. The account gave her about 0.14% of lifetime spend, so the absence of evidence is partly an absence of testing rather than proof she does not exist. Held as a named gap rather than a persona.

*The peaceful outcome mom.* Not a persona at all, and worth saying because roughly $110,205.90 of lifetime spend sits on her. She is a mood, not a person. Across 1,342 comments there are roughly 12 clear recognitions and almost none sit on that creative. The sharpest response to it is a rejection of the footage: "I'm sure the mom that can afford matching outfits prob just pays in cash 🤦‍♀️," 2026-09-03.

**The two the product cannot serve, watched as a cost rather than an opportunity.** The chronic-condition family and the expecting mother. Both are recruited by the advertising and rejected by the funnel, in public, using the brand's name as the setup. Reaching either harder makes the problem worse.

## Open loops

**1. The account reaches an older woman it has never spoken to.**

Grievance openers deliver 30% to 38% of their spend to women 45 and over where warm openers deliver 7% to 12%, and the format cut reproduces it: Skit sends 31.5% of its lifetime spend there against POV's 10.6%. She watches three to five times longer than anyone the account courts. No ad in the library was built for her on purpose, and the one that speaks to her age directly got $34.21 before it was paused.

*Pull: Pattern.* The same split appeared independently through two different instruments, nine per-ad delivery breakdowns upstream and my own format-tag pull today, which turned a curiosity about one ad into a question about the whole account.

*Question:* What is the older woman the grievance creative keeps reaching actually coming to this offer for?

*Why it matters:* she is roughly a fifth of the spend and the most attentive audience the account has, and the deeper watch time suggests her situation differs from the young partnered mother's. If it does, she needs her own message rather than a harder version of the same one, and nobody has written it.

*Territory: Personas.*

**2. Nobody knows what the flagship persona's real ranking is, because the only outcome anyone can see is a phone number.**

Every cost-per-lead comparison in this build measures the cost of a phone number, not the cost of a customer. The account's `invitee_meeting_scheduled` conversion returned no data at all in the window and only 42 `Call` events fired against thousands of leads. The brand's own definition of a winner is two gates and Parker can only see gate one.

*Pull: Tension.* The account ranks its creative confidently on cost per lead while the one number that would say whether a cheap lead is a good lead is missing, and those two things cannot both be trusted.

*Question:* Which of the account's messages produce leads that actually book a call with an agent?

*Why it matters:* if the aspirational creative produces a curious browser and the grievance creative produces a woman in real pain who answers the phone, the persona ranking in this document inverts and roughly two thirds of the budget is behind the wrong woman. Nothing else in the persona system matters as much as this answer.

*Territory: Product.* **Routed to the brand**, because the outcome lives in the partner agencies' systems.

**3. The brand's written record of its customer and its actual customer language have nothing in common.**

Every phrase in the brand context document's Customer Language section returns zero hits across 1,342 comments. One of the five stated ICPs is Parker's own Slack text, adopted verbatim. Meanwhile the phrase carrying roughly 68% of spend, "wife of the year," appears zero times in customer language, and the phrases that do recur are ones the brand picked up from customers rather than the reverse.

*Pull: Tension.* The same document calls these lines the brand's own emotional outcomes in one section and how customers describe outcomes in another, and both cannot be true as written.

*Question:* Where did the customer quotes in the brand's Customer Language section come from?

*Why it matters:* the answer flips the value of the whole section. If those lines came from real women on sales calls or in a research session, they are the best customer evidence this brand owns and every persona above should be rebuilt with them. If a copywriter wrote them, the section is the brand talking to itself and every writer who trusts it ships the brand's marketing back at the customer as her own voice.

*Territory: Personas.* **Routed to the brand**, because only the team knows what went into that document.

**4. The word the whole brand is built on may be reading as a rule rather than an identity.**

"Insurance" appears in 284 of the corpus against "mom" at most 73, and that 73 is inflated because the string also matches "moment," both carried on 1,322. Sixteen comments across 7 ads ask whether grown children still count and 16 across 12 ask about dads. Nobody answers on the thread.

*Pull: Surprise.* For a brand named Health For Moms whose entire creative device is that one word, the audience using the category word nearly four times as often is not what the setup would predict.

*Question:* How does this audience describe who she is when she talks about buying health insurance?

*Why it matters:* it decides whether "mom" is the identity the creative should lead with or a wrapper quietly generating eligibility confusion, and that routes the naming, the casting and the callout line in every brief downstream.

*Territory: Personas.*

**5. The most attentive creative in the account is the one nobody funded.**

The denial skit holds 24.48% of viewers, double the craft floor and more than six times the current top spender's 3.28%. Nearly every recognition in the corpus sits on it. It cost $3,774.02 across three ads, against roughly $110,205.90 on the montage nobody recognizes.

*Pull: Resonance.* It is the only creative in this brand's history that made people say it was about them instead of arguing with it, and the reason it works is worth understanding before anyone scales it.

*Question:* Why does the denial skit earn agreement where the deductible complaint earns argument?

*Why it matters:* if the answer is that it names an experience she has lived rather than a number she can dispute, that reshapes the whole creative approach rather than one ad, and it gives both Persona 1 and Persona 2 a doorway the account has barely used.

*Territory: Messaging.*

---

This is everything I know about advertising to older audiences.
