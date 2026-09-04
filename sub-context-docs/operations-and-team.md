---
brand: health-for-moms
doc: operations-and-team
generated_on: 2026-09-04
refresh_by: 2026-12-04
pass_status: partial
sources:
  - "Parker chat history via search_chat_history, read live 2026-09-04. 9 threads, 8 Slack in channel C0BUQEFF70V and 1 web. Six read message by message: 1788469337.157819 the ramp-up and brand-guidelines correction, 1788473402.812619 the tooling and workflow conversation, 1788479022.847859 the comment moderation exchange, 1788480849.190169 the ban request, 1788481525.524429 the introduction of the business partner, and 1788529081.275569 the landing page headline request. This is the only direct source on the team that exists."
  - "Meta ad account HealthForMoms, act 484897827497337, via Parker MCP search_facebook_ads_sql, pulled live 2026-09-04. Two cuts: the 90-day window 2026-06-06 to 2026-09-03 grouped by ad, and a filtered cut on landing_url containing go.healthformoms. Campaign names, ad set names, ad naming, statuses, landing destinations, creation dates and delivery all read from the live pull."
  - "Parker MCP list_custom_metrics, get_available_brands and check_northbeam_connection, all run live 2026-09-04."
  - "Upstream brain docs read in full first: running-notes/missing-context.md, running-notes/brand-rules.md, running-notes/success-definition.md, running-notes/standard-sync.md, BUILD-STATUS.md, source-pulls/ad-comments.md, source-pulls/reddit.md, sub-context-docs/reputation-analysis.md."
  - "Method docs loaded before analysis per expertise-routing.md: ad-account-analysis.md, creative-strategy-by-brand-size.md, creative-strategy-fundamentals.md."
brand_intake_run: false
data_limitations:
  - "No operations intake has ever been run for this brand. running-notes/missing-context.md records that the Phase 0 intake covered the business objective, the north star and the reporting surface, and nothing about team structure, tooling, process, agencies or budget. So most of this doc is a named blank routed to the brand, which is the correct outcome for this doc type rather than a failure of the pass."
  - "Everything about the team comes from Parker chat history, which is one side of a conversation with a marketing tool. It is not an org chart, an intake form or a call. Every team claim below is brand-provided in passing, never confirmed."
  - "running-notes/missing-context.md records 4 chat threads, 1 web and 3 Slack. The live listing on 2026-09-04 returns 9, 1 web and 8 Slack. Five threads were opened after that note was written. The note is stale and this doc supersedes it on the thread count."
  - "Ad names, campaign names and ad set names are inventory handles. They can reveal how the account is organized and they cannot prove who made a piece of creative or what is in it. Every supplier read below is marked inferred for exactly that reason."
  - "Parker has read access to Facebook comments and no write access. It cannot hide, delete, reply to or ban. The team asked directly on 2026-09-03 and was told no. That is a tooling gap, recorded here rather than in the open loops."
  - "Lead quality, the second of the brand's two gates for calling an ad a winner, is invisible to every tool Parker holds. It lives with the partner agencies. Nothing in this doc or anywhere in this brain can see it."
  - "Northbeam is not connected, re-verified live 2026-09-04. All attribution is Meta-reported."
  - "There is no get_current_time tool on this MCP surface. The 2026-09-04 date comes from the session clock and matches the rest of this build."
  - "refresh_by is set 90 days out rather than the 365-day cadence in parker-system/system/refresh-cadence.md. Three triggers have already fired: a second person joined the working team on 2026-09-04, a new landing destination went live in late August and is losing most of its traffic, and Open Enrollment starts 2026-11-01."
---

# Operations and team — Health For Moms

## How this pass was built, and what it can carry

Most context docs are built from research. This one cannot be, and it is worth saying why up front so nobody reads the blanks as laziness.

Almost nothing about how a business actually runs leaves a public trace. The website will not tell you who buys the media, where the work gets stuck, or what the team wishes it could stop doing by hand. That information lives inside the company, and the way it normally reaches a doc like this is an intake conversation. **For Health For Moms that conversation has never happened.** `running-notes/missing-context.md` records that the Phase 0 intake asked about the business objective, the north star and where performance is read, and asked nothing about team, tools, process, agencies or budget.

So I did the two things that were available. First, I read every Parker conversation this team has ever had, nine threads, six of them message by message. That turned out to be a real source rather than a consolation prize, because people say true things about how they work while asking for something else. Second, I read the ad account itself as an operational artifact rather than a performance one: how the campaigns are shaped, how ads are named and duplicated, how fast new creative arrives, where the clicks are pointed, and what has been configured versus what was left on defaults.

