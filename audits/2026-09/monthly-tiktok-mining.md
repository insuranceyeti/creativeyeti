---
brand: health-for-moms
doc: monthly-tiktok-mining
month: 2026-09
generated_on: 2026-09-04
refresh_by: 2026-10-04
data_sources_read: [Parker TikTok mining library via search_tiktok_videos with with_video_report true, brand Meta ad account via audits/2026-09/monthly-hook-audit.md and audits/2026-Q3/90-day-performance-audit.md, source-pulls/ad-comments.md as the labelled substitute for the missing customer review audit, source-pulls/customer-reviews.md, audits/2026-09/monthly-organic-tiktok-audit.md as the sibling read, running-notes/missing-context.md, running-notes/brand-rules.md, BUILD-STATUS.md, brand context document]
knowledge_docs_read: [parker-system/creative-strategy-context/expertise-routing.md, parker-system/creative-strategy-context/adapting-scripts.md, parker-system/creative-strategy-context/hooks.md, parker-system/creative-strategy-context/problem-solution-video-ad-formats.md, parker-system/creative-strategy-context/visuals.md, parker-system/creative-strategy-context/seasonality.md, parker-system/creative-strategy-context/customer-review-mining-method.md]
videos_selected: [10 total, all from the one pool Parker exposes. See the split note below — the five-and-five brand-versus-global constraint could not be met as written, and that is a data limitation rather than a choice]
library_size: 23 videos, 100% of what Parker holds for this brand. 19 Relevant, 2 Potentially Relevant, 2 Not Relevant by Parker's own relevancy pass
prior_report: none. This is the baseline cycle for this doc type
data_limitations:
  - "The five-and-five source split could not be honored, and I am naming it rather than faking it. Parker exposes one TikTok tool, `search_tiktok_videos`, and it requires a `brandId`. It returns the 23 rows scoped to Health For Moms, each joined to a row in the global TikTok report store through `global_report_id`. There is no call that reaches the global store on its own. So the brand pool and the global pool are the same 23 videos seen through one door. All ten entries below come from that pool. The section labels are kept so this doc sits cleanly beside its siblings, and the split I made is stated in plain terms under the heading for the second half."
  - "Views-to-follower ratio cannot be computed for any video. The tool returns `global_author_id` and `global_author_username` but no follower count on any of the 23 rows, and no second call exposes one. The prompt asks for that ratio on every entry. I have substituted the closest honest measure Parker can produce: each video's like, comment, share and save rate against its own views, held against the library's own middle of 83,900 views, a 5.78% like rate and a 1.31% save rate across the 19 Relevant videos. That measures whether a video punched above the pool, not above its creator's baseline, and it is a weaker test. Every entry says which."
  - "There is no customer review audit to anchor selections against, because the brand has no reviews. `search_customer_reviews_sql` returned `totalResults: 0` on an unfiltered run at 30ms today, 2026-09-04, and `search_customer_reviews_semantic` returned `count: 0` and `totalReviewsAnalyzed: 0` at topK 50 with the similarity floor dropped to 0.01, against a collection the tool confirms exists. Post-purchase surveys returned `totalResponsesForBrand: 0` on the same day. So the review-side anchor named in the prompt's required sources is empty. `running-notes/missing-context.md` sanctions Facebook ad comments as the labelled substitute for this brand, and every customer-language anchor below is drawn from the 1,322-comment corpus in `source-pulls/ad-comments.md` and marked as ad comments, never as reviews."
  - "This is not a read of the brand's own organic. Health For Moms runs no TikTok account Parker can see, and `search_and_manage_organic_social` is not in Parker's tool inventory for this brand. Every video below belongs to a stranger. Nothing here is brand organic performance."
  - "The library is a fixed scrape, not a live feed. All 23 videos were ingested on 2026-09-03 from a single keyword set of 18 phrases. Parker cannot run a fresh TikTok keyword, hashtag or handle search from this environment, so the pull could not be widened. Post dates are trustworthy; representativeness of today's feed is not."
  - "View, like, share and save counts are one snapshot taken at scrape time on 2026-09-03. There is no earlier reading, so no growth rate exists and a video posted three days before the scrape is not comparable to one posted ten months before it on equal terms."
  - "No comment bodies are available. Parker holds comment counts on all 23 videos and not one comment text. Comment rate is used as a proxy and it is a weak one."
  - "There is no prior month's TikTok mining report. The audits directory held no file of this type before today, so nothing could be carried forward and no prior adaptation outcome could be closed."
  - "Northbeam is not connected. Every brand performance number quoted below is Meta-reported on the org default attribution window, and this account has zero purchase events by design, so CPL and lead volume are the only valid measures."
  - "There is no `get_current_time` tool on this MCP surface. The 2026-09-04 date comes from the session clock and matches the date stamped on the most recent docs in this build."
  - "Parker's relevancy reasoning on these rows names two ICPs, `Megan` and `Kelsey`, that do not exist in the current brand context document, which names Jen, Danielle, Marissa, Courtney and Nicole. The relevancy scoring appears to have run against an older persona set. No persona claim below rests on relevancy reasoning alone."
---

# Monthly TikTok mining — Health For Moms — 2026-09

This is the baseline pull, and it is a category read rather than a report card. Health For Moms has no organic TikTok account that Parker can see, so the 23 videos in its mining library all belong to strangers talking about health insurance, hospital bills and what it costs to have a baby in America. My sibling doc, `audits/2026-09/monthly-organic-tiktok-audit.md`, already read all 23 at full report depth this cycle and built the niche picture: the hook table, the script transcriptions, the creator demographics, the underperformers. I have not rebuilt any of that. What this doc does instead is the thing the mining prompt actually asks for, which is ten self-contained adaptation entries, each one tied to a specific number, comment or tested ad inside this brand's own ecosystem, and each one read through `adapting-scripts.md` so the reader gets the structural translation rather than a compliment about the video. Where the two docs touch the same video I cite the sibling and go somewhere it did not. Two things shape everything below. The library's attention is anchored hard to pregnancy, and the brand's own comment sections say the product screens pregnant women out, which is the sharpest tension in this month's pull. And the library is seasonal in a way nobody in this build has counted yet: **9 of the 19 Relevant videos, or 47.4%, were posted between October 1 and December 31**, a stretch that is a quarter of the calendar. That matters right now, in September, because the brand's own stated objection list already contains "I should just wait for open enrollment."

## How the ten were chosen, and the split I actually made

The prompt asks for five videos from the brand's TikTok database and five from a global database, and calls the split structural. That split is not available here. `search_tiktok_videos` takes a `brandId` and will not run without one, and every row it returns for this brand carries a `global_report_id` pointing into the same global report store the prompt treats as the second pool. One door, one pool, 23 rows. Rather than dress up an invented second half, I made a split that is real and said what it is. **The first five are the videos that anchor to something the brand has already tested in paid**, so the reader can hold each one against a CPL, a hook rate or a hold rate the account produced. **The second five are the videos whose format the account has never run once**, so that half carries range instead of depth. Both halves come from the same 23 rows and both are labelled honestly.

I ordered inside each half by how usable the reference is, not by view count. `adapting-scripts.md` is blunt that the decision of which content to rewrite "comes down to how easily we believe our solution slots into the script," and view count is the validation on top of that, not the qualifier. Two of the ten sit under 32,000 views and earn their place because the brand can execute them tomorrow.

**On recency.** The prompt says newer wins where two videos are comparable, and I held that where I could, but the library will not fully allow it. Six of my ten were posted before 2026 and the oldest is from October 2024. That is the pool's shape, not a preference: the scrape's own newest Relevant video is a political advocacy ad the brand's compliance rules ban outright. Every entry carries its post date so the reader can weigh it.

---

## Brand database — 1

### The video

**Source label: brand-scoped library, anchored to tested brand evidence.**
Playable file: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7571648042147908894_1788468281/7571648042147908894_join_me_as_i_call_around_and_get_self_pay_pricing_.mp4`
TikTok: `https://www.tiktok.com/@drashleehendry/video/7571648042147908894`
Posted **2025-11-12**.

@drashleehendry. **6,200,000 views, 661,800 likes, 208,000 shares, 22,700 comments, 108,770 saves.** Like rate **10.67%**, share rate **3.36%**, save rate **1.75%**, comment rate **0.37%**. Against the library's 5.78% like and 1.31% save middle, this is roughly double on both. Views-to-follower ratio unavailable, no follower count in any Parker field. `global_is_ad` is recorded as **false**, and the engagement shape backs that up: a boosted post does not carry a 3.36% share rate.

### Why this video is here

The anchor is the account's own hold rate, and it is unusually clean. The brand has already built this format three times and Parker holds the numbers. `MOMS38 - 2 - V3`, in the ad set named "Moms38 - 2 - 1 (when you call your insurance)", produced a **24.48% hold rate, the highest of any ad in the account and more than double the 12% craft floor**, at a **$30.91 CPL**. The two sibling versions held **17.43%** and **9.15%** at **$22.90** and **$16.65** CPLs. Verified, from the sibling audit's cross-check against `search_facebook_ads_sql`. So the brand knows the recorded-call structure grips people harder than anything else it makes, and it also knows the version it has been shipping produces its most expensive leads. This video is the same mechanic executed as documentary rather than as comedy, and it is the largest video in the brand's entire mining library at **66.1% of all 9,376,300 views in the pool**.

The second anchor is a customer objection, and it comes from ad comments rather than reviews because this brand has none. **103 comments out of 1,322, spread across 13 different ads**, are people correcting each other about the difference between a deductible and an out-of-pocket maximum. That spread across 13 ads matters more than the raw count, per the denominator rule in `customer-review-mining-method.md`. What those comments describe is a woman who has been quoted a number she does not understand and cannot verify. This video is ninety percent a woman verifying numbers out loud.

