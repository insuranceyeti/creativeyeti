---
brand: health-for-moms
doc: monthly-performance-report
month: 2026-08
report_cycle: 2026-09
generated_on: 2026-09-03
refresh_by: 2026-10-03
date_range: 2026-08-01 to 2026-08-31
prior_month_compared: 2026-07-01 to 2026-07-31
data_sources_read: [live Meta ads manager via Parker MCP search_facebook_ads_sql on account HealthForMoms act 484897827497337, Parker MCP search_facebook_ad_comments_sql, Parker MCP get_brand_persona brand context document, Parker MCP search_chat_history, running-notes/brand-rules.md, running-notes/success-definition.md, running-notes/missing-context.md, audits/2026-Q3/90-day-performance-audit.md, audits/2026-09/monthly-hook-audit.md]
knowledge_docs_read: [parker-system/creative-strategy-context/ad-account-analysis.md, parker-system/creative-strategy-context/ad-metrics-glossary.md, parker-system/creative-strategy-context/killer-performance-ads.md, parker-system/creative-strategy-context/andromeda-v2.md]
test_slate_committed_at_month_start: no
prior_month_lineage: none. This is the first monthly performance report for this brand. The nearest prior read is the 90-day performance audit generated 2026-09-03, whose window overlaps this one.
data_limitations:
  - "No test slate was committed at the start of August. Parker chat history holds six threads and every one was created 2026-09-03, so there is no record of a hypothesis or a success bar set before the month began. Every test in section three was reconstructed from campaign and ad set creation dates plus the creative itself, and each reconstructed hypothesis is marked inferred."
  - "No prior monthly performance report exists. Month-over-month movement here was built by pulling July directly rather than by carrying a baseline forward."
  - "Lead quality is invisible to Parker. It lives with the partner insurance agencies, not in Meta. Every winner named below has cleared gate one only."
  - "Placement-level breakdown is not exposed by the Parker MCP ad tool for this account. The demographics block returns age, gender, device and platform only, so no Feed versus Reels versus Stories read was possible."
  - "Reach and frequency are not returned for this account, so the saturation check that ad-account-analysis.md calls central could not be run and the entity-ID read below rests on creative evidence rather than on delivery data."
  - "Account-level hook rate and hold rate are not in the period summary. Both are reported spend-weighted across the top 20 ads, which carry 99.36% of August spend and 99.58% of July spend."
  - "Two of August's top 20 ads, Moms43 - 4 - V3 and MOMS39 - 2 - V2 - Copy, return no landing_url field. Their destination is inferred from their landing rate rather than read directly."
  - "Northbeam is not connected. Every number here is Meta-reported on the Meta default attribution window. This is not multi-touch attribution."
  - "Customer reviews and post-purchase surveys are dark surfaces with zero rows, and no competitors are tracked in Parker, so no outside-in check on these reads was possible."
  - "Ad naming convention was never supplied by the team. Ad and campaign names are used as inventory handles only, never as evidence of what a creative is or does."
---

# Monthly performance report — Health For Moms — 2026-08

This is the September cycle, and it reads August, the last month that closed. The window is 2026-08-01 to 2026-08-31 in America/New_York, pulled live from the Meta account HealthForMoms, act 484897827497337, on the Meta default attribution window. July is pulled the same way and sits alongside every figure.

Here is how the reading was done, so a skeptical reader can check it. I pulled all 90 ads that carried delivery in August and worked from the top 20 by spend, which together carry $42,473.75 of the month's $42,748.63. That is 99.36% of the money, so this is not a sample, it is the account. I did the same for July, where the top 8 carry 99.58% of $18,389.74. On top of that I ran four segment pulls: ads by landing destination, ads by creation date, the quiz destination across the whole quarter, and all 59 Facebook ad comments left in August. Every creative claim rests on the text hook, verbal hook, visual hook and angle fields Parker stores for each ad, never on the ad name. Where I could only see a name, I say so.

Two rules from the brand shape every judgment below. First, this is lead generation with zero purchase events, so ROAS, AOV and purchase value are meaningless here and never appear. The account is judged on CPL, lead volume, CPM, CTR, hook rate and hold rate. Second, a winner here is two-gated. The team said it plainly at intake: *"CPL is important to scale but then we look at the lead quality as well before really scaling."* Parker can see gate one and cannot see gate two. So nothing below is called a winner outright. Ads that beat the CPL bar are called gate-one candidates, and lead quality stays the open question on every one of them. The brand's own CPL tiers are the bar: under $15 is fantastic, $15 to $20 is good, $20 to $25 is meh, over $25 is not good. *Stated* by the brand in the brand context document.

The month in one line: the account more than doubled its spend, more than doubled its leads, and paid about four percent more per lead once a broken landing page is stripped out. That is a real scaling result, and it is buried under a headline number that looks worse than the month actually was.

## What worked

**The August creative rebuild, as a cohort.** 85 ads created inside August carried $20,255.73, which is 47.4% of the month's spend, and returned 1,060 leads at a $19.11 CPL. Strip out the 11 ads pointed at the broken destination described in the next section and the same cohort reads $18,209.33 for 1,054 leads at a **$17.28 CPL**, squarely inside the brand's "good" band. The five carryover ads that survived from earlier months took the other $22,492.90 and returned 927 leads at $24.26. *Verified* by a created-time filtered pull against the month total.