Two disciplines govern what follows. Everything the team said is marked **brand-provided**, which means their word, quoted, not confirmed. Everything I read off the account is marked **verified** where it is a number I pulled and **inferred** where I am reasoning from how things are named or arranged. And where a stated constraint smells like a habit that has hardened rather than a real limit, I say so and mark it to probe, because mistaking one for the other quietly shrinks what the strategy will even attempt.

The single most useful thing this pass found is not about the team at all. It is a live landing destination that is losing roughly nine of every ten clicks it is paid for. That sits in the media buying section, and it is the reason this doc is worth reading today rather than at its refresh date.

---

## Team

**Two people are visible, and that is the whole roster this pass can see.**

**The primary operator.** One person runs this brand's marketing conversation with Parker. Every one of the eight Slack threads comes from the same account in the same channel, `C0BUQEFF70V`. Across those threads he does the strategy, the creative direction, the brand guidelines, the media questions and the comment moderation himself. `verified` from the thread listing, `inferred` that these are one person's threads rather than a shared account.

What he does, read off what he actually asks for rather than a title:

- He owns the brand guidelines and corrects Parker when it gets the audience wrong. On 2026-09-03 at 21:05: *"Some of those ICPs are very wrong. I'm uploading branding guidelines into your Training."* He then uploaded the document and made the call on who the customer is, including overruling the guidelines himself: *"honestly single moms are fine just as long as we also use lingo about them not being broke if that makes sense."* **brand-provided.**
- He writes and commissions copy. On 2026-09-04 at 13:38: *"can you help me write some landing page H1s for healthformoms?"* **brand-provided.**
- He does brand safety by hand. Covered in Bottlenecks below.
- He is building this brain himself, in Claude Code, over the last two days. On 2026-09-04 at 00:26: *"nothing quite yet im still setting up the claude brain so stay tuned!"* **brand-provided.**

**Wes, business partner.** Introduced on 2026-09-04 at 00:25 UTC: *"meet my biz partner Wes."* Wes's first message names what he is here for: *"oh you know, ready to make some BANGERS for healthformoms."* **brand-provided.** That is the entire evidence base on Wes. What he owns, whether he buys media, whether he is full time, and whether he was involved before yesterday are all unknown. Named blank, routed to the brand.

**The Parker workspace holds one organization and one brand.** `get_available_brands` returns organization `Insuranceyeti`, id `71367b2e-920c-46ca-81a5-51363f3c9ee4`, containing only Health For Moms. `verified`, live pull 2026-09-04. `sub-context-docs/reputation-analysis.md` establishes that the operating entity named on the brand's own terms page is Insurance Yeti LLC, Orlando FL. The GitHub repo this brain lives in is `insuranceyeti/creativeyeti`.

**Which departments use Parker: one, and it is not a department.** There is no evidence of a second Parker user, a second channel, or a marketing team beyond the two people above. On a larger team this section would map who across the organization Parker serves. Here the honest answer is that Parker serves one operator and, since yesterday, his partner. `inferred`, strong, from the thread listing.

**How the person describes his own skill level, which matters for what to recommend.** On 2026-09-03 at 22:22: *"not claude code but I really do want to become more of a agentic marketer! I use maybe just normal chat but the normal chat doesnt have updated guidelines like you have."* He is comfortable in Slack and in general chat tools, new to Claude Code, and actively trying to level up. **brand-provided.** Anything this brain recommends should assume a capable marketer who is early in the tooling, not a technical operator.

**The single-person risk, named plainly.** Strategy, brand guidelines, copy, creative direction, comment moderation and now the brain build all sit with one person. That is normal at this size and it is still a risk worth flagging, because every recommendation this brain ever makes lands on the same desk. `inferred`.

**What is not known and only the brand can answer:** whether anyone else touches the ad account day to day, who Wes is in the business, whether there are employees or contractors beyond the creative suppliers named below, and who at the partner agencies is the counterpart. All routed to the brand.

---

## Bottlenecks

The team named its own bottleneck twice inside thirty-one minutes, unprompted, on the first night of using this brain. That is as clear a signal as this doc will ever get, so it goes first and it goes in their words.

**1. Comment moderation, done by hand, one ad at a time.**

Verbatim, Slack thread 1788479022.847859, 2026-09-03 at 23:43 UTC:

> *"Do you have permissions to clean up comments or no?"*

Parker said no, it can read and analyze comments but cannot hide, delete or moderate them, and that this has to be done in Meta Business Suite. Three minutes later, at 23:46:

> *"yes please and give me all ads LIVE its on so i can go hide them"*

Then, Slack thread 1788480849.190169, 2026-09-04 at 00:14:

> *"can you find me an ad theyre on so I can ban them"*

**My read.** This is a true limit, not a habit. The corpus is 1,342 comments across 112 ad IDs and it grew by twenty in the twenty-four hours to 2026-09-04, verified in today's pull. The brand is the only party who can act on any of it, the acting has to happen ad by ad inside Meta's interface, and the person doing it is also the person doing strategy and copy. `sub-context-docs/reputation-analysis.md` establishes what fills the silence: the most-liked thing anyone has ever said about this company's service is a warning not to give it your phone number, at 33 likes.

**And one thing to probe rather than accept.** The team's whole framing is hide and ban. Nobody has ever said replying is impossible, and in twenty months and 1,342 comments the brand has never replied once. Hiding a comment that says the brand sells your number is defensible. Never answering the most-liked question in your own comment section, *"Anyone actually have this and have insight?"* at 15 likes, is a choice somebody made or a job nobody owns. Which of those it is changes what is possible here, and only the brand can settle it. Marked to probe, and it is open loop 2.

**2. Brand context does not travel to the tools he actually works in.**

Verbatim, 2026-09-03 at 22:22:

> *"I use maybe just normal chat but the normal chat doesnt have updated guidelines like you have. So maybe in code id also have to build a new skill with updated moms stuff / copy for it"*

**My read.** A true limit today with a known fix, and the fix is the thing he was already building when he said it. Worth carrying because it explains the shape of his asks: he comes to Parker for anything that needs the brand's real rules, which is why the guideline corrections and the copy requests all land here.

**3. The brain build itself was in flight and blocking.**

On 2026-09-04 at 00:26: *"nothing quite yet im still setting up the claude brain so stay tuned!"* And on 2026-09-03 at 23:32, the thread titled *"is it set up ? its still doing things but not sure if its just starting or what."* **brand-provided.** Temporary by nature, and worth recording because a first read of this brain will land on someone who spent two days waiting for it.

**4. Not stated by the team, and larger than everything above: the landing destination.**

The team has not named this and may not know it. Eleven live ads are pointing at a domain that converts at one twelfth of the account's normal rate. It is in Media buying setup below with the numbers. I am listing it under bottlenecks because it is the place where work is actually getting stuck, even though nobody has said so.

**What is not known:** creative production turnaround, approval chains, who signs off on a script before it is filmed, and how long it takes to get a new ad live. All routed to the brand.

---

## What they want automated

Captured in their terms first, because the precise ask is what a later workflow can act on.

**1. Cleaning up comments.** The most direct automation request on record, asked of Parker straight out: *"Do you have permissions to clean up comments or no?"* The follow-up sharpens it into two jobs rather than one. Hiding damaging comments on live ads, and banning rival operators from the page. **brand-provided**, 2026-09-03.

**2. Finding which live ads a damaging comment sits on.** *"yes please and give me all ads LIVE its on so i can go hide them"* and *"can you find me an ad theyre on so I can ban them."* This is a different job from moderation and Parker can already do all of it. It is the search-and-locate half, and the team is already using Parker for it. **brand-provided.**

**3. Carrying the brand's rules into whatever tool he is working in.** *"maybe in code id also have to build a new skill with updated moms stuff / copy for it."* **brand-provided.**

**4. Copy on demand, against the real guidelines.** Landing page headlines on 2026-09-04, scripts and angles on 2026-09-03. He is not asking for this to be automated so much as demonstrating that it already is, which is a signal about what he will keep coming back for.

**5. A tool he raised himself and nobody has resolved.** On 2026-09-03 at 23:05: *"Ialso have Gethookd should i hook up that to this claude code thing and we can pull from there too for inspo?"* and at 23:06: *"I know gethookd does have an MCP but just not sure what it works with."* **brand-provided.** He owns a creative inspiration tool with an MCP and does not know whether it connects. That is a small unblock with a real payoff for a two-person team, and it is still open.

**Where the ask and the leverage differ, said plainly.** The mining method and the strategy priors both warn that teams often ask to automate the symptom rather than the cause, so this is worth naming rather than just recording the request. What the team asked for is comment cleanup. What today's pull found is $3,633.54 of live spend in the last 90 days producing 20 leads at $181.68 each because of where the clicks are pointed. Both are real. The first protects trust and is genuinely a performance lever in a category where trust is the binding constraint. The second is a bigger number and it is fixable this week. A good answer does both and does the landing page first.

---

## Outside help

**No agency relationship has ever been stated by the brand. This whole section is inferred from how the account is organized, and it is marked that way on every line.**

**The partner insurance agencies. This is the most consequential outsourcing in the business and the brand has never described it here.**