The third anchor is a compliance fact the brand should read as an asset. The brand's guardrails require that a doctor character be a real licensed physician or that the language be adjusted so no false credential is implied. Stated, from the brand context document. Health For Moms already owns a real credential it has never once put on camera: the licensed partner agents every lead is handed to. The sibling audit routed that to the brand as its open loop 8, and I am not re-asking it here.

### Visual breakdown

The frame is the only clinical setting in all 23 videos. Neutral wall, a modern abstract painting, an examination table behind her, bright overhead office light, a practice logo for Mid-South Direct Primary Care sitting in shot the whole time. She is in glasses, a navy medical polo and a white lab coat. The camera is eye level on a desk tripod and never moves for five minutes and thirty-two seconds. Against `visuals.md` principle one, half-second clarity, this frame answers "what is this" instantly, because a lab coat plus a phone call reads as medical business before a single word lands.

The device that carries the whole video is colour. Every price she is told gets written on screen in one of two colours as she hears it. **Red for what is billed, green for the cash or all-in price.** They stack down the left of frame and sit side by side: `SVD (everything) $5,730` in green, then `SVD $2,760` in red against `SVD $2208` in green, then `C-section $3,103` red against `C-section $2,482` green, then `SVD $5,840` red against `SVD $2,244` green. She never says the word expensive. The two colours argue for her. That is `visuals.md` principle two, visual hierarchy, doing real work: the number is primary, her face is secondary, the room is tertiary, and the eye lands in the right place with no effort.

The second visual event is her notebook. She writes each figure down by hand while the person on the phone says it. It is a small thing and it is doing something specific, which is proving the call is live. A quoted price on screen is a claim. A quoted price being handwritten in real time as a stranger reads it aloud is evidence. That is principle six, native context beating polish, inside an otherwise polished frame.

Held against the brand's own account, the gap is stark. **No ad in the Health For Moms library uses colour to make a comparison.** Its proven document ad, the "Approved State List ✔️" creative `moms-53 3`, puts a wall of state names on screen and produced **110 leads at a $16.01 CPL with a 3.15% CTR and a $0.67 CPC**, the highest CTR in the account's top 20. Verified. So the brand has proof that a document on screen converts here. It has never tried a document with two colours arguing inside it.

### Hook analysis

The first line is spoken mid-action, with no setup: *"This is Dr. Ashley Hendry. I was calling to get a quote for a self-pay patient to see what the global vaginal delivery fee would be."* On screen, black on a white box across the top, held for the entire 5:32: `Pregnancy Self pay pricing`. In `hooks.md` terms this is an **Authority hook**, and it is executed the way that doc says to execute one, which is to state the credential plainly and then demonstrate expertise rather than assert it. She uses insider vocabulary in the first sentence, "global fee," and does not stop to explain it. That is the move. The viewer who does not know the term now needs to stay to find out.

The brand's nearest attempt failed at exactly the point this one succeeds. `MOMS30 - 1 - V20` puts a clinician in a lab coat on screen and gives her nothing to say: **39.38% hook rate and a 2.44% hold rate**. Verified. The credential stopped people and then the ad had no credentialed thing for the credential to do. Hendry's hook rate is not measurable, but her 10.67% like rate on 6.2 million views says the opposite happened.

### Script analysis

Run it through `adapting-scripts.md` and the segment map is unusually simple, which is why it is adaptable. Segment one, the credentialed introduction and the ask. Segment two, the first number spoken by the second party. Segment three, the follow-up that will not let the number stand alone: *"Does that cover the hospital facility fee or is that just the OBGYN group fee?"* Segment four, the correction that reframes everything: *"That is the normal price."* Segment five onward, the same three beats repeated with a second hospital. There is no monologue anywhere in it. Every sentence is either a question or an answer from someone else.

The structural rule from Step 5 of that doc is to replace content and never the structure. What replaces cleanly here is the caller and the question. A licensed partner agent calling to check what a family's current plan actually pays on a specific procedure is the same act, the same credential, the same recorded second voice. What does not replace is the payload, since self-pay pricing is not what this brand matches people to. Under Step 6, proof mapping, the compliant substitute for the red-versus-green price comparison is the brand's own approved framing, which is "up to 30%" and "$0 deductible option" rather than a flat guarantee. Step 7 is where a recreation of this will most likely fail. The reference is five and a half minutes of dead air, hold music and slow arithmetic, and the doc is explicit that pacing drift is structural failure. Cutting this to thirty seconds does not make a short version of it. It makes a different video, because the length is the proof.

---

## Brand database — 2

### The video

**Source label: brand-scoped library, anchored to tested brand evidence.**
Playable file: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7584916120965008671_1788468783/7584916120965008671_when_i_was_pregnant_with_my_first_i_missed_out_of_.mp4`
TikTok: `https://www.tiktok.com/@friencine/video/7584916120965008671`
Posted **2025-12-17**.

@friencine. **175,800 views, 25,100 likes, 6,978 shares, 308 comments, 15,858 saves.** Like rate **14.28%**, share rate **3.97%**, save rate **9.02%**, comment rate **0.18%**. All three of those first rates are **the highest of all 23 videos in the library**, on 2.8% of the reach the biggest video holds. Views-to-follower ratio unavailable. Runtime forty-six seconds, the shortest substantial video in the pool.

### Why this video is here

The anchor is the brand's business model, and it is the tightest fit in this month's pull. Health For Moms does not sell a product. It hands a mother's details to a partner insurance agency and an agent calls her. That means the whole business runs on one mother telling another mother, and **the share rate is the closest organic proxy this brand has for its own referral mechanism**. This video out-shares everything in its category at 3.97% and out-saves everything at 9.02%. The sibling audit asked why in its open loop 2 and left it open. I am not re-asking it. I am using it, because the mechanic is visible in the script.

The second anchor is compliance, and it is the single most useful phrase in the library. The brand's rules require hedged financial language, "up to 30%" and "$0 deductible option," never a flat promise. This creator produces a hedge on her own, without being asked, in two words: **"free-ish money."** That is customer language doing a compliance job by accident. Under `customer-review-mining-method.md` it carries three qualifying signals at once, which is well past the candidate threshold: it is a metaphor, it is punchy enough to be a hook as it stands, and it is a comparative claim with the qualifier built into the word.

The third anchor is the account's demonstrated appetite for a strong stated opinion. The brand's second-largest hook family is a Demographic opener stacked onto a myth-busting turn, running **22 distinct video ads, $27,980.64 and 1,156 leads at a $24.20 CPL** lifetime. Verified. So the account already knows a woman saying a flat contrarian thing works here. It has never let her say it as an opinion she will defend.

### Visual breakdown

There is almost nothing in the frame and that is the whole point. A Black woman in her late twenties or early thirties in a patterned head wrap and gold-rimmed glasses, sitting on a bed. Behind her a headboard and a decorative rainbow pillow. Soft daylight from a window. Camera eye level, medium close-up from the chest up, handheld or propped, low fidelity. This is `visuals.md` principle six at its purest, native context beating polish, and it is worth holding against the brand's paid work, where the best-performing creative opens on a mother and baby in white bedding in soft beige light. That is a beautiful frame. It is a different species of image from this one.

The text does two separate jobs and they are worth separating. The hook line, `A HILL I WILL DIE ON A SECOND TIME MOM!`, sits top-centre in bold white with a black outline and holds for the full forty-six seconds. Then at seven seconds a second box appears, white with black sans-serif, reading `Hospital Indemnity Insurance`, and it is doing a labelling job rather than a hook job. It names the unfamiliar term at the exact moment she says it, so the viewer can hold it, remember it or search it. Fourteen of the 19 Relevant videos in this library hold a persistent banner like the first one, and the brand can copy that cheaply.

The visual event is her hands. There is no product, no document, no cutaway and no second location for forty-six seconds. Her facial expression and her gestures are the entire motion budget, and the report notes them as the primary focal point. That is the honest cost of this reference and the brand should know it going in. A talking head with no prop has to be carried by the writing, and `visuals.md` principle two says if the hierarchy is not there you are asking the copy to do the visual's job.

### Hook analysis

Spoken and captioned as one: *"A hill that I will die on as a second-time mom is you need that hospital indemnity insurance."* The mechanic is an unfinished sentence. She tells you she will die on a hill before she tells you what the hill is, and the phrase "second-time mom" qualifies her and filters the audience in the same breath. In `hooks.md` terms that is a **Controversy or Anti-Traditional hook** fused to a **Demographic** filter, and the two stack inside eight words. The audio hook carries no music at all, which the report notes explicitly, so the only sound is a woman's unaccompanied voice in a quiet room. Ten of the 19 Relevant videos in this library share that, which means the format that wins here does not depend on borrowed audio and therefore carries into paid with no licensing problem.

### Script analysis

The segment map under `adapting-scripts.md` is four beats and no more. Segment one, the assertion, which is the hill. Segment two, the reframe as a hack: *"You're basically getting paid to have this baby. You're basically getting paid extra free-ish money to have this baby."* Segment three, the instruction, repeated three times: *"Sign up, just sign up... but get it... Sign up for hospital indemnity insurance."* Segment four, the return to the opening line: *"That is a hill I will strongly stand and die on."*