**moms-63 2b.** $5,336.12 for 403 leads at a **$13.24 CPL**, a 40.01% hook rate, a 2.38% hold rate, a 1.72% CTR and a $21.27 CPM. Created 2026-08-14. Destination `www.healthformoms.co/save/`. *Verified* from its ad record.

**moms-63 3e.** $3,427.98 for 237 leads at a **$14.46 CPL**, a 42.06% hook rate, a 2.88% hold rate and an $18.34 CPM, the cheapest impressions among the top spenders. Created 2026-08-14. *Verified* from its ad record.

**moms-53 3.** $1,243.37 for 90 leads at a **$13.82 CPL**, a 36.40% hook rate, a **3.25% CTR** and a **$0.85 cost per link click**, both the best in the top 20. Created 2026-08-25. *Verified* from its ad record.

**The "Battle Res" resurrection set.** Three older ads relaunched on 2026-08-11 and 08-12: MOMS39 - 2 - V2 - Copy at $1,351.90 for 72 leads at $18.78, Moms36 - 3 - A - 2 - V4c - Copy at $597.71 for 30 leads at $19.92 on an 11.29% hold rate and a 9.78-second average play time, and Moms Nahuel WV#1 - V9 - Copy at $403.70 for 21 leads at $19.22. All three landed in the "good" band. *Verified* from all three ad records.

The pattern behind these wins is not a new angle. It is new footage on a proven line. The three cheapest ads of the month all reuse text that the account already knew converts, and all three put a different image under it. moms-63 2b and 3e carry the exact POV husband line that the April workhorse carries, word for word, but the picture changed: instead of a mother and baby lying still on white bedding, a well-dressed mom walks out of a house holding her young son's hand, outdoors, in motion. Same message, different style. Read through the Andromeda v2 differentiation hierarchy, that is a vehicle-and-hook change sitting one rung below a format change, and it is exactly the kind of move the entity-ID rules reward, because Meta weighs the first three seconds hardest and these three seconds are genuinely different. The account paid $13.24 and $14.46 for leads on the new footage and $23.37 on the old footage carrying the identical words. *Verified* from both ads' visual hook and text hook fields read against their period metrics. That is about as clean a natural experiment on visual differentiation as an account ever hands you.

moms-53 3 is a different and more interesting win, because it is the brand's own best angle finally shot as a person instead of a mood. A woman in a grey tank top stands in front of a white screen listing US states under the heading "Approved State List ✔️" and says, "I'm so thankful for the mom that told me about this." The state angle is what the brand told us works best: *"State angle has worked very well if you see the account. Emotional and direct response."* This ad is that mechanic delivered as a mom-to-mom recommendation, and it produced the highest CTR and the cheapest clicks in the account by a wide margin. In Schwartz terms it plays solution aware, and in Life Force 8 terms it runs on care and protection of loved ones plus social approval, the borrowed trust of another mother. *Inferred* from the verbal hook and visual hook read against the awareness ladder in killer-performance-ads.md.

The resurrection set matters for a different reason: it says the account's older library is not spent. Three ads pulled off the shelf and relaunched all cleared $20 CPL, and one of them, Moms36 - 3 - A - 2 - V4c - Copy, holds attention for 9.78 seconds, more than double the account's biggest ad. Against the 12% to 15% hold-rate floor in ad-account-analysis.md, an 11.29% hold rate is the closest anything in this account got to healthy all month. *Verified* from its period metrics.

## What didn't work

**Moms43 - 5 - V1.** $6,677.21 for 251 leads at a **$26.60 CPL**, up from $18.10 in July on $2,443.02. Spend tripled, CPL rose 47%. Hook rate 39.00%, hold rate 8.05%, CPM $32.81 against an account average of $23.66. Second-biggest line item of the month and the biggest collapse. *Verified* from matched July and August pulls on facebook_ad_id 120243987355020519.

**The Moms54 crying-mom set.** Three ads created 2026-08-13, ad set now paused. moms54-2 at $1,463.05 for 42 leads at **$34.83**, moms54-3 at $1,280.49 for 43 leads at **$29.78**, moms54-4 at $646.44 for 17 leads at **$38.03**. Combined $3,389.98 for 102 leads at a $33.24 CPL, all three in the brand's "not good" band. And yet moms54-3 posted a **57.02% hook rate, a 13.65% hold rate and an 8.08-second average play time**, the best attention numbers anywhere in the account. *Verified* from all three ad records.

**The go.healthformoms.co destination.** 11 ads created 2026-08-17 and 08-31 under the "Moms CBO OTP" campaign. $2,046.40 for 6 leads at a **$341.07 CPL**. They bought 1,103 link clicks and delivered **77 landing page views**, a 7.0% landing rate against 84.6% everywhere else in the account. *Verified* by a landing-url filtered pull across the month.

**Moms43 - 4 - V3, the workhorse, quietly getting more expensive.** $15,800.53 for 676 leads at **$23.37**, up from $19.74 in July on almost identical spend. Impressions fell from 770,527 to 701,713 while CPM rose from $19.88 to $22.52. *Verified* from matched July and August pulls on facebook_ad_id 120241073380060519.