The business model is a match and consult referral, not a direct sale. The brand takes a form fill and hands the person to a partner agency, and that agency owns everything that happens next. Three things make this the section's headline:

- **Every campaign in the account carries a `USHA` prefix.** All four campaigns visible in the 90-day window are `USHA - ABO - SCALE - MOMS`, `USHA - ABO - TEST - MOMS`, `USHA - CBO - OTP` and `USHA - ABO - Battle Res`. `verified` from today's pull. USHEALTH Advisors is a real health insurance sales organization that goes by USHA, and the most natural reading is that the account is organized around that partner. `inferred`, and it needs the brand to confirm because it changes who the real client of this creative is.
- **The brand's worst reputational damage originates in this handoff.** `sub-context-docs/reputation-analysis.md` documents it as the primary root cause of the negative word of mouth: people fill the form and are called by many companies they did not choose. The most-liked comment about the service, at 33 likes, is a report of daily calls from unknown numbers. Two commenters say the page made an explicit promise about not being contacted by random agents that was then broken. The brand has the least visibility and the least control over exactly the step doing the most damage.
- **Parker itself flagged this to the team and could not name the owner.** In the moderation thread on 2026-09-03: *"This is a real trust problem worth flagging to whoever manages the partner agency relationships."* Nobody in this brain knows who that is.

**Creative production. At least four distinct outside signatures appear in the account's ad names.**

The prompt's own rule is that names are inventory handles: they can reveal how an account is organized and they cannot prove who made a piece of creative or what is in it. On that basis, and marked `inferred` throughout:

- **An animation supplier.** Sixteen ads carry the token `Animation Agency`, in their own ad sets named `Animation Agency #4`, `#5` and `#6`, all created in one batch on 2026-05-06. The filtered lifetime cut reports $435.67 of spend and 8 leads at a $54.46 cost per lead across them. `verified` on the numbers and the batch date. One of them, `Animation Agency #4 - H1`, is a personified medical bill with a grumpy face standing on an insurance card, opening with *"I am your deductible."* That is a genuinely different creative capability from the rest of the account, it was tested once in May, and it has never been given real budget.
- **A named individual.** Ads named `Moms Nahuel WV#1 - V9` and `Moms Nahuel WV#2 - V3`. A first name in an ad name usually means an editor or a freelancer.
- **A second production shop.** Ads named `OMC-Health for Moms-[B3-C17-V2]`, `OMC-Health for Moms-[B3-C11-V7]` and `OMC - C11 - 2b`. The bracketed batch, concept and version pattern is a delivery convention from a vendor with its own naming system rather than the brand's.
- **A third.** `B1 samar- Copy`, the account's highest-spending ad of all time.

Four naming conventions in one account is the shape of work coming in from several places without a single standard. **The brand is producing about 49 new ads a month with two visible people, so most of that production has to be bought from outside.** Who, on what terms, and whether the brand is happy with any of them are all named blanks routed to the brand.

**Not evidenced anywhere:** a media buying agency, a creative strategy agency, a landing page or web developer, or a compliance reviewer. Their absence in the account is not proof they do not exist.

---

## Budget and spend

**No budget has ever been stated. The only spend numbers here are the ones Parker can see in the ad account, which is media spend only and not the marketing budget.**

**What is verified, from today's live pull.** The 90-day window 2026-06-06 to 2026-09-03, one Meta ad account:

- **$100,065.31 spend**, 4,358,573 impressions, 78,514 clicks, 51,299 link clicks, 42,425 landing page views
- **4,421 leads at a $22.63 cost per lead**, and **zero purchases**, which is by design because this is lead generation
- CPM $22.96, CTR 1.80%
- Delivery: 95.3% female, 42.6% aged 35 to 44 and 36.7% aged 25 to 34, 99.5% mobile, 60.3% Facebook and 39.1% Instagram, with 0.5% on Audience Network and 0.1% on Threads

**The channel split is not a split. It is one channel.** Everything runs through paid Meta. `sub-context-docs/reputation-analysis.md` establishes the same thing from the outside: no organic search presence, no press, no discoverable organic social, no retail, no marketplace. The reputational consequence is in that doc. The operational consequence belongs here, and it is that this business rents its only distribution channel and has no second surface to fall back to.

**The budget moved sharply and nobody has written down why.** `audits/2026-Q3/90-day-performance-audit.md` records that spend fell 73.5% quarter over quarter, from $374,508 to $99,267, while cost per lead held essentially flat at $22.65 against $22.64. Flat efficiency through a two-thirds spend cut reads as a budget decision rather than a performance failure. `verified` as the audit's finding, and the reason for the decision is a named blank only the brand can fill. It matters because Open Enrollment starts 2026-11-01 and the account is currently running at roughly a quarter of the spend it carried a quarter ago.