That closing return is the mechanic most adaptations would drop, and it should not be dropped. Step 4 of the method says do not alter segment order and do not compress, and the bookend is why forty-six seconds feels finished rather than cut short. What transfers to this brand is the shape, the sentence rhythm and the hedge word. What does not transfer is the payload, since hospital indemnity is a different product from what this brand matches people to, so under Step 3's first caveat the adaptation needs the solution segment slotted where segment three currently sits. The brand's own true claim maps onto the reframe beat almost exactly: having insurance is not the same as being covered. Step 8 is where the care goes. The repeated imperative "just sign up" is a flat instruction, and this brand cannot promise an outcome, so the compliant equivalent keeps the urgency in the rhythm and moves the certainty out of the verb.

---

## Brand database — 3

### The video

**Source label: brand-scoped library, anchored to tested brand evidence.**
Playable file: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7616717859724545311_1779072506/7616717859724545311_ive_wanted_to_make_this_video_for_so_long_but_was_.mp4`
TikTok: `https://www.tiktok.com/@kaseyjaneanderson/video/7616717859724545311`
Posted **2026-03-13**.

@kaseyjaneanderson. **872,100 views, 75,400 likes, 12,100 shares, 1,316 comments, 17,993 saves.** Like rate **8.65%**, share rate **1.39%**, save rate **2.06%**, comment rate **0.15%**. Like rate roughly 1.5 times the library middle. Third largest view count in the pool and the largest posted in 2026. Views-to-follower ratio unavailable.

### Why this video is here

The anchor is the account's most expensive lesson. Health For Moms has been building a high-distress lane, and its own numbers argue against it. Six video ads share the line "This is why you cannot settle for mediocre insurance," carrying **$3,423.18 and 103 leads at a $33.23 blended CPL**, with individual ads at **$29.85 and $38.09**. Those same ads posted the account's **highest hook rates at 57.02% and 52.40%**, against the flagship's 45.55%. Verified. So the ads that stop the most people produce the most expensive leads in the account. This video is the counter-example at scale: a confession of something genuinely frightening, delivered completely calmly, at 872,100 views and an 8.65% like rate.

The second anchor is the identity the ad comments keep surfacing. **160 of 1,322 comments, or 12%, across 17 different ads, disclose the commenter's own deductible or premium unprompted.** These are not uninsured shoppers. They already pay. The single most-liked comment in the whole corpus, at 47 likes on 2026-03-22, reads: *"This sounds too good to be true. I pay over $1,000 a month for a premium. We have to pay an $8000 deductible per family member or up to $17,000 for the entire family. It's insane. I have 2 members of the family with chronic diseases. This absolutely insane. I want the 1990's back."* This creator is the mirror image of that woman: she looked at the same arithmetic and walked away from insurance entirely. Ad comments, not reviews, and marked mixed confidence per `source-pulls/ad-comments.md`, because nothing in this brain confirms any commenter bought.

The third anchor is the employer-plan trap, which the brand's creative assumes away. A recurring set of commenters says plainly they cannot switch: *"nope. My job picks the plan that they offer."* on 2026-03-30, and *"Mine is $6k per person too but since it's thru my job I don't really have a choice"* on 2026-03-17. This creator's husband owns his own business and has no benefits, which is the other side of the same wall, and she names it in one line.

### Visual breakdown

A woman in her late twenties or early thirties, long brown hair, ribbed maroon long-sleeve shirt, sitting at a wooden dining table. Behind her a wall of framed family photos and warm soft light, likely a lamp rather than a window. A coffee mug sits at the bottom of frame. The report reads it as a late-night kitchen table conversation, and that is exactly right. `visuals.md` principle four, human presence, is carrying this: her face is the only thing to look at for eighty-eight seconds and the framed photos behind her are quietly doing the credibility work that a caption would otherwise have to claim.

One text block and nothing else: `WE DON'T HAVE HEALTH INSURANCE family of 4`, top centre, bold white serif, held the full runtime. Serif rather than sans, which is unusual in this library and reads slightly editorial. The important structural choice is that it never leaves. A viewer who arrives at second forty still knows what she is watching, which is the same function the persistent banner performs in fourteen of the 19 Relevant videos here.

There is one odd small visual detail worth naming because it is doing real work. She holds a small silver ring or object near her mouth, the way someone holds a microphone, though it makes no sound. The report flags it as a pattern interrupt, and it is: it gives the eye a close-up focal point in an otherwise motionless frame. That is `visuals.md` principle three, pattern interruption without confusion, done with an object that costs nothing.

### Hook analysis

*"We have not had health insurance for three years."* Flat, calm, matter-of-fact, no music. This is a **Controversy or Anti-Traditional hook** in the `hooks.md` sense, and its power is that it breaks a social norm about family safety rather than shouting about a bill. The text hook says the same thing and adds the stake, "family of 4," so the sound-off viewer gets both halves.

The reason this belongs in front of this brand right now is the shape of the delivery, not the content. Sort the account's own openers by temperature and the split is clean: the calm ones delivered CPLs of **$13.29, $15.14, $16.01, $19.52, $21.56 and $24.45**, and the high-distress ones delivered **$29.85, $34.94 and $38.09**. Verified. Not one of the 19 Relevant videos in this library opens on crying. Two independent sources, the brand's own CPL data and an unrelated organic feed, pointing the same direction.

### Script analysis

The `adapting-scripts.md` segment map is a clean six. Segment one, the confession. Segment two, the reason, which reframes the confession as a choice rather than a failure: *"This is the reason why I can be a stay-at-home mom."* Segment three, the credential, and it arrives late on purpose: *"Prior to having kids, I was a nurse. I had the big benefits."* Segment four, the sacrifice, in a rhythm of repeated verbs: *"And so we sacrificed. We sacrificed the benefits, we sacrificed the big paychecks."* Segment five, the objection she raises against herself: *"The biggest question people have is like, 'What about an accident?'"* Segment six, the solution and the sign-off.

Two mechanics carry over and one does not. The credential placed at segment three rather than segment one is the sharper of the two, because it means the viewer has already decided she is reckless before learning she is a nurse, and the correction lands harder for having been delayed. The self-raised objection at segment five is the other, and it maps directly onto this brand's own stated objection list, which includes "Is this legit?" and "I don't want to get on a call and be sold to." What does not carry is her ending, which is a plug for a specific health-sharing group. Under Step 6 the compliant substitute is the brand's own match-and-consult step in the same structural position, not a name-drop.

---

## Brand database — 4

### The video

**Source label: brand-scoped library, anchored to tested brand evidence.**
Playable file: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7593050209676987662_1777257347/7593050209676987662_if_you_have_health_insurance_they_may_cover_matern.mp4`
TikTok: `https://www.tiktok.com/@paumod/video/7593050209676987662`
Posted **2026-01-08**.

@paumod. **916,200 views, 81,400 likes, 20,400 shares, 599 comments, 52,376 saves.** Like rate **8.88%**, share rate **2.23%**, save rate **5.72%**, comment rate **0.07%**. The save rate is **the second highest in the library** and more than four times the 1.31% middle. Second largest view count in the pool. Views-to-follower ratio unavailable.

### Why this video is here

The anchor is a documented gap in the brand's own funnel, and it is the most consequential thing in this month's pull. **The brand's ad library returns zero matches for the word "pregnant" across every ad name, headline, body copy, text hook, verbal hook, visual hook, angle, creator description, script and AI analysis field, lifetime, all ad types.** Verified. Meanwhile 12 of the 19 Relevant videos in this library are anchored to pregnancy, delivery or a baby's first year, and this one is the second largest of them. So the category's attention is concentrated somewhere the account has never spoken.

The second anchor is what makes that gap complicated rather than simply an opportunity, and it is the reason this entry is here rather than a simpler pregnancy video. **42 comments across 15 different ads over 14 months are women saying they were told they do not qualify because they are pregnant or planning to be.** *"Health for Moms, but only if your babies are out of the womb. I was denied for being pregnant. Scam."* on 2026-02-03. *"Health care for moms but you don't qualify if your pregnant? Make that make sense."* on 2026-05-05. *"How can you have healthcare for moms if you don't cover maternity? Makes zero sense. False advertising."* on 2025-08-12. Ad comments, mixed confidence. The brand's own stated objection list, which names five objections, does not contain this one at all.

Which is exactly why this specific video is the right reference and most pregnancy videos in this library are not. **It is not aimed at getting pregnant women covered. It is aimed at women who already have coverage and do not know what it pays for.** That audience is inside the brand's product envelope, it is the 12% of the comment corpus who already have a plan and are angry about it, and the brand's guardrail against pregnancy-only targeting does not touch it. Stated guardrail: "No pregnancy-only targeting — focus on moms with kids, not expectant mothers exclusively."

### Visual breakdown

A woman in her late twenties or early thirties in a cream fleece zip-up with gold jewellery, in a living room with daylight through blinds behind her. The background is slightly out of focus and clean. Selfie-style handheld at eye level with visible minor shake, and the report reads the shake as part of the credibility rather than a flaw. Direct eye contact with the lens throughout, which is `visuals.md` principle four working at its strongest setting.

One high-contrast text block dominates the centre of frame for the full seventy-three seconds: `PSA IF YOU'RE PREGNANT do this before you start shopping`. Two type treatments in one block, serif and sans mixed. It is doing three jobs at once, which is why the video holds: it names the audience, it makes a promise, and it stakes an urgency claim with the word "before." Then at fifty-four seconds a single second overlay appears, `AEROFLOWBREASTPUMPS.COM`, and it is the only other thing on screen for the entire video.

**There is no product, no document, no cutaway and no demonstration anywhere in it.** She lists breast pumps, milk storage bags, compression socks and a belly band and shows none of them. That is worth sitting with, because it runs against the strongest visual pattern in this whole library, which is the document on screen. Six of the 19 Relevant videos put a real bill or screen in frame. This one, at the second highest view count and the second highest save rate in the pool, shows nothing at all. What is holding the viewer is not the visual, it is the promise in the banner and the running list of specific dollar-saving items in the audio. The lesson for the brand is precise: when the payload is a checklist of things the viewer might get for free, the list itself is the visual event, and the banner has to carry the frame alone.