Start with the destination, because it is the read that changes every other number on the page. Those 11 ads are not a creative failure. They are a plumbing failure being scored as a creative one. Nine of every ten moms who clicked never reached a page. The worst case is Moms Nahuel WV#1 - V9 - Copy, which bought 687 link clicks and produced 63 landing page views and 6 leads for $1,631.40, and whose click quality score reads 9.17 against a range of 72.45 to 90.14 across the other 19 ads in the month's top 20. The same creative file, running to `www.healthformoms.co/save/` under a different campaign, produced 21 leads for $403.70 at a $19.22 CPL. Identical video, identical hook, identical woman on screen. One destination made it a "good" ad and the other made it a $271.90 ad. *Verified* by comparing facebook_ad_id 120247022199760519 against 120247145872230519 across the same month. This is why the whole report segments by destination before it grades anything. Left in the blend, that $2,046.40 pushes the month's CPL from $20.55 to $21.51 and drags the account from the edge of "good" into the middle of "meh" on the strength of a redirect nobody was watching.

Moms43 - 5 - V1 is the honest failure of the month and it deserves the plain version. This is the ad the 90-day audit named as the counter-example that holds attention, a UGC selfie video with a screenshot of someone complaining about high deductibles, opening on the spoken line "This is why you can't simply just say 'Oh, I have insurance, I'm covered.'" It got a big budget increase in August and it broke. Its hold rate actually improved, from 6.94% to 8.05%, so people were watching more, not less. What moved against it was cost: CPM went from $26.22 to $32.81, the most expensive impressions of any ad with real spend. That is the shape of an audience getting used up rather than a creative getting worse. Per ad-account-analysis.md, when CPM climbs while attention holds steady, the account is paying more to reach the same pool, and frequency is the metric that would confirm it. Parker cannot see frequency on this account, so this stays *inferred* rather than verified. The team's own rule points the same way: efficiency outranks volume, and this ad got more money while its cost per lead was drifting up.

The Moms54 set is the most instructive failure, because it did the hard part brilliantly and then lost. A young woman with a red, tear-stained face speaks into her phone camera in tight close-up: "Just got off a two hour call fighting for them to cover my newborn son's hospital stay." That is a genuine hook by every standard in killer-performance-ads.md. It stops the scroll, it targets a real emotion, it has the WOW factor of something you do not see in other insurance ads. 57.02% hook rate and 13.65% hold rate prove it worked. Then it sold nothing at $29.78 a lead. The diagnosis is stage of awareness, not craft. That opener is an unaware or problem-aware lead. It makes a mother feel the fear, and the brand's whole conversion mechanic is a solution-aware move: check whether your state is on the list, then talk to an agent. A viewer landed in high-intensity negative emotion is not in the mood to fill in a form about her ZIP code. The CPM tells the same story from the auction side, $36.75 and $37.83 on the two crying ads against $18.34 on the calm outdoor walk. Meta charged this account a premium to put grief in front of moms and the moms did not convert on it. *Inferred* from the visual and verbal hooks read against the awareness ladder and the emotional-state framing in killer-performance-ads.md, corroborated by the CPM gap.

And the workhorse is aging. Moms43 - 4 - V3 spent almost exactly what it spent in July and bought 68,814 fewer impressions and 100 fewer leads. Its hook rate is unchanged at 45.50%, so the first frame still works. Its hold rate is 3.25% and its average play time is 4.06 seconds, both far under the floor, and both unchanged too. Nothing about the creative got worse. It just costs more now. This ad has been running since 2026-04-15.

## What we tested

No test slate was committed at the start of August. Parker's chat history holds six threads and all six were created on 2026-09-03, the day this brain was built, so there is no written record of a hypothesis or a success bar set before the month started. That absence is itself the finding, and it is the first thing to fix. The bets below were reconstructed from campaign creation dates, ad set groupings and the creative itself. Each hypothesis is what the evidence says the team was trying, marked *inferred*, not what the team told anyone.

**Test 1 — New footage under the proven POV line.** What was tested: the account's best-known text hook, the POV husband line, re-shot with a mom and son walking outdoors instead of a mother and baby lying in bed. Baseline: Moms43 - 4 - V3 at a $23.37 CPL in the same month. Result: moms-63 2b at $13.24 on $5,336.12 and moms-63 3e at $14.46 on $3,427.98. Launched 2026-08-14. **Worked.** *Verified* from both ad records against the same-month baseline.

The hypothesis reads as "the line still converts, the picture is what is tired." That is a vehicle-and-hook swap in the Andromeda v2 hierarchy, one rung below a full format change, and it is the single highest-value thing the account learned all month: the account bought leads 43% cheaper by changing what the viewer sees while changing not one word of what she reads. The size of the gap is what makes it a real result rather than noise. Two ads, $8,764.10 of combined spend, 640 leads, both landing in the "fantastic" band against a same-month baseline of the identical copy at nearly double the cost.

**Test 2 — Emotional intensity as a hook lever.** What was tested: three UGC ads built on visible distress, a crying mother, a newborn's hospital stay, a son falling off the monkey bars. Baseline: the account's calm lifestyle openers at roughly 40% hook rate and 3% hold rate. Result: hook rate up to 57.02% and hold rate up to 13.65%, CPL between $29.78 and $38.03, ad set paused. Launched 2026-08-13. **Failed on cost, succeeded on attention.** *Verified* from the three ad records; the hypothesis behind the test is *inferred* from the creative and the launch date, since no slate was written down.

The hypothesis was almost certainly "this account cannot hold anyone, so lead with something impossible to scroll past." It worked on its own terms and lost anyway. The lesson is that hook rate and hold rate are behavior metrics, not scale metrics, and ad-account-analysis.md is explicit that a high hook rate does not by itself mean an ad is bringing in money. This test bought the account its best attention numbers of the year and its worst cost per lead, in the same three files.