**A measurement hygiene note, because three different lifetime numbers are circulating in this brain.** Parker told the team $742,000 across 1,557 ads in Slack on 2026-09-03. `reputation-analysis.md` reports $161,685.48 and 7,451 leads from its 2026-09-04 pull. My own cut today returns $156,014.96 and 7,039 leads. These are not contradictions, they are different scopes: my figure and the reputation figure are lifetime totals for the ads matched by each query, and the $742,000 is the account's whole history. Nobody has written down the account's true all-time number in a way a later reader could trust. **The 90-day window figure is the one every read in this brain should use, and it is stated above.** `inferred` on the cause of the difference.

**What is a named blank and routed to the brand:**

- The total marketing budget, and whether media spend is all of it
- How firm the number is and who controls it, which bounds every recommendation this brain will ever make
- What creative production costs, which is real money that never appears in the media number
- Unit economics: what a lead is worth, gross margin, payback window, and a maximum tolerable cost per lead. `running-notes/brand-rules.md` already records the consequence of this gap, which is that "efficient" is currently measured against the account's own trailing cost per lead rather than against a business threshold. Without a ceiling, no read in this brain can say whether $22.63 is good.
- Whether spend is planned to rise for Open Enrollment, and by how much

**One read against the spend level, using the brand-size lens.** At roughly $33,000 a month of media this brand sits between the two lower bands in `creative-strategy-by-brand-size.md`. The plays that fit are getting shots on goal, testing messaging cheaply, and then putting budget behind what proves out. The account is already doing the first: 147 new ads in 90 days. What it is not obviously doing is the third, since those 147 new ads carry only $26,529.01 of the window's $100,065.31, so about three quarters of spend still sits on older creative. `verified` on the numbers, `inferred` on the read.

---

## Ownership

Named as clearly as the evidence allows, with the unowned seats called out because an unowned function is where strategy stalls.

**Strategy: the primary operator, working through Parker.** He sets the audience, corrects it when a tool gets it wrong, uploads the guidelines and makes the calls. `inferred`, strong, from six chat threads.

**Creative direction and copy: the primary operator, with Parker.** Concepts, angles, hooks and landing page headlines all run through him. `inferred`, strong.

**Creative production: outside, and split across at least four suppliers.** See Outside help. `inferred`.

**Media buying: unknown, and somebody is doing it daily.** The account shows a live hand at work. A new campaign, `USHA - CBO - OTP`, was stood up with eleven ads on 2026-08-17 and 2026-08-31. Ad sets are numbered up to `Moms68`. 147 ads were created in the last 90 days. Whether that hand belongs to the primary operator, to Wes, or to someone not visible in Parker is a named blank and it is the most important unanswered ownership question in this doc, because it decides whose desk a media recommendation lands on. Routed to the brand.

**Brand safety and comment moderation: the primary operator, manually, starting 2026-09-03.** `brand-provided`, and worth noting it appears to have started the day the brain was built.

**The customer conversation after the click: the partner agencies, entirely.** They own the call, the pitch, the follow-up and the phone number. This is the seat that produces the brand's worst public damage and the brand has no visibility into it. `inferred` from the business model plus the reputation evidence.

**Owned by no one, and both matter.**

- **The comment section as a conversation.** Somebody now moderates it. Nobody answers it. Zero brand replies in 1,342 comments over twenty months.
- **Lead quality reporting.** `running-notes/success-definition.md` sets a two-gate definition of a winner, cost per lead first and then lead quality before real scale. Gate two lives with the partner agencies and reaches nobody in this brain. That is not a tooling gap so much as a missing feedback loop between two organizations, and it means every scale recommendation this brain makes has to carry a caveat it cannot resolve.

---

## Media buying setup

Recorded to understand the environment the creative gets delivered into, not to redesign it. One thing in here does look like it is working against the brand, and per the prompt it is flagged for the brand and its media owner to confirm rather than resolved here.

**The account.** One Meta ad account, `HealthForMoms`, act `484897827497337`, USD, marked primary and enabled. No second account. `verified`, live 2026-09-04.

**Campaign structure.** Four campaigns carried spend in the 90-day window, all prefixed `USHA`:

| Campaign | What it appears to be |
|---|---|
| `USHA - ABO - SCALE - MOMS` | the proven creative, ad set budgets |
| `USHA - ABO - TEST - MOMS` | the testing lane, where most new concepts land |
| `USHA - ABO - Battle Res` | a smaller lane, ad set `Moms battle res ad set` |
| `USHA - CBO - OTP` | new, campaign budget, ad set `Moms CBO OTP` |