### Hook analysis

Spoken: *"If you're watching this and you're pregnant, don't shop for anything until you call your health insurance."* On screen at the same moment, the PSA banner. In `hooks.md` terms this is a **Demographic hook** fused to a direct command, with a **Trigger Word** doing the framing, and the trigger word is "PSA." That word is worth naming on its own because it recasts a sales message as a public service announcement, which is precisely the register a brand with a trust problem in this category needs. No background music, so it lands as a personal message rather than a produced asset.

The brand has tested the trigger-word move and knows what it costs. `Moms43 - 5 - V1` runs on the word "hack" and produced **243 leads at a $27.72 CPL on a 38.91% hook rate and an 8.05% hold rate**, with the highest CPM among the account's big spenders at **$33.23** against a $23.64 average. Verified. So the trigger word stops people here and the read from that ad is that the cost problem sat in delivery rather than in the opener.

### Script analysis

Under `adapting-scripts.md` this is a **How To or Steps** structure in the `problem-solution-video-ad-formats.md` taxonomy, and its segment map is a hook, a personal mistake, four itemised payoffs, a tool and a sign-off. The four payoffs are the engine and they follow one rule: **each carries a specific number or a specific product name.** *"My insurance covered 70% of it, I think I paid maybe 30, 40 dollars out of pocket."* Then *"My insurance sent me a hundred a month, more than I could ever get through, 100% covered."* Then compression socks, 100% covered. Then a belly band, covered. The percentages descend in specificity and rise in generosity, and the pacing gets faster as the list runs, which is what stops seventy-three seconds of talking from sagging.

The hedge is the part a compliance-bound brand should copy word for word in shape. *"Every health insurance is different, yours may not cover anything at all but it's worth a quick check."* She undercuts her own promise and the video still holds a 5.72% save rate. That is direct evidence that a hedge does not cost you the save in this category, which matters enormously for a brand whose rules force "up to 30%" rather than a flat number. Under Step 6 of the method, the brand-safe proof swap here is straightforward: the itemised payoffs become the specific things the brand's own approved claims cover, and the third-party website in the final beat becomes the brand's match step in the same structural slot. Step 7 is the risk. The reference is a fast list, and slowing it to explain the brand's model would be pacing drift.

---

## Brand database — 5

### The video

**Source label: brand-scoped library, anchored to tested brand evidence.**
Playable file: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7536693373290270007_1788469019/7536693373290270007_revealing_how_much_i_pay_for_my_monthly_doctor_vis.mp4`
TikTok: `https://www.tiktok.com/@asap.kristy/video/7536693373290270007`
Posted **2025-08-09**.

@asap.kristy. **120,200 views, 8,560 likes, 40 shares, 59 comments, 228 saves.** Like rate **7.12%**, above the 5.78% middle. Share rate **0.03%** and save rate **0.19%**, both near the bottom of the pool. Views-to-follower ratio unavailable. The oldest video in the first half at roughly thirteen months, and included because the mechanic it demonstrates is the cheapest thing on this list to build.

### Why this video is here

The anchor is the cheapest lead the account has ever bought with a document on screen, and the mechanic matches almost exactly. The `moms-53 3` state-list ad produced **110 leads at a $16.01 CPL with a 3.15% CTR and a $0.67 CPC**, the best CTR in the account's top 20, and its entire visual event is a document on screen that the viewer scans for her own information. Verified. The screenshot-overlay family does a version of the same thing: `MOMS39 - 2 - V2` has spent **$27,775.42 lifetime for 1,213 leads at a $22.90 CPL on a 40.62% hook rate**, and the copy running in the recent window landed a **$19.18 CPL**. Verified. So a document in frame is proven twice in this account. This video is the two-number version of it, which is the one variant the brand has never built.

The second anchor is the shape of the objection the brand's comment corpus keeps producing. The deductible correction runs to **103 comments across 13 ads**. What those women are arguing about is the gap between a number they were quoted and a number they actually paid. This video puts both numbers on screen nine seconds apart and lets the gap be the entire argument. Under `customer-review-mining-method.md` that is a whole-review concept rather than a nugget: the structure itself is the asset.

The third anchor is honest and it cuts the other way. **This video's payload is that employer insurance is worth having.** Her conclusion is *"That is why it's so important to have insurance."* That is not a message this brand can run as written, because a large share of its audience is the employer-plan captive who already has that insurance and is drowning under it. The reference is a structural one, not a messaging one, and the entry would be dishonest if it pretended otherwise.

### Visual breakdown

The driver's seat of a clean modern car in bright natural daylight. A woman of Asian descent in her mid twenties, glasses, long dark wavy hair, white off-the-shoulder sweater. The white sweater against the dark car interior is doing genuine contrast work and keeps her face as the primary focal point with no lighting setup at all. The car is a repeatable choice rather than an accident: three separate creators in this library film from a driver's seat in daylight, and the reports read it the same way each time, as a quick thought shared during a busy day.

The two overlays are the whole video. At thirty-two seconds a screenshot of a bill summary reading `Amount Billed $1,100.00`. Then at forty-one seconds, nine seconds later, a second screenshot reading `What I Owe $28.11`. Two real screens, held briefly, sitting in the same frame position. Under `visuals.md` principle one that pair passes the half-second test in a way a spoken sentence never can, because the reader gets both numbers and the size of the gap before understanding a word of context.

Two persistent text blocks run above them. `IM CURRENTLY 5 MONTHS PREGNANT SO HERES HOW MUCH I PAY FOR MY MONTHLY DOCTOR VISITS` holds top centre for the full 1:06. Then from nineteen seconds a second block sits middle-left: `I fortunately have insurance through my employer so I pay $90 roughly per month for medical, dental, and vision`. That second block is the qualifier, and putting a qualifier on screen rather than only in the audio is a move a compliance-bound brand should note, because it means the caveat survives the sound being off.

### Hook analysis

*"As you all know I am currently pregnant so I wanted to share with you guys exactly how much I'm currently paying for my monthly doctor visits."* This is a **Storytelling hook** in the `hooks.md` taxonomy, opened with a life update and closed with a curiosity gap, and the phrase "as you all know" is doing something specific: it assumes a prior relationship with the viewer that does not exist. That assumed familiarity is a cheap and reliable way to make a cold viewer feel like a returning one, and it costs nothing to write. The word "exactly" is the load-bearing one, because it promises a number rather than a story about a number.

### Script analysis

The `adapting-scripts.md` segment map is five: the setup, the itemisation of what the visit includes, the qualifier about her employer plan, the two-number reveal, and the gratitude close. The critical structural fact is where the qualifier sits. It comes **before** the reveal, not after. She tells you she pays $90 a month and has already hit her deductible, and only then shows you $1,100 against $28.11. Reversing those two beats would make the reveal feel like a trick. Keeping the order makes it feel like arithmetic.

Under Step 5, what replaces here is only the numbers and the caveat, and this is where the brand's compliance envelope actually helps rather than hinders. The brand cannot show a customer's bill, because it has no customers whose bills it holds and no review corpus to draw a real one from. What it can show, under the Data Integrity rule in `problem-solution-video-ad-formats.md`, is a figure it has already approved, and anything it has not approved stays a flagged placeholder rather than an invented number. Step 7's pacing note matters too: the nine seconds between the two screenshots is the tension, and closing that gap to a snappy two-second cut removes the only suspense the video has.

---

## Global database — 1

**A standing note for this second half.** These five come from the same 23-row pool as the first five, because as recorded in the frontmatter Parker exposes no separate global TikTok query. What separates them is stated and real: **the brand's paid account has never once run the format each of these demonstrates.** Comment Response, faceless, green screen and the question with no answer all sit on the brand's own untested-format list, and the second task is a device no ad in the account uses. So this half carries range rather than depth, and every entry names the untested format it proves in category.

### The video

**Source label: brand-scoped library, format the account has never run.**
Playable file: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7572985864435879181_1788468482/7572985864435879181_selfpaynoinsurance_emergencyroom.mp4`
TikTok: `https://www.tiktok.com/@readra21/video/7572985864435879181`
Posted **2025-11-15**.

@readra21. **213,100 views, 3,807 likes, 246 shares, 97 comments, 124 saves.** Like rate **1.79%**, second lowest in the library. Save rate **0.06%**, the lowest of all 23. Views-to-follower ratio unavailable. Fifteen seconds long. **This is the second largest recent view count in the pool attached to the weakest engagement in it**, and that split is the reason it is here.

### Why this video is here

The anchor is a named gap on the brand's own list. Faceless "Ugly Ads" sits at number nine on the brand's untested formats. Stated. **Every ad inspected in this account has a person in frame.** This is a proven in-category faceless execution at 213,100 views, and it is proven with a caveat the brand needs to carry: it reached a lot of people and moved almost none of them. Under `visuals.md` principle four, human presence drives trust and attention, and a fifteen-second video with no face and the library's lowest save rate is a fairly clean demonstration of what principle four costs when you ignore it.

The second anchor is the strongest visual pattern in the whole library, and this video is its purest form. Six of the 19 Relevant videos put a real document in frame and let it carry the message. The brand has tested that device and it produced a **$16.01 CPL on `moms-53 3`**, against a $22.10 account average in the same window. Verified. What the brand has never tested is a **bill**, and this is the reference for one.

The third anchor is a compliance conflict I am flagging rather than burying. Parker's own relevancy note on this row records that the video argues a high-deductible plan can be a good idea, which runs directly against the brand's "$0 deductible option" claim. The structure is liftable. The argument is not.