**Test 3 — Bringing dead ads back.** What was tested: three previously paused creatives relaunched into a fresh campaign. Baseline: their own historical performance and the account's current CPL. Result: $18.78, $19.92 and $19.22 CPL on $2,353.31 combined. Launched 2026-08-11 and 08-12. **Worked.** *Verified* from the three ad records.

The hypothesis reads as "the audience has turned over enough that old creative is new again." It paid off cheaply, and it is worth naming that this test cost almost nothing to run because the assets already existed. Against the brand's stated bottlenecks, which include casting, production and scripting, a shelf of proven files that still deliver $19 leads is the cheapest inventory the team owns.

**Test 4 — A second landing destination.** What was tested: routing 11 ads to `go.healthformoms.co/save/` instead of `www.healthformoms.co/save/`. Baseline: an 84.6% landing rate everywhere else in the account. Result: a 7.0% landing rate, 6 leads, a $341.07 CPL. Launched 2026-08-17. **Failed, and not on creative.** *Verified* by the landing-url filtered pull and by the same video file performing normally on the other destination.

Whatever the hypothesis was, the test never got the chance to answer it, because the page did not receive the traffic. This is the one result in the month that must not be read as a creative verdict. Four of those 11 files also run to the working destination elsewhere in the account and perform normally there.

**Test 5 — The state list as a person, not a graphic.** What was tested: the state angle delivered by a woman on camera crediting another mom. Baseline: the account's other new-concept launches in August. Result: $13.82 CPL, 3.25% CTR, $0.85 cost per link click on $1,243.37. Launched 2026-08-25. **Worked, on six days of delivery.** *Verified* from its ad record, with the read marked thin on run time.

Six days is thin. Called a promising early read rather than a settled result, and flagged for a fair test in September at real budget.

**Test 6 — Calm lifestyle POV without the savings claim.** What was tested: the Moms65, Moms66 and Moms68 sets, POV overlays about peace of mind rather than a dollar figure, over children and domestic scenes. Result: moms-66-816 at $23.19 on $927.73, moms-65 1a at $27.35 on $738.56, moms-66-816 - 2 at $34.51 on $138.04, moms-66-816 - 5 at $47.38 on $47.38, moms-65 1c at $15.38 on $46.13. Launched 2026-08-18 and 08-27. **Mostly failed, with one file too small to judge.** *Verified* from all five ad records.

The hypothesis reads as "the feeling of being covered will sell as well as the number." It did not. Every version that got real money landed in "meh" or worse, and the one cheap result, moms-65 1c at $15.38, sits on $46.13 of spend and 3 leads, which is nowhere near enough to call. Note that moms-66-816 - 2 posted a 64.13% hook rate, the highest single hook rate in the account this month, and still cost $34.51 a lead. That is the same lesson as Test 2 arriving from the opposite direction.

**Test 7, carried over from July and quietly killed — claymation.** In July the team launched a set of animated ads under Moms46, a claymation woman at a desk buried in unpaid bills, with hooks like "Did you know your bill is cheaper if you don't use your insurance?" That set spent $516.86 across four files for 16 leads at a $32.30 CPL. It also posted the best hold rates in the July account: 13.59%, 12.58% and 11.15%, all at or near the 12% floor that nothing else in this account reaches. By August every one of those files was gone. **Inconclusive, and retired before it was settled.** *Verified* by pulling the four Moms46 files in July and finding none of them carrying delivery in August.

This is the month's most uncomfortable result, and it is why the test lens has to stay separate from the performance lens. A format that was the only thing in the account clearing the hold-rate floor was killed on a CPL read taken over roughly four weeks and under $520 of spend. That is a defensible call on cost and a possibly expensive one on learning, because the differentiation hierarchy in Andromeda v2 puts format at the very top, and animation is the largest format change this account has ever made.

## What we learned

The clearest thing August taught this account is that its creative problem is not what it says, it is what it shows. Three separate lines of evidence in the same month point at the same conclusion and none of them was designed to. The POV husband line produced a $23.37 lead on April's footage and a $13.24 lead on August's footage with identical words. The crying-mom set produced the account's best attention numbers and its worst costs with a completely different picture and a similar underlying message. The claymation set was the only thing in the account holding viewers past twelve percent, and it was the only thing that looked nothing like anything else. Read across all three, the account's performance is tracking the image far more tightly than the copy. *Inferred* from three independent same-month comparisons rather than from a controlled test. This is exactly what Andromeda v2 describes: Meta scans visual composition, people in frame, setting, camera angle and scene structure in the first three seconds, and a different headline over the same visual reads as the same ad. The account has been running a messaging test in a system that mostly grades pictures.

That reframes the concentration problem the 90-day audit flagged. Six ads sharing the POV husband text hook carried $25,348.18 in August, which is 59.3% of the month. On the old reading, that is a message concentration risk. On the evidence above, it is better understood as an image portfolio question, and the good news inside it is that the account already proved it can break the fingerprint cheaply. moms-63 2b and 3e sit in that 59.3% cluster and they look nothing like the April original. The line is not the liability. Four near-identical mother-and-child domestic scenes were. *Inferred* from the visual hook fields on the cluster, since entity-ID grouping is not something Meta exposes and frequency is not returned for this account.