Both ad set budget and campaign budget optimization are in use at once. A clean separation of scale from test is a real discipline and the brand deserves credit for it. `verified` on the names, `inferred` on the roles.

**Naming.** Ad sets carry a concept number plus a plain-English angle label, like `Moms43 - 4 (State Moment)` and `MOMS34 - N1 - A (Mom Moment Montage)`. Ads carry the concept number and a version suffix, `- V1`, `- V3`, `- V4c`. Duplicated ads carry `- Copy`. The concept counter runs to `Moms68`. `running-notes/brand-rules.md` records that no naming convention was captured at intake and treats this as a working read. Today's pull is consistent with that read and it is still inferred, not stated.

**Production cadence.** **147 ads created in the 90 days to 2026-09-03**, about 49 a month. Those 147 carry $26,529.01 of lifetime spend and 1,306 leads at a $20.31 cost per lead, which is slightly better than the account's $22.63. `verified`. For a two-person team that is a lot of creative arriving, which is the strongest single argument that production is bought rather than made.

**One body copy runs the entire account.** All eighteen ads in the top-spend cut carry the identical headline, *"Approved by thousands of Mom's across America"*, and the identical primary text beginning *"Moms, we're not just caregivers—we're protectors of futures."* `verified`, 18 of 18. Everything is being varied except the words underneath the video. That is a process fact rather than a creative judgment, and it means the primary text has never been tested.

**Duplication resets the social proof.** Ads are duplicated into new campaigns rather than rebuilt. `moms-63 2b` and `moms-63 2b - Copy` share media hash `00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399` and ran in two campaigns at the same time. Each duplicate is a fresh post with a fresh empty comment thread. For a brand whose comment sections are hostile that is arguably an accident in its favor, and it also means engagement and any moderation work do not carry over. `verified` on the shared hash, `inferred` on the effect.

**The finding that needs attention this week: the `go.healthformoms.co` destination.**

The `USHA - CBO - OTP` campaign runs eleven ads, all ACTIVE, and every one points at `https://go.healthformoms.co/save/` rather than the `www.healthformoms.co/save/` the rest of the account uses. Filtered cut, 90-day window, `verified` live 2026-09-04:

| | `go.healthformoms.co` cut | Whole account, same window |
|---|---|---|
| Spend | $3,633.54 | $100,065.31 |
| Link clicks | 2,291 | 51,299 |
| Landing page views | **167** | 42,425 |
| Landing page views per link click | **7.3%** | **82.7%** |
| Leads | 20 | 4,421 |
| Cost per lead | **$181.68** | **$22.63** |

The cleanest proof is a matched pair, because it removes the creative from the argument entirely. `moms-63 2b` and `moms-63 2b - Copy` are the same video, same media hash, same headline, same body copy, same hook. One points at `www`, the other at `go`:

- `moms-63 2b`, `www.healthformoms.co/save/`: 3,404 link clicks, 2,981 landing page views, **417 leads at $13.26**
- `moms-63 2b - Copy`, `go.healthformoms.co/save/`: 750 link clicks, 64 landing page views, **6 leads at $160.84**

And the starkest single row: `moms-53 3 - Copy` spent $495.57 for 511 link clicks, 9 landing page views and zero recorded leads.

**The read.** Something between the click and the page is failing on that subdomain. It could be a broken redirect, a page that will not load on mobile, or a pixel that never fires so the events are real but invisible. Nine in ten clicks not arriving is not a creative problem and it is not an audience problem. `verified` on every number above. `inferred` on the cause, and deliberately not resolved here, because this is exactly the kind of thing the prompt says to flag for the brand and its media owner to confirm. It is live right now, it started with ads created 2026-08-17 and 2026-08-31, and the campaign is running into the Open Enrollment ramp.

**Measurement setup.** `list_custom_metrics` returns four custom metrics and zero formulas, live 2026-09-04. **All four are marked `auto_detected_from_insights`.** None has a description, none tracks a cost per action, none tracks a value, and none has ever been synced from Meta. In other words nobody has configured anything; Parker found these by looking at the data. Their raw names are `offsite_conversion.fb_pixel_custom`, `offsite_conversion.fb_pixel_custom.Call`, `offsite_conversion.fb_pixel_custom.click` and `offsite_conversion.fb_pixel_custom.invitee_meeting_scheduled`.

Two things worth pulling out of that. A `.Call` event is firing, which fits a funnel whose real conversion is a phone call. And `invitee_meeting_scheduled` is the event name Calendly emits, which suggests scheduling software sits somewhere in the funnel. `verified` on the metric list, `inferred` on the Calendly read, and both are questions for the brand rather than conclusions.