### Visual breakdown

There is no person anywhere in it. A handheld phone, held top-down, over a real multi-page itemised medical bill lying on a flat surface under bright even light. The camera pans slowly down the document, tracking the way a reader's eye moves down a column. That pan is the only motion in the video and it is doing the whole job.

The document's printed column headers are the only text on screen, and there are no overlays at all: `CHARGES`, `ADJUSTMENTS`, `PAYMENT RECEIVED`, `BALANCE`, `BALANCE YOU OWE NOW`. Then the three numbers the video exists for: **total charges of $55,623.00, an adjustment of minus $54,219.00, and a final balance you owe now of $1,404.00.** Under `visuals.md` principle two the hierarchy here is created by the pan rather than by scale, because the eye is given no choice about the order it reads in.

What is missing is the reason it underperformed, and naming it is the most useful thing this entry does. There is no text hook, no overlay, no banner and no face. A viewer who scrolls in at second six sees a piece of paper and has no idea what she is watching or why. Principle one, half-second clarity, fails outright. So the correct read for the brand is not "faceless does not work," it is "faceless without a banner does not work," and fourteen of the 19 Relevant videos in this library carry the banner this one lacks.

### Hook analysis

*"You ever wonder why we don't want insurance?"* spoken by an unseen woman in her thirties or forties in a flat, slightly disgruntled tone. This is a **Question hook** in the `hooks.md` taxonomy layered on a controversial premise, and the visual hook underneath it is the top-down document. The text hook field on the report is empty, which is the failure. This account already knows what a text hook is worth here: `moms55-1` runs an **85.86% first-frame retention** on a **42.58% hook rate**. Verified. That retention comes from something legible in frame zero.

### Script analysis

Four sentences and fifteen seconds, which makes this the most compressed reference in the library. *"You ever wonder why we don't want insurance? Here's our bill prior. And here's our bill cash pay. This is why the insurance companies need to be out."* Under `adapting-scripts.md` the segment map is three: question, comparison, verdict. Not a beat more.

The whole mechanic is the comparison in segment two, and it is a **Before / After Contrast** in the `problem-solution-video-ad-formats.md` taxonomy applied to two numbers rather than two photographs. Step 5's replacement is clean: the two numbers become two numbers this brand can actually stand behind, and Step 6's proof mapping says use an approved observable figure rather than a dramatised one. Segment three is where the brand must diverge. "This is why the insurance companies need to be out" is a political verdict and the brand's rules ban partisan framing outright, with the team stating plainly that political content does not work for them. Under the substitution library in `adapting-scripts.md`, controversy gets replaced with curiosity, so the verdict beat becomes a question that hands the viewer somewhere to go rather than someone to blame. And the fix this reference most needs is additive rather than substitutive: it needs a banner in frame zero, because without one the brand would be buying the same 1.79% like rate.

---

## Global database — 2

### The video

**Source label: brand-scoped library, format the account has never run.**
Playable file: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7611735950615498014_1788469122/7611735950615498014_how_much_did_you_pay_for_your_delivery_i_had_a_won.mp4`
TikTok: `https://www.tiktok.com/@dannitangie/video/7611735950615498014`
Posted **2026-02-28**.

@dannitangie. **28,200 views, 945 likes, 380 shares, 76 comments, 147 saves.** Like rate **3.35%**, save rate **0.52%**, share rate **1.35%**, comment rate **0.27%**. Below the library middle on likes and saves, above it on shares. Views-to-follower ratio unavailable. Small reach, and it is here for the mechanic rather than the numbers.

### Why this video is here

The anchor is another named gap. Green Screen sits at number ten on the brand's untested format list. Stated. This is the format executed in category, on the exact subject matter the brand sells against, by a creator who is inside the brand's stated audience.

The second anchor is the same deductible confusion the comment corpus keeps producing, **103 comments across 13 ads**, and this video is the fullest answer to it anywhere in the library. It does not explain the difference between a deductible and an out-of-pocket maximum. It shows four real documents in a row and does arithmetic on a phone calculator until the number is settled. That is a demonstration rather than a claim, which is what `visuals.md` says survives the sound being off.

The third anchor is the brand's proven document device, and this entry extends it in the direction the brand has not taken. `moms-53 3` proved one document on screen at **$16.01 CPL**. This reference is four documents in sequence, each replacing the last behind the same speaker, which is a materially different production ask and a much cheaper one than a shoot with props.

### Visual breakdown

A woman in her late twenties or early thirties, long dark hair, floral loungewear, bright even light from a ring light or a large window. She is standing in front of a green screen and the background cycles through four things while she stays put.

The sequence is the reference. From sixteen to thirty-four seconds, a hospital bill showing `Total Charges $40,789.94` and `Balance Due $1,925.38`. From thirty-five to fifty-four seconds, an anaesthesia bill showing `Total billed $10,000` and `Total due $1,139.29`. From fifty-five seconds to 1:10, the baby's own hospital bill, `Billed $523.00` and `Outstanding balance $132.03`. Then from 1:11 to 1:42, an iPhone calculator app with the arithmetic visible on screen: `1,952.38 + 132.03 + 1,139.29 = 3,223.7`. The documents are real, from Orlando Health with Blue Cross Blue Shield details visible.

Two things about that make it a strong reference. First, she points at the numbers while she talks, so the viewer's eye is directed rather than left to hunt, which is `visuals.md` principle two done with a hand instead of a layout. Second, the calculator is the payoff frame, and it is a phone doing ordinary arithmetic rather than a designed graphic. That reads as someone working it out rather than someone presenting a conclusion, and it is the single cheapest credibility device in this whole library.

The opening banner is the only overlay: `How much does it cost to have a baby in the US with insurance?`, centre, bold white, held for the first fifteen seconds before the documents take over. That is a different banner strategy from the persistent one most of this library uses, and it works here because the documents themselves become the visual anchor once the banner leaves.

### Hook analysis

*"I just had a baby four months ago and while I was pregnant I was always wondering like how much is this going to cost?"* A **Storytelling hook** opening into a curiosity gap, with the banner asking the question in plain search-friendly language over the top. No music. The report notes her direct eye contact against a formal hospital bill already visible behind her, so the credibility artefact is in frame before the first sentence finishes.

The word doing the most work arrives at second sixteen, not second zero: *"the first bill is definitely a jumpscare when it comes into the mail."* Jumpscare is a metaphor and it is the kind of phrase `customer-review-mining-method.md` flags as a top-priority signal, because a customer reaching for an image rather than a description is where lift-able language lives. The brand has no review corpus to mine for language like that, which makes the category feed one of the few places it can find any.

### Script analysis

The segment map under `adapting-scripts.md` is a **Timeline Ad** in the `problem-solution-video-ad-formats.md` taxonomy, built as five beats: the question, then three bills in ascending surprise, then the sum. The third bill is the structural surprise and it is why the video works: *"what I didn't realize is that you also get billed for the baby. Like the baby gets billed and they send it to you."* That beat exists purely to reset the viewer's assumption at the two-thirds mark, which is exactly where a list video normally loses people.

Under Step 5, the replacement for this brand is a swap of the documents and nothing else. Step 4 says do not alter segment order, and the ascending order here is load-bearing, since running the largest bill last would make the baby beat an anticlimax. The honest constraint is Step 6, proof mapping, and it is a hard one. **The brand has no real customer bill to put on that green screen**, because it has zero reviews, zero surveys and no order data, and `problem-solution-video-ad-formats.md` is explicit that a statistic must come from the brand context document, a real pulled review, an ad comment, or data the user supplied, with a flagged placeholder rather than an invention where none exists. What the brand does hold is 1,322 ad comments containing women's own self-reported figures. Using one of those as the on-screen artefact, labelled as a real comment rather than dressed as a customer, is the compliant version of this reference. Her closing line points at the same place: *"Let me know if that's around the ballpark of what you paid when you had your baby or if I need new insurance."*

---

## Global database — 3

### The video

**Source label: brand-scoped library, format the account has never run.**
Playable file: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7431177503483415839_1788468595/7431177503483415839_replying_to_madratterr_the_affordable_care_act_mad.mp4`
TikTok: `https://www.tiktok.com/@adulting_with_kim/video/7431177503483415839`
Posted **2024-10-29**.

@adulting_with_kim. **25,500 views, 309 likes, 53 shares, 126 comments, 147 saves.** Like rate **1.21%, the lowest in the entire library.** Comment rate **0.49%**, fourth highest. Save rate **0.58%**. Views-to-follower ratio unavailable. The oldest video in this doc at roughly twenty-two months, and the inversion between its like rate and its comment rate is the finding.

### Why this video is here

The anchor is the brand's own richest untapped asset. Comment Response sits at number seven on the untested format list. Stated. And `running-notes/missing-context.md` names Facebook ad comments as one of this brand's few live and rich evidence surfaces. **The brand holds 1,322 real comments on 112 ad IDs, dated 2025-01-08 through 2026-09-03, and has never once put one of them on screen as a hook.** The raw material for this format already exists in a place Parker can read today.

The second anchor is what that like-to-comment inversion means for a lead-generation account. This video earned the least admiration in the library and close to the most replies. **For an account selling a form fill rather than a product, a reply is structurally nearer to the thing being bought than a like is.** That reframing matters, because judged on likes this is the worst video in the pool and judged on the action the brand actually wants it is near the top.

The third anchor is casting, and it is the one thing this creator supplies that nothing else in the library does. **She is the only creator across all 23 videos who reads as over 40.** The brand's own account puts **30.4% of the "I wish this was a joke" family's spend on women aged 45-54 and 9.3% on 55-64**, against 14.3% and 3.6% for the account overall, and that family holds a **15.17% lifetime hold rate**, the best attention in the account. Verified. So the account has found an older woman that this feed almost never contains, and this is its single casting reference for her.