The second thing the month taught is that this account's funnel is short and it needs to stay short. Hold rate is 4.51% spend-weighted across 99.36% of the month's spend, against a 12% to 15% floor, and it barely moved from July's 3.95%. The account is not going to become a long-watch account before Open Enrollment, and August is the month that showed it does not have to be. moms-63 2b delivered $13.24 leads on a 2.38% hold rate and a 3.36-second average play time. moms54-3 delivered $29.78 leads on a 13.65% hold rate and an 8.08-second average play time. In this account, over this month, the ads that held people longer cost more per lead, not less. *Verified* across the top 20 by spend, which carry 99.36% of the month. That is the opposite of the working theory the 90-day audit carried forward, and it is worth stating plainly because it changes what to brief. The job of these ads is to qualify a mom in two seconds and move her, not to keep her. Per hook-psychology's frame of what a hook has to do, this account wins on notice and qualify and is not currently paid for transport.

The third thing is the one nobody was looking for. In August the account's ads drew 59 Facebook comments. **36 of them, or 61.0% of everything said all month, are the single word "Help."** Every one of those 36 sits on Moms43 - 4 - V3, which carries 47 of the month's 59 comments, or 79.7% of them, on 37.0% of the spend. *Verified* by a full pull of August ad comments. Neither the ad copy nor any hook field Parker can see contains an instruction to comment "Help," so what is producing this is genuinely unexplained. What is not in doubt is what it represents: three dozen mothers a month raising their hand in a channel with no path to an agent in it. If even a fraction of those are real intent, the account is leaking qualified leads into a comment thread. The team is at least half aware of this. In Slack on 2026-09-03 someone asked, verbatim, *"Do you have permissions to clean up comments or no?"*

The rest of the comment thread is a small, sharp voice-of-customer surface and it is the only one this brand has, since reviews and surveys are both empty. The most-liked comment of the entire month, with 2 likes and a reply, is an objection: *"It only works if you don't have any preexisting conditions. You gotta be perfectly healthy to qualify it looks like."* A second reads *"Has anyone had success with this?"* and a third *"Is this insurance or something like a Christian health share?"* Those three lines are a trust problem, a proof problem and a category-confusion problem, and none of them is currently answered anywhere in the creative. Against golden rule four in killer-performance-ads.md, zero confusion, this account has a real gap: moms are not sure what they are being offered or whether it will cover a sick child. That is the objection to beat before November.

The state mechanic cuts both ways, and August is the first month with evidence on the second edge. moms-53 3 produced the account's cheapest clicks and one of its cheapest leads. It also produced *"Ofc Georgia ain't on there 🤣"* and *"What a joke!! They don't have quote for me In tx"*, both on 2026-08-29 and 08-31. Texas and Georgia are two of the largest uninsured populations in the country. *Stated* as general category knowledge, not verified against a source in this run. The exclusivity that makes the hook work is also turning away moms in the biggest states, loudly and in public, under the ad. That is worth knowing before the team scales the angle that works best.

Finally, the month gave a straight answer to the question the 90-day audit left hanging, which was whether the account could put money behind newer creative without CPL rising. It can. Spend on ads created inside the month went from 26.6% across the quarter to 47.4% in August, and that cohort delivered leads at $17.28 clean against $24.26 on the two survivors holding the other half of the budget. The account paid $7 less per lead on the half of its money that went to work made this month. *Verified* by the created-time filtered pull, net of the broken destination. The gate-two caveat stands on all of it, because Parker cannot see whether a $17 lead from a six-day-old ad holds up with the agencies the way a $24 lead from a five-month-old ad does. That is the single most valuable piece of information the team could hand back.

## What we should do next month and why

**Stop reporting a blended CPL until the destinations are separated, and fix the redirect this week.** August's headline CPL of $21.51 is not the account's cost per lead. It is $20.55 on 95.2% of the spend and $341.07 on the rest, and the difference is one broken page. This is the cheapest fix available and it has the largest effect on the number the team steers by. The proof is sitting in the account: one video file ran to both destinations in the same month and produced a $19.22 lead on one and a $271.90 lead on the other. Until that is resolved, every ad routed through `go.healthformoms.co` should be treated as unscored, not as a loser, because grading creative on a page that eats 93% of its traffic will get good creative killed. Related and urgent: 15 ads pointed at `quiz.healthformoms.com` went live on 2026-09-02 and 09-03 and have spent $139.01 for 2 leads so far. Check that destination's landing rate on day one, not at the end of September.

**Make September a footage sprint, not a copy sprint.** The single clearest lever this account has is putting new pictures under lines that already convert. It returned a 43% cheaper lead in August on the one occasion it was tried properly. Concretely: take the POV husband line and the state list line, the two the account has proven, and shoot each one across three genuinely different setups, meaning a different person, a different setting and a different camera position, not a different overlay on the same clip. Andromeda v2 is explicit that a different text overlay on the same visual is a false differentiator and gets grouped into the same entity, so this only pays if the first three seconds are actually different. Budget the round the way the brand already said it wants to work, one to five net-new concepts and one to five iterations a month, and spend the iteration slots here rather than on new headlines.

**Give animation a real test instead of leaving it dead.** The claymation set was the only creative in this account clearing the hold-rate floor and it was retired on $516.86 and about four weeks. Format is the top rung of the differentiation hierarchy, and this account is a video account with almost no format variety in it, which is the brand's own diagnosis: *"Right now we're mainly on iterations of our state angle that you will see in the account doing well. But not a ton of creative diversity."* Relaunch two claymation files with the state-list mechanic in them rather than the general hospital-billing angle, and give them enough budget to produce at least 50 leads before calling it. If the CPL still lands above $25 with the proven mechanic inside, the format is genuinely wrong for this account and it can be closed for good. Right now nobody knows.