**Attribution.** Northbeam is not connected, re-verified live 2026-09-04. Attribution windows are on the Meta default. The reporting surface is Meta Ads Manager in platform, stated by the team at intake and recorded in `running-notes/brand-rules.md`. So Parker's numbers and the team's numbers should agree, and nothing in this brain should imply multi-touch attribution.

**Landing destinations in use.** Three appear in today's pull: `https://www.healthformoms.co/save/` as the workhorse, `https://go.healthformoms.co/save/` as the broken one, and `sub-context-docs/reputation-analysis.md` records a third at `quiz.healthformoms.com` that went live 2026-09-02. A new quiz funnel and a new subdomain in the same fortnight says somebody is actively rebuilding the post-click experience, which makes it more likely the `go` problem is a rollout in progress than a long-standing fault. `inferred`.

**Also on file and routed elsewhere:** two ads sit DISAPPROVED in the account with no visible reason, documented in `sub-context-docs/category-and-market-research.md`.

---

## Open loops

**1. Eleven live ads are pointing at a door that most people never get through.**

The `USHA - CBO - OTP` campaign spent $3,633.54 in the last 90 days and turned 2,291 link clicks into 167 landing page views and 20 leads at $181.68 each. The same video, on the account's normal domain, turns clicks into landing page views 83% of the time and produces leads at $13.26. The only difference between the two is the domain in the link.

Pull: **Surprise.** Identical creative producing a twelvefold difference in cost per lead is not something creative, audience or budget can explain, and nothing else in this brain predicts it.

Question: What happens to a click that lands on `go.healthformoms.co/save/`?

Why it matters: if the page or its pixel is broken, this is money being spent on traffic that never arrives, it is fixable in an afternoon, and it is running into the November ramp. If instead the page works and only the tracking is broken, then twenty leads is an undercount and the campaign is being judged on a number that is not real. Those two situations call for opposite actions and right now nobody knows which one this is.

Territory: **Product.** **Routed to the brand**, since answering it needs the site and the pixel rather than the ad account.

**2. The brand has moderated its comment sections for a day and has never answered one.**

In twenty months and 1,342 comments there is not one brand reply. In the same week the team asked Parker to help hide comments and to help ban a rival operator, and both are reasonable. Meanwhile the most-liked question in the whole corpus, *"Anyone actually have this and have insight?"* at 15 likes, sat unanswered while five strangers answered it, four of them negatively.

Pull: **Tension.** The brand describes its partner agents as friendly, approachable and pressure-free, and its own public conduct in the only room where people ask about it is silence followed by enforcement. Both cannot be the whole picture.

Question: What is stopping the brand from replying in its own comment sections?

Why it matters: the answer separates a real constraint from a habit, and the two lead somewhere completely different. If compliance or the partner agreement forbids the brand speaking about coverage in public, then moderation genuinely is the only lever and the strategy should stop expecting more. If nobody has simply ever owned it, then in a category where trust is the binding constraint the cheapest available win is answering the question people keep asking.

Territory: **Messaging.** **Routed to the brand.** Related to the silence loop in `sub-context-docs/reputation-analysis.md`, which asks what happens to the women reading those threads; this one asks why the brand is not in them.

**3. Two people are shipping about fifty new ads a month.**

147 ads were created in the 90 days to 2026-09-03. The account carries at least four different outside naming conventions, including sixteen ads batched from an animation supplier on a single day in May. The visible team is one operator and a business partner who joined yesterday.

Pull: **Gap.** There is an obvious production engine running behind this account and nothing in this brain knows a single thing about it.

Question: Who actually makes these videos?

Why it matters: everything this brain will ever recommend has to be produced by somebody. Whether the brand can commission a new format, cast a different kind of person, or turn a script around before November depends entirely on a roster nobody has written down.

Territory: **Creators and talent.** **Routed to the brand.**

**4. The brand's own definition of a winner has a second half nobody can see.**

`running-notes/success-definition.md` records the team's bar in their words: *"CPL is important to scale but then we look at the lead quality as well before really scaling."* Cost per lead is visible on every ad. Lead quality lives with the partner agencies and reaches no tool Parker holds, so every scale recommendation this brain makes is made on half the evidence the team itself uses.

Pull: **Gap.** The team named a two-gate standard and only one gate has ever produced a number anybody in this brain has seen.

Question: Who at the partner agencies knows whether a lead was any good?

Why it matters: without it, this brain can only ever say an ad is cheap, never that it is good, and the two come apart badly in lead generation. It also decides something concrete for November, which is whether the ads to scale are the ones with the lowest cost per lead or a different set entirely.