### Visual breakdown

The driver's seat of a clean car with white leather upholstery in bright high-key light. A blonde woman in her late thirties or early forties in a green tank top and a simple silver necklace. Static medium close-up, eye level, dashboard-mounted or held. The car reads as professional competence without a studio, and the report notes the interior as a subtle cue for reliability.

The visual hook is one element and it is the entire format: **a TikTok comment sticker pinned top-left for the full sixty seconds**, quoting a real viewer verbatim. `I've been out of insurance for a year because I can't afford it out of pocket and don't qualify for Medicaid`. It never leaves the frame. Underneath, standard auto-generated captions run along the bottom.

That persistence is the mechanic worth naming, because it is what separates a comment-response ad from a video that happens to mention a comment. The sticker is the topic banner, the credibility artefact and the hook all at once. A viewer arriving at second forty reads a stranger's problem before she hears a word of the answer, and under `visuals.md` principle five, emotional specificity, that stranger's sentence is doing something a brand-written headline structurally cannot: it names a specific stuck state in the viewer's own register.

The rest of the frame is hands. No product, no document, no cutaway. Her gestures carry the visual energy across a static shot for a full minute, which is the same constraint @friencine works under and the same solution.

### Hook analysis

*"I am shocked how many people are in your exact situation."* This is the textbook **Comment Response hook** from `hooks.md`, and the reason it works is that the comment does the stop and the response does the qualify. The word "your" is the hinge. She is answering one person by name, which is why every other person in the same situation leans in.

There is a second, quieter mechanic in that opening line that the brand should note. She does not open with the solution or with empathy for the individual. She opens by telling the commenter she is not alone, which converts a private embarrassment into a shared condition in eight words. For a category where the brand's own comment sections are full of women disclosing five-figure deductibles to strangers, that move is well matched to the audience.

### Script analysis

The `adapting-scripts.md` segment map is five: the empathy open, the correction of a misconception, the mechanism, the proof, and the call to comment. The proof beat is the strongest thing in the script and it is a single concrete case rather than a statistic: *"A lot of people think 'Well, my income is too high, I'm not gonna qualify for a subsidy.' And that's not true either. I just got a family of three with two working parents a zero premium on their health insurance."*

Under Step 6 that beat is exactly where this brand hits its wall, and the wall is worth stating plainly rather than working around. The payload is a government subsidy programme, and the brand's compliance rules ban government and marketplace references outright, with "ACA" on the list of words never used in creative. So the mechanism beat cannot be lifted. What can be lifted is the shape of the correction, and the brand already has its own version sitting in its comment sections. **16 comments across 7 ads are women politely asking whether they still count as a mom if their children are grown**, including *"What if your kids are over 18, do I still qualify as a Mom?"* on 2026-04-29 and *"What about moms with adult children or children in college?"* on 2026-04-21. That is a real misconception, asked in the customer's own words, and answering it on screen is the compliant version of this exact structure. Step 8's tone note applies to the close: her call to action is "comment and I'll be in touch," which reads as a continuation of a conversation rather than a pitch, and the brand's own stated objection "I don't want to get on a call and be sold to" says that register is the one its audience is asking for.

---

## Global database — 4

### The video

**Source label: brand-scoped library, format the account has never run.**
Playable file: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7567018980993469710_1773512819/7567018980993469710_ever_heard_of_indemnity_insurance_for_moms_its_the.mp4`
TikTok: `https://www.tiktok.com/@kclairemoore/video/7567018980993469710`
Posted **2025-10-30**.

@kclairemoore. **131,200 views, 5,725 likes, 945 shares, 63 comments, 2,938 saves.** Like rate **4.36%**, save rate **2.24%**, share rate **0.72%**, comment rate **0.05%**. Save rate roughly 1.7 times the library middle on a two-minute runtime, which is the number that matters here. Views-to-follower ratio unavailable.

### Why this video is here

The anchor is a problem the account has and has not solved: it cannot hold anyone. **The account's average hold rates sit far below the 12% craft floor**, with the flagship `Moms43 - 4 - V3` at a **3.30% hold** on a 45.55% hook rate and **618 leads at a $24.45 CPL**, and the permission-style opener `moms-66-816` at a **2.30% hold**, the lowest in the top 20. Verified. Meanwhile this creator runs **two minutes and two seconds** of dense financial detail and holds a save rate 1.7 times the library middle. The device she uses to buy that time is one the brand has never once tried.

The second anchor is the brand's own audience shape. Delivery in the recent window ran **94.9% female, 43.8% aged 35-44, 35.7% aged 25-34, 99.4% mobile**. Verified. A woman doing her makeup in a bathroom with a baby in a bouncer behind her is a frame that audience recognises without being told what it is, and `visuals.md` principle six says that recognition is worth more than production value.

The third anchor is the language. The account's biggest hook family is the POV husband opener, **20 ads, $87,991.09 and 4,499 leads at a $19.56 blended CPL**, and it works by staging a conversation between a wife and her husband. Verified. This creator's closing line is *"happy baby making. Happy babies. Bye!"*, which is a register no ad in this account has ever used and which sits close to the one the account's biggest winner already runs on.

### Visual breakdown

A bathroom with white tile and a glass shower door. A woman in her late twenties or early thirties in a tan button-down with a small gold necklace, eye level on a tripod or leaned against a vanity. **A baby is visible in a bouncer in the bottom-left corner of frame for the whole video.** That baby is not decoration. The report reads it as proof of life, and it is: it validates her claim to speak on this subject without her ever having to state a credential.

The device that makes the two minutes work is **the second task**. She is applying makeup throughout, cycling through a mascara wand, bronzer and brushes. The report names the function precisely, which is that the secondary activity gives the eye somewhere easy to rest while the ear processes dense financial information. `hooks.md` puts the same rule plainly: when the message is mechanical and informational, the visual has to be simple and give the eye somewhere to go. One other creator in this library uses the identical device, pouring coffee while reading out paycheck deductions, and both videos run well over a minute on numbers and both hold.

The text plan is two overlays and no more. `HAVING A BABY IN 2026` sits centre in bold black on a white rectangle for the full 2:02, functioning as an audience filter with a date built into it. Then from fifteen to twenty-three seconds a small white sans-serif line, `Indemnity Insurance`, appears at the exact moment she says the term. Same two-tier structure as @friencine, a persistent filter plus a timed label for the unfamiliar word, and it appears to be the library's default solution for teaching a term the viewer does not know.

### Hook analysis

*"Stop scrolling if you're having a baby in 2026 because I have ways to save you money."* A **Demographic hook** fused to a direct command, with the date acting as a second filter on top of the first. In `hooks.md` terms the command "stop scrolling" is doing the notice job and "if you're having a baby in 2026" is doing the qualify job, and stacking them means the video pays no attention tax on viewers it cannot serve. Her tone is energetic and conspiratorial, described as sharing a secret with a friend.

Worth noting against this brand's own data: the visual hook is her holding a mascara wand and looking into the lens, which signals a get-ready-with-me video before it signals an insurance video. That is `visuals.md` principle three, a pattern interrupt that stays native, and it is the opposite of what the brand's polished creative does in frame zero.

### Script analysis

Under `adapting-scripts.md` this is a **UGC** structure with a **Testimonial or First-Person Story** spine, and the segment map runs seven beats: the command, the discovery credited to another creator, the term, the mechanism, the outcome, the contrast with her first child, and the sign-off. The contrast beat at position six is the strongest and it is a from-state and to-state pair in the sense `customer-review-mining-method.md` means: *"I just paid off my first child who's three because I was on a payment plan because it was so expensive. And um now I can just send that and pay Riggan off super fast."* Two children, two outcomes, one sentence.

The beat the brand should copy hardest is the second one, and it is the least obvious. She credits where she learned it: *"I came across a TikTok which I wish I could find the girl in 2024 when I was pregnant."* She then says a version of it twice more, *"I feel like nobody talks about it and I had no idea what it was"* and *"I gotta come spread the word."* That is word-of-mouth language, which `customer-review-mining-method.md` names as a qualifying signal that maps directly onto ads mirroring the real buyer journey. For a brand whose entire model is one mother telling another mother, and which currently has no customer it can quote, a creator explaining that she is passing along something she was told is the closest structural match to its own business in this entire library. Under Step 6 the payload swaps to the brand's approved claims and under Step 7 the two-minute pacing has to survive, because the length is what the second task was buying.

---

## Global database — 5

### The video

**Source label: brand-scoped library, format the account has never run.**
Playable file: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7576033059330329886_1788468277/7576033059330329886_are_we_not_living_in_the_same_economy_childlessmil.mp4`
TikTok: `https://www.tiktok.com/@molly_daw/video/7576033059330329886`
Posted **2025-11-23**.

@molly_daw. **31,200 views, 999 likes, 30 shares, 557 comments, 49 saves.** Like rate **3.20%**. **Comment rate 1.79%, tied for the highest in the entire library and roughly twelve times its typical rate.** Share rate 0.10%, save rate 0.16%, both near the floor. Views-to-follower ratio unavailable. Eighteen seconds long.

### Why this video is here

The anchor is what this account is actually buying. It is a lead-generation account with **zero purchase events by design, 4,336 leads at a $22.67 CPL over 90 days**. Verified. A reply is the closest free behaviour to a form fill, and this video generated 557 of them from 31,200 views by offering absolutely nothing. Eighteen seconds, one question, no answer, no product, no next step.