**Retire the crying-mom vehicle for cold traffic and keep the emotion.** The Moms54 set proved this account can win attention whenever it wants to. It also proved that grief in the opener does not convert a solution-aware mechanic. Rather than abandoning the emotional register, move the intensity later. Open calm, qualify with the state list, and let the harder story land at three to five seconds where killer-performance-ads.md puts the best benefit or the re-hook. That is a script change, not a casting change, and the account already has the footage.

**Answer the pre-existing-conditions objection on camera, before November.** The most-liked comment of the month says the product only works if you are perfectly healthy. Another asks whether it is insurance at all or a health share. Nobody in the account's creative answers either one. This is the highest-value new script in the queue, and the evidence for it is customer language, not a hunch. A skeptical-testimonial or comment-response format, both of which the brand already listed as formats it wants to test, would carry it naturally. That objection will get louder in Open Enrollment when every competitor is in the feed making comparable claims.

**Do something with the 36 "Help" comments, and decide what they are.** Whether they are prompted or organic, three dozen moms a month are raising a hand in a channel with no route to an agent. At the account's own $19 to $23 CPL, that pile is worth a few hundred dollars a month at least, and it costs nothing but attention to work. Do this before scaling budget, because the volume of it will scale with the spend.

**Then, and only then, scale, and scale the new cohort rather than the survivors.** The team's stated sequence is efficiency first, then volume. August satisfied the first half: spend went up 132.5% and clean CPL moved only 3.8%, from $19.80 to $20.55. The account has room. But 52.6% of the money is still sitting on two ads that cost $24.26 a lead, one of them launched on 2026-04-15 and now buying fewer impressions for more money. Shift that weight toward the August cohort as September's new footage proves out. The one thing that must come with it is gate two. Every recommendation above clears the CPL gate only. Before real budget goes behind a $13 lead from a six-day-old ad, someone at the partner agencies needs to say whether those leads close like the $24 ones do. That question is worth more to this account right now than any creative decision in this report.

## Open loops

First, what the 90-day audit left open and where those loops stand after August. Loop 4, whether the account could move budget to newer creative without CPL rising, is largely answered: it moved from 26.6% to 47.4% of spend and the new cohort came in $7 cheaper per lead. Loop 3, what the surviving high-hold ads do in the first five seconds, got an answer that reverses the premise, because in August the high-hold ads were the expensive ones. Loops 1, 2, 5, 6 and 7, on the young-mom skew, the spend collapse, the male drift, the narrow casting and the missing Open Enrollment history, are all still open and none of them was tested this month. The loops below are new questions this month raised.

**1. Three dozen moms typed one word and nobody knows why.**
36 of the 59 Facebook comments the account received in August are the single word "Help," and every one of them sits on Moms43 - 4 - V3. Nothing in that ad's copy, text hook, verbal hook or visual hook that Parker can read tells anyone to comment "Help."
*Pull: Surprise.* Sixty-one percent of a month's comments being one identical word is not a pattern any of the account's other 89 ads produced, and nothing in the creative explains it.
**Question: What are the moms who comment "Help" on this ad actually asking for?**
If they are qualified moms who could not find the link, the account is losing leads it already paid for, and the fix is a reply routine rather than a creative one.
*Territory: Messaging.*

**2. The market thinks you have to be healthy to qualify.**
The most-liked comment of the month, with 2 likes and a reply, reads *"It only works if you don't have any preexisting conditions. You gotta be perfectly healthy to qualify it looks like."* A separate thread asks *"Is this insurance or something like a Christian health share?"* and another asks *"why don't any of the plans offer prenatal care?"*
*Pull: Tension.* The brand describes itself as a matching service for families who are struggling with coverage, and the loudest voices under its ads describe a product that only works for families with nothing wrong.
**Question: Who does the market believe this product is for, and where did that belief come from?**
If moms with a sick kid or a pregnancy are self-selecting out before they ever click, the addressable pool going into Open Enrollment is smaller than the targeting suggests, and the fix is a proof script rather than more spend.
*Territory: Product.*

**3. The best hook in the account was also the most expensive.**
The Moms54 set posted a 57.02% hook rate, a 13.65% hold rate and an 8.08-second average play time, the best attention numbers anywhere in the account this month, and produced leads at $29.78 to $38.03 while the calmest ads produced them at $13.24.
*Pull: Tension.* Hook rate and cost per lead usually move together in this account and this month they moved hard in opposite directions, so one of the two is measuring something other than what it is being used for.
**Question: Who is a crying mother in a close-up bringing to this account, and what do those people do after they click?**
Knowing whether that hook draws a different kind of mom or the same mom in a worse mood decides whether the emotional register gets rebuilt or retired before November.
*Territory: Creators and talent.*

**4. The angle that converts best is the one people are angriest about.**
moms-53 3, the "Approved State List ✔️" ad, produced the account's cheapest clicks at $0.85 and a $13.82 CPL. Under it sit *"Ofc Georgia ain't on there 🤣"* and *"What a joke!! They don't have quote for me In tx."*
*Pull: Tension.* The exact mechanic that makes the hook work by narrowing the field is publicly turning away moms in two of the country's largest uninsured states.
**Question: How much demand is the state list turning away, and where is it concentrated?**
If a large share of the moms this account reaches sit outside the approved states, the answer changes both the targeting map and how loudly the list should be shown.
*Territory: Product.*