Territory: **Product.** **Routed to the brand.**

---

## Appendix - Parker media links

All links and paths preserved exactly as returned by Parker MCP on 2026-09-04.

**Brand:** Health For Moms, brand `aed0ff06-555d-4f4f-9bf8-31178e2fb977`. **Organization:** `Insuranceyeti`, `71367b2e-920c-46ca-81a5-51363f3c9ee4`. **Ad account:** `HealthForMoms`, act `484897827497337`, USD, primary and enabled. **Brain repo:** https://github.com/insuranceyeti/creativeyeti

### The matched pair behind the landing destination finding

Same video, same media hash `00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399`, two different landing domains.

- `moms-63 2b` — `USHA - ABO - TEST - MOMS`, ad set `Moms63`, landing `https://www.healthformoms.co/save/`, 417 leads at $13.26
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
- `moms-63 2b - Copy` — `USHA - CBO - OTP`, ad set `Moms CBO OTP`, landing `https://go.healthformoms.co/save/`, 6 leads at $160.84
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247339552100519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

### The other high-spend ads on the `go.healthformoms.co` destination

- `Moms Nahuel WV#1 - V9 - Copy` — $1,639.37, 690 link clicks, 63 landing page views, 6 leads at $273.23
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872230519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/645496c411d82a546a3e2deada69459c716615ad09f635ca0b978625c2778b37.mp4
- `moms-63 3e - Copy` — $506.38, 332 link clicks, 31 landing page views, 8 leads at $63.30
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247339547070519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- `moms-53 3 - Copy` — $495.57, 511 link clicks, 9 landing page views, zero leads
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247339531520519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- `Moms Nahuel WV#2 - V3 - Copy`
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872220519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- `Moms36 - 3 - A - 2 - V4c - Copy`
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872130519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- `Animation Agency #4 - H1 - Copy`
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872150519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- `Animation Agency #5 - H3 - Copy`
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872140519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- `Moms36 - 3 - A - 3 - V5a`
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- `OMC-Health for Moms-[B3-C11-V7] - Copy`
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872180519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- `Moms42 - 1 - V1a - Copy`
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872120519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

### The outside animation supplier's batch, created 2026-05-06

- `Animation Agency #5 - H3` — ad set `Animation Agency #5`, $201.14 lifetime, 5 leads at $40.23
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120242276504880519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/451d49f7e63eb2f65fe125f35ddb70f77bb3c27ccbe8d33ddf06cadf296e3a27.mp4
- `Animation Agency #4 - H1` — the personified medical bill, verbal hook "I am your deductible", $78.34 lifetime, 3 leads at $26.11
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120242276281690519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1fcb56617f1abef55835db4394f845606247c6dc9ddd955792cd7c71d21bd222.mp4
- `Animation Agency #6 - H3`
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120242276602730519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- `Animation Agency #6 - H2`
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120242276602740519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- `Animation Agency #5 - H1`
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120242276504870519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977

### The account's top live spender, for reference on structure and copy

- `Moms43 - 4 - V3` — `USHA - ABO - SCALE - MOMS`, ad set `Moms43 - 4 (State Moment)`, $43,119.77 in the 90-day window, 1,935 leads at $22.28
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4
- `MOMS38 - 1 - V1` — the ad the rival operator worked, $54,173 lifetime
  - Parker: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239479305920519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
  - Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/50a0309be06d87e55299b9e00d7962b88516c847dec96e80cfffc8098393996b7531.mp4

### Landing destinations in use

- https://www.healthformoms.co/save/
- https://go.healthformoms.co/save/
- https://quiz.healthformoms.com/#/indvfam — live 2026-09-02, blocked to WebFetch

### Parker chat threads read for this doc

Slack channel `C0BUQEFF70V`, team `T02N4RQ62DR`.

- `1788469337.157819`, 2026-09-03 — the ramp-up, the ICP correction, and the brand guidelines upload
- `1788469337.613099`, 2026-09-03 — the ad account overview request
- `1788473402.812619`, 2026-09-03 — the tooling and workflow conversation, Gethookd, and how the team wants to work
- `1788478345.205779`, 2026-09-03 — the brain setup status check
- `1788479022.847859`, 2026-09-03 — the comment moderation exchange and the partner agency flag
- `1788480849.190169`, 2026-09-04 — the request to locate an ad in order to ban a rival operator
- `1788481525.524429`, 2026-09-04 — the introduction of the business partner
- `1788529081.275569`, 2026-09-04 — the landing page headline request
- Web thread `b4aa53c3-f10e-4ecb-9612-c40f39803f6a`, 2026-09-03, titled "Parker Brain setup"