The second anchor is a surprise the sibling audit did not name, and it is the reason this entry earns a slot rather than being a repeat. **This creator is not a mom.** The hashtags on the row are `childlessmillennial`, `millennials`, `dink`, `millennialsoftiktok` and `middleclass`. She is a married woman doing the arithmetic on whether she can afford to become a mother at all, and she produced the highest-conversation video in a library scraped specifically for mom-and-insurance keywords. The brand targets moms exclusively. Its five stated ICPs are Jen, Danielle, Marissa, Courtney and Nicole, and every one of them already has children.

The third anchor is the register. The account's own data says calm openers produce its cheapest leads at **$13.29 to $16.01** and its high-distress openers produce its most expensive at **$29.85 to $38.09**. Verified. This video is exhausted rather than distressed, which is a third register the account has not tested, and it sits between the two the account already knows.

### Visual breakdown

A woman in her late twenties or early thirties, hair pulled back, in a blue and white tie-dye sweatshirt, sitting on a neutral couch. A large round wall mirror behind her, warm indoor light. Handheld, eye level, medium close-up, with visible shake.

**Her hand is resting on her head.** That is the entire visual hook and it arrives before she speaks. The report reads it as exhaustion or deep thought, and it functions as `visuals.md` principle five, emotional specificity, delivered by posture rather than by expression or by copy. It is the cheapest emotional signal in the library and the brand's polished creative has no equivalent.

The text plan is bare: standard platform subtitles, centre screen, white, mirroring the audio exactly, cycling through eight short blocks across eighteen seconds. `Hey, how are y'all affording kids?` then `I can barely take care of myself,` then `me and my husband can barely afford ourselves.` No banner, no graphic, no colour, no artefact, nothing to look at but her face. That absence explains the shape of the numbers precisely: with nothing to save and nothing to show a friend, people did the only thing the video left available, which was to answer it.

### Hook analysis

*"Hey, how are y'all affording kids?"* This is a **Question hook** in `hooks.md` terms, and the thing that separates it from the library's other question hooks is that it is genuine rather than rhetorical. She is not setting up a reveal. She actually wants to know, and the audience can hear that. The word "y'all" builds the bridge in one syllable by addressing the viewer as a peer rather than as an audience.

Compare it with the library's failed question hook. @nothingeversticks asks *"Do you really know what your health insurance pays for?"* on 13,100 views with a 2.26% like rate and **zero shares**, and never answers it. `hooks.md` is firm that an ad has to answer the question it asks. Both videos leave the question open. The difference is that @molly_daw's question is one the audience can answer for her, and @nothingeversticks's is one only the brand can answer. That distinction is the practical takeaway and it decides which kind of question a brand should open on.

### Script analysis

Eighteen seconds, three segments, and the third one is a repetition. Segment one, the question. Segment two, the personal admission that qualifies her to ask it: *"I can barely take care of myself, but me and my husband can barely afford ourselves. I feel like everywhere I turn and look, a new friend, family member or neighbor is having a baby."* Segment three, the question again, three times, degrading: *"How. How? What's going on? How are y'all doing this?"*

That degrading repetition is the mechanic, and under `adapting-scripts.md` Step 7 it is the thing most likely to be lost in adaptation. Writing it out as three separate sentences on a page makes it look like filler. Spoken, it is the sound of someone giving up on getting an answer, and it is what turns a complaint into an invitation. Step 3 of the method says the sentence-length pattern and energy level must remain intact, and here they are the whole asset.

The structural gap is the one the brand fills. Under the first caveat in Step 3, a reference that is ninety-five percent right but has no slot for the solution needs a segment added where it makes sense. This video has no segment four. The brand's own version arrives from a second voice rather than from her, which is precisely the **Comment Response** structure demonstrated two entries above, and the account has never run either format. Worth holding honestly alongside that: the brand's own stated objection list includes "I should just wait for open enrollment," and a video that only names the problem gives a woman waiting for November nothing to do today.

---

## What this month's pull says as a whole

Three things sit above the individual entries.

**The library is a seasonal document and nobody in this build had counted it.** **9 of the 19 Relevant videos, or 47.4%, were posted between October 1 and December 31**, across three separate years. That stretch is a quarter of the calendar carrying nearly half the category's Relevant content. Verified, computed from the `global_video_created_at` field on all 23 rows. I want to be careful about how hard the view-share version of that lands. Those nine carry **6,911,000 of the library's 9,376,300 total views, or 73.7%**, but @drashleehendry alone is 6,200,000 of that, and stripping her out drops the Oct-to-Dec share of remaining views to **22.4%**. So the count is the finding and the view share is not. `seasonality.md` says the value in a seasonal read is the nuance rather than the calendar, and the nuance here is that the brand's own stated objection list already contains "I should just wait for open enrollment," which means its audience is being told by the calendar to defer at exactly the moment the category's content volume peaks. That doc is also firm that seasonal creative has to be teed up months ahead and that evergreen winners stay running while seasonal work layers in rather than replacing them. It is September. The account's evergreen POV husband family is at **$87,991.09 across 20 ads at a $19.56 blended CPL** and should not be touched.

**The category's attention is anchored to a life stage the brand's product may screen out.** 12 of the 19 Relevant videos are built on pregnancy, delivery or a baby's first year, and the brand's ad library returns zero matches for "pregnant" lifetime. The sibling audit read that as untested ground and asked why the attention concentrates there. The comment corpus complicates it: **42 comments across 15 ads over 14 months are women reporting they were told they do not qualify because they are pregnant or planning to be**, and the brand's own stated objection list does not name that objection at all. So the honest read is that the gap between the category's biggest subject and the brand's silence on it may not be an oversight. It may be the product. That is why the pregnancy-adjacent reference I selected, @paumod, speaks to women who already have coverage rather than to women trying to get it.

**The formats the account has never run are all cheap and all proven in category.** Faceless, green screen, comment response and the second task each have a working in-category example in this library, each costs less to produce than the account's current polished output, and each has a specific failure mode this pull identified. Faceless dies without a banner in frame zero. Green screen needs a real document the brand does not currently own. Comment response needs a comment the brand already has 1,322 of. The second task needs the runtime to be worth buying, which the account's 2.30% to 3.30% hold rates suggest it currently is not.

---

## Open loops

Four. The territories this audit hunts in that came back genuinely clean are left empty rather than filled. The five-and-five split failure, the missing follower counts and the empty review store are infrastructure and sit in the frontmatter's data limitations rather than here, per the rubric.

### Loop 1 — How much of the audience this category's content reaches is an audience this brand's product can actually cover?

**Observation.** Twelve of the 19 Relevant videos in the library are anchored to pregnancy, delivery or a newborn, and those twelve include the three largest by view count. At the same time, 42 comments across 15 of the brand's own ads over 14 months are women saying they were told they do not qualify because they are pregnant or planning to be, and the brand's own five stated objections do not include that one.

**Pull — Tension.** It fired when I finished counting the library's pregnancy anchor and then read the comment corpus, and the two sources could not both be describing a workable opportunity.

**Question.** How much of the demand this category's biggest content reaches is demand this brand's product can serve?

**Justification.** If most of it cannot be served, then the whitespace the account keeps being pointed at is a trap and the money should go elsewhere. If most of it can, the account is leaving its largest audience untouched. The answer changes where the next quarter's production goes.

**Territory.** Product.

### Loop 2 — What happens to a mom in this category between October and January?

**Observation.** Nine of the 19 Relevant videos, 47.4%, were posted between October 1 and December 31, across three different years, in a window that is a quarter of the calendar. One of them opens with *"It is December. Why is nobody talking about this right now?"* and another carries the hashtag `openenrollment2025`. The brand's own stated objection list already contains "I should just wait for open enrollment."

**Pull — Pattern.** It fired when I sorted the library by post date rather than by views and the same three-month stretch kept coming back across unconnected years and unconnected creators.

**Question.** What changes for a mother in this category between October and January?

**Justification.** The brand judges everything on CPL and it has never had a seasonal read of its own. If her behaviour, her question or even who in the household is asking shifts inside that window, then the creative built for the rest of the year is the wrong creative for the quarter the account is about to enter.

**Territory.** Personas.

### Loop 3 — Who is the woman doing this math before she has children?

**Observation.** The highest-conversation video in the whole library, at a 1.79% comment rate and 557 replies from 31,200 views, belongs to a creator whose own hashtags are `childlessmillennial` and `dink`. She has no children and is working out whether she can afford to. The brand's five stated ICPs all already have kids, and the library was scraped on mom-and-insurance keywords.

**Pull — Surprise.** It fired when I read the row's hashtags after reading the transcript, having assumed from the video that she was a mother like everyone else in the pool.

**Question.** Who is the woman running these numbers before she has a child?

**Justification.** She showed up unbidden in a mom-keyword scrape and out-talked every mother in it. If that audience is reachable and near the brand's product, it is a buyer nobody in the category is speaking to. If she is not, the brand should know that the loudest video in its category belongs to someone it cannot sell to.

**Territory.** Personas.

### Loop 4 — Who is picking up this demand when no brand does?

**Observation.** Two creators in this library are individual licensed insurance agents doing organic lead generation in the comments, one closing with *"comment and I'll be in touch and we will run a quote,"* the other offering *"if you need any help with this, this stuff is confusing, I get it."* At the same time the brand's own comment sections are being worked by other agents: one operator's pitch script appears at least nine times under a single ad on a single day, addressed to different women by name, and another writes *"You can get a health insurance without paying premiums $0/month... Pm me if you need health insurance."*

**Pull — Pattern.** It fired when the same behaviour turned up in two unconnected places, the open category feed and the brand's own paid comment sections, on the same day of reading.