**5. Half the budget is still on two old ads and nobody can see whether that is the safer half.**
Five carryover ads took 52.6% of August spend at a $24.26 CPL while 85 ads made inside the month took 47.4% at $17.28 clean. Parker can see that gap and cannot see what happens to either set of leads after the handoff.
*Pull: Gap.* There is a seven-dollar-per-lead difference sitting in the account and the one piece of information that would settle whether to act on it lives entirely outside Meta.
**Question: How do the leads from the August creative compare with the leads from the older ads once the partner agencies have worked them?**
This is gate two on every recommendation in this report, and without it the whole scaling plan rests on half the brand's own definition of a winner. **This one only the brand can answer.**
*Territory: Product.*

## Appendix - Parker media links

Every ad discussed in the body of this report, indexed so a strategist can reopen the media without searching. Links and paths are preserved exactly as returned by the Parker MCP.

**M001: Moms43 - 4 - V3.** August's top spender at $15,800.53, 37.0% of the month, 676 leads at a $23.37 CPL, 45.50% hook rate, 3.25% hold rate, 4.06-second average play time. Discussed in "What didn't work" as the aging workhorse, in "What we learned" as the source of 47 of the month's 59 comments, and in open loop 1. Created 2026-04-15. No landing_url returned; destination inferred from an 85.7% landing rate.
Facebook ad id: 120241073380060519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

**M002: Moms43 - 5 - V1.** $6,677.21 for 251 leads at $26.60, up from $18.10 in July. 39.00% hook rate, 8.05% hold rate, $32.81 CPM. The month's biggest collapse, discussed in "What didn't work." Created 2026-06-01.
Facebook ad id: 120243987355020519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120243987355020519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0fe2980848d12fe1c6fd107a759e68fe37d8776c34235b5fab3c15e751af171d.mp4
Landing page: https://www.healthformoms.co/save/

**M003: moms-63 2b.** $5,336.12 for 403 leads at a $13.24 CPL, the month's cheapest lead at scale. 40.01% hook rate, 2.38% hold rate. The new footage under the proven POV line. Discussed in "What worked" and Test 1. Created 2026-08-14.
Facebook ad id: 120247093361410519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
Landing page: https://www.healthformoms.co/save/

**M004: moms-63 3e.** $3,427.98 for 237 leads at $14.46, 42.06% hook rate, $18.34 CPM. Sibling of M003 in Test 1. Created 2026-08-14.
Facebook ad id: 120247093478820519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4
Landing page: https://www.healthformoms.co/save/

**M005: moms-53 3.** $1,243.37 for 90 leads at $13.82, a 3.25% CTR and a $0.85 cost per link click, both best in the top 20. The "Approved State List ✔️" opener. Discussed in "What worked," Test 5 and open loop 4. Created 2026-08-25.
Facebook ad id: 120247254787160519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4
Landing page: https://www.healthformoms.co/save/

**M006: moms-53 3 - Copy.** Same video file as M005 routed to the broken destination. $342.80, 368 link clicks, 7 landing page views, zero leads. Discussed in "What didn't work." Created 2026-08-31.
Facebook ad id: 120247339531520519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247339531520519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4
Landing page: https://go.healthformoms.co/save/

**M007: Moms Nahuel WV#1 - V9 - Copy, on the broken destination.** $1,631.40 for 6 leads at $271.90. 687 link clicks, 63 landing page views, click quality 9.17. The worst ad of the month and the proof that the destination, not the creative, is the cause. Created 2026-08-17.
Facebook ad id: 120247145872230519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872230519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/645496c411d82a546a3e2deada69459c716615ad09f635ca0b978625c2778b37.mp4
Landing page: https://go.healthformoms.co/save/

**M008: Moms Nahuel WV#1 - V9 - Copy, on the working destination.** The identical video file under the "Battle Res" campaign. $403.70 for 21 leads at $19.22. The control side of the destination comparison. Created 2026-08-11.
Facebook ad id: 120247022199760519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247022199760519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/645496c411d82a546a3e2deada69459c716615ad09f635ca0b978625c2778b37.mp4
Landing page: https://www.healthformoms.co/save/

**M009: moms54-3.** $1,280.49 for 43 leads at $29.78, on a 57.02% hook rate, a 13.65% hold rate and an 8.08-second average play time. The newborn hospital-stay opener. Best attention in the account, worst band on cost. Discussed in "What didn't work," Test 2 and open loop 3. Created 2026-08-13.
Facebook ad id: 120247063711860519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063711860519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/5a62b11062812d9509cb2cd8c95e89777a15d1a6ac1cdb1f6e9a92eb77f93a9d.mp4
Landing page: https://www.healthformoms.co/save/

**M010: moms54-2.** $1,463.05 for 42 leads at $34.83, $31.97 CPM. The $6,000-deductible tweet-overlay opener in the Moms54 set. Created 2026-08-13.
Facebook ad id: 120247063459400519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063459400519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/3a3e8a8b9f24c4b0e70dd7e422561de2773ffc4fd2dfdabd358971ca6be65f98.mp4
Landing page: https://www.healthformoms.co/save/

**M011: moms54-4.** $646.44 for 17 leads at $38.03, 52.38% hook rate, 8.62% hold rate, $37.83 CPM. The monkey-bars opener, the most expensive lead in the Moms54 set. Created 2026-08-13.
Facebook ad id: 120247063735970519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063735970519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e3aa685999bf4fde82152827c7fc95489462441238ae397a7e24c3a2f8bd7ddc.mp4
Landing page: https://www.healthformoms.co/save/

**M012: MOMS39 - 2 - V2 - Copy.** $1,351.90 for 72 leads at $18.78, 37.47% hook rate, 5.02% hold rate, 2.48% CTR. Part of the resurrection set in Test 3. Created 2026-08-12. No landing_url returned; destination inferred from an 83.0% landing rate.
Facebook ad id: 120247037227340519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247037227340519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b5709e2fc3c51b32fc818394fcc0d33d94206dccad0c923f953671d48875d937.mp4

**M013: Moms36 - 3 - A - 2 - V4c - Copy.** $597.71 for 30 leads at $19.92, on an 11.29% hold rate and a 9.78-second average play time, the longest watch time in the month. Part of the resurrection set. Created 2026-08-11.
Facebook ad id: 120247022319520519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247022319520519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/fe4ef9c25b9bd439ba7664d9b004e6a952789df99e759dd325e2a638e364cf42.mp4
Landing page: https://www.healthformoms.co/save/

**M014: moms-66-816.** $927.73 for 40 leads at $23.19, 40.48% hook rate, 2.29% hold rate, 1.28% CTR. The calm POV lifestyle set in Test 6. Created 2026-08-18.
Facebook ad id: 120247158621190519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247158621190519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/250176511bd811aeff8642de2f95bc64c7958a90faf13850f42db3d7e7cfa62c.mp4
Landing page: https://www.healthformoms.co/save/

**M015: moms-66-816 - 2.** $138.04 for 4 leads at $34.51 on a 64.13% hook rate, the highest single hook rate in the account this month. Discussed in Test 6. Created 2026-08-18.
Facebook ad id: 120247158822290519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247158822290519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/f5c4eb5609b56151437b8b0158cdbaca37952195ef907194b6acc2487fbcc09f.mp4
Landing page: https://www.healthformoms.co/save/

**M016: moms-65 1a.** $738.56 for 27 leads at $27.35, 32.37% hook rate. The third POV husband variant, and the one in Test 6 that did not clear the bar. Created 2026-08-27.
Facebook ad id: 120247285907980519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247285907980519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/bb071de9e8d0e46ca498a10528b066d07bf324999cb3e1b0d11d83c83592cc67.mp4
Landing page: https://www.healthformoms.co/save/

**M017: moms55-1.** $335.30 for 18 leads at $18.63, 42.58% hook rate. The car-line "insurance math" opener launched 2026-08-28, too young to judge.
Facebook ad id: 120247304910390519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247304910390519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b3ef51c46ea047450eeba20ec707c5b9022d136aa15f90b609da424269526a11.mp4
Landing page: https://www.healthformoms.co/save/

**M018: Moms46 - V1.** July only. $381.82 for 12 leads at $31.82 on a 13.59% hold rate and a 6.77-second average play time, the best hold rate in the July account. The claymation format retired before August. Discussed in Test 7. Created 2026-07-02.
Facebook ad id: 120246046671140519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120246046671140519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0e843f33de6045345de8bafc06819312831ea5db2037b5a0670dc09af3412597.mp4
Landing page: https://www.healthformoms.co/save/

**M019: Moms46 - V2.** July only. $86.06 for 2 leads at $43.03 on an 11.15% hold rate. Second claymation file. Created 2026-07-02.
Facebook ad id: 120246046732760519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120246046732760519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/5658ec375b09b246b0bd732b5c1c7b5eccc7aa5a73358ee66252445be52e38ac.mp4
Landing page: https://www.healthformoms.co/save/

**M020: Moms46 - V3.** July only. $12.63 for zero leads on a 12.58% hold rate. Third claymation file. Created 2026-07-02.
Facebook ad id: 120246046735300519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120246046735300519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/a99ab548d778d98bf1da96a76b070d9fc6075fd5ba130947eb2c4434c758ac48.mp4
Landing page: https://www.healthformoms.co/save/

**M021: moms-67 4#.** The first ad on the new quiz destination, created 2026-09-03, outside the reporting month. $66.77 for zero leads so far. Named in "What we should do next month" as the destination to check on day one.
Facebook ad id: 120247380940680519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247380940680519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/50ac45c62c1386238854a24b156f56f119620062459f1314a7fb3611355040ff.mp4
Landing page: https://quiz.healthformoms.com/2

---

**Brand Context Applied:**

- **What I used:** The brand's own CPL tiers and its two-gate winner definition, its stated best angle and the state-list mechanic, its stated failure of political framing, its Open Enrollment date of November 1 with a two-month planning lead, its stated creative volume of one to five net-new concepts and one to five iterations a month, its named bottlenecks in casting, production and scripting, its five ICPs, and its own words on low creative diversity. The live Meta account for every number, and the August Facebook ad comments as the only voice-of-customer surface this brand has.
- **What I avoided:** ROAS, AOV, purchase value and add-to-cart appear nowhere, per the standing rule for this lead-generation account. No political or partisan framing was recommended, per the brand's stated guardrail. No ad is called a winner on CPL alone, per the team's own two-gate definition. Lead-quality claims are not made anywhere, because Parker cannot see them.
- **Why this fits:** The account is nine weeks out from the single most important date on its calendar, with a two-month planning lead that started three days ago. It has a proven angle, very little creative diversity, and a month of evidence that its cheapest wins came from changing the picture rather than the words. The recommendations aim the September round at footage variety, at the objections its own commenters are raising, and at the broken plumbing that is currently mis-scoring good creative, so that when budget goes back on in November it goes behind ads that were graded fairly.

This is everything I know about Andromeda v2.