**Question.** Who is actually picking up the demand this category generates?

**Justification.** The brand pays for the attention and something else may be converting it. If individual agents are harvesting a meaningful share of the women who watch these ads, then the leak is downstream of creative and no hook change fixes it.

**Territory.** Product, the buyer journey side of it.

---

## Appendix - Parker media links

**M001** — @drashleehendry, "Pregnancy Self pay pricing," posted 2025-11-12, 6,200,000 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=a15b7ef7-b29d-467f-8498-893c832bf05a&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@drashleehendry/video/7571648042147908894` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7571648042147908894_1788468281/7571648042147908894_join_me_as_i_call_around_and_get_self_pay_pricing_.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7571648042147908894_1788468281/thumbnail.jpg` — Discussed in: Brand database 1.

**M002** — @friencine, "A HILL I WILL DIE ON A SECOND TIME MOM!", posted 2025-12-17, 175,800 views. Highest like, share and save rates in the library. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=484c7ffd-b990-4ae4-96a9-7c73313736c0&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@friencine/video/7584916120965008671` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7584916120965008671_1788468783/7584916120965008671_when_i_was_pregnant_with_my_first_i_missed_out_of_.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7584916120965008671_1788468783/thumbnail.jpg` — Discussed in: Brand database 2.

**M003** — @kaseyjaneanderson, "WE DON'T HAVE HEALTH INSURANCE family of 4," posted 2026-03-13, 872,100 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=731bd1a3-8c13-4faa-8c54-ccdce1503972&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@kaseyjaneanderson/video/7616717859724545311` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7616717859724545311_1779072506/7616717859724545311_ive_wanted_to_make_this_video_for_so_long_but_was_.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7616717859724545311_1779072506/thumbnail.jpg` — Discussed in: Brand database 3.

**M004** — @paumod, "PSA IF YOU'RE PREGNANT do this before you start shopping," posted 2026-01-08, 916,200 views. Second highest save rate in the library. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=94e28178-adf8-4ee5-9de1-a274f54dddf7&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@paumod/video/7593050209676987662` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7593050209676987662_1777257347/7593050209676987662_if_you_have_health_insurance_they_may_cover_matern.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7593050209676987662_1777257347/thumbnail.jpg` — Discussed in: Brand database 4.

**M005** — @asap.kristy, the two-number bill reveal, posted 2025-08-09, 120,200 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=ae99a5dd-5102-41c2-becb-59c9c414c747&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@asap.kristy/video/7536693373290270007` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7536693373290270007_1788469019/7536693373290270007_revealing_how_much_i_pay_for_my_monthly_doctor_vis.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7536693373290270007_1788469019/thumbnail.jpg` — Discussed in: Brand database 5.

**M006** — @readra21, the itemised bill panned top-down, posted 2025-11-15, 213,100 views. Lowest save rate in the library. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=d4293d9f-8006-49df-9a76-a9abff310d2b&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@readra21/video/7572985864435879181` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7572985864435879181_1788468482/7572985864435879181_selfpaynoinsurance_emergencyroom.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7572985864435879181_1788468482/thumbnail.jpg` — Discussed in: Global database 1.

**M007** — @dannitangie, the green-screened bill walkthrough, posted 2026-02-28, 28,200 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=9723d817-f5c9-46d8-829f-996332d76784&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@dannitangie/video/7611735950615498014` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7611735950615498014_1788469122/7611735950615498014_how_much_did_you_pay_for_your_delivery_i_had_a_won.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7611735950615498014_1788469122/thumbnail.jpg` — Discussed in: Global database 2.

**M008** — @adulting_with_kim, the comment sticker answered from a car, posted 2024-10-29, 25,500 views. Lowest like rate and fourth highest comment rate in the library, and the only creator in it who reads as over 40. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=3b443979-1d81-4537-a25c-a9f44715c240&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@adulting_with_kim/video/7431177503483415839` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7431177503483415839_1788468595/7431177503483415839_replying_to_madratterr_the_affordable_care_act_mad.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7431177503483415839_1788468595/thumbnail.jpg` — Discussed in: Global database 3.

**M009** — @kclairemoore, "HAVING A BABY IN 2026," posted 2025-10-30, 131,200 views. The makeup second task. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=f90a6870-b22b-42d1-8b7b-0c9316d2b6ba&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@kclairemoore/video/7567018980993469710` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7567018980993469710_1773512819/7567018980993469710_ever_heard_of_indemnity_insurance_for_moms_its_the.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7567018980993469710_1773512819/thumbnail.jpg` — Discussed in: Global database 4.

**M010** — @molly_daw, "Hey, how are y'all affording kids?", posted 2025-11-23, 31,200 views. Joint highest comment rate in the library. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=c284bf02-419e-4332-a8a9-aae37bcc4704&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@molly_daw/video/7576033059330329886` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7576033059330329886_1788468277/7576033059330329886_are_we_not_living_in_the_same_economy_childlessmil.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7576033059330329886_1788468277/thumbnail.jpg` — Discussed in: Global database 5.

**M011** — @nothingeversticks, "Do you really know what your health insurance pays for?", posted 2026-06-15, 13,100 views. Zero shares. Cited as the failed question hook. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=9d665f4b-7c17-4ff0-9ac8-03d35c5ee0c8&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@nothingeversticks/video/7651751227738410253` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7651751227738410253_1788110408/7651751227738410253_picking_a_health_insurance_plan_is_so_much_fun_sin.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7651751227738410253_1788110408/thumbnail.jpg` — Discussed in: Global database 5, hook analysis.

**M012** — @insurancebyalexa, "HAVE YOU HEARD OF THE 'FAMILY GLITCH'?", posted 2022-12-02, 29,000 views. A licensed agent doing organic lead generation, cited in open loops 2 and 4. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=f61d6671-3d49-4e61-96d1-97a730a56ca4&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@insurancebyalexa/video/7172410850244988206` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7172410850244988206_1788468596/7172410850244988206_is_your_employer_health_insurance_too_expensive_i_.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7172410850244988206_1788468596/thumbnail.jpg` — Discussed in: Open loops 2 and 4.

**M013** — Brand ad `MOMS38 - 2 - V3`, ad 120239427583990519, ad set "Moms38 - 2 - 1 (when you call your insurance)." The scripted insurance call, 24.48% hold rate, the highest in the account. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239427583990519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/ac618198a35cfeb2673e5da1357fffe956395a61101a1885c2e462f2e58c1319.mp4` — Discussed in: Brand database 1.

**M014** — Brand ad `MOMS30 - 1 - V20`, ad 120238476016180519. The silent clinician in the lab coat, 39.38% hook rate and a 2.44% hold rate. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238476016180519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1138af6ab844716ddbcd78a371c0ea9d4897abfc8c71f84bbdadbee2a0bdd3b8.mp4` — Discussed in: Brand database 1, hook analysis.

**M015** — Brand ad `Moms43 - 4 - V3`, ad 120241073380060519. The POV husband hook, the account's top spender, 45.55% hook rate, 3.30% hold rate, $24.45 CPL in the window. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4` — Discussed in: Global database 4, and the whole-pull read.

**M016** — Brand ad `moms-63 2b`, ad 120247093361410519. POV husband copy, the cheapest lead in the account at a $13.29 CPL. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4` — Discussed in: Brand database 3, Global database 5.

**M017** — Brand ad `moms54-4`, ad 120247063735970519. The "monkey bars" crying hook, $38.09 CPL, the account's most expensive lead. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063735970519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e3aa685999bf4fde82152827c7fc95489462441238ae397a7e24c3a2f8bd7ddc.mp4` — Discussed in: Brand database 3.

**M018** — Brand ad `MOMS39 - 2 - V2 - Copy`, ad 120247037227340519. The screenshot-outrage overlay, $19.18 CPL in the window. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247037227340519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b5709e2fc3c51b32fc818394fcc0d33d94206dccad0c923f953671d48875d937.mp4` — Discussed in: Brand database 5.

The brand ad `moms-53 3`, the "Approved State List ✔️" creative referenced throughout as the account's $16.01 CPL document ad, is discussed in Brand database 1, 5 and Global database 1. Its dashboard and media handles are held in `audits/2026-09/monthly-hook-audit.md` and were read from that doc rather than re-pulled, so I am not reproducing a link I did not fetch this run.

---

**Brand Context Applied:**

- **What I used:** The five stated ICPs from the brand context document, the brand's own CPL tiers, its stated five-objection list, its untested-format list, the account's lead-generation shape at 4,336 leads and zero purchases, the 94.9% female and 25-to-44 delivery split, and the 1,322-comment Facebook corpus standing in for the missing review evidence under the substitution rule in `running-notes/missing-context.md`.
- **What I avoided:** No government, marketplace or ACA reference appears as a recommendation anywhere, because "ACA" is on the brand's never-use list. No political or partisan framing was carried forward, which is why the library's newest Relevant video is excluded from the ten. No doctor character is proposed without the brand's real licensed partner agents behind it. No pregnancy-only targeting is recommended, and the one pregnancy-adjacent reference selected speaks to women who already hold coverage. No invented statistic appears anywhere; where the brand has no real artefact to show, the entry says so and names the placeholder.
- **Why this fits:** The account is running on a 3.30% hold rate with its biggest spender and has never tested four formats that all have working in-category proof sitting in its own mining library. It has also just entered the quarter where nearly half this category's content historically lands, with an evergreen family at $87,991.09 that should keep running while seasonal work layers on top. These ten references are the cheapest available way to widen the format bank before that window closes.

*this is based on everything I have learned about adapting and re-writing scripts*

*this is based on everything I have learned about visuals in advertising*

*This is everything I know about seasonality in creative.*
