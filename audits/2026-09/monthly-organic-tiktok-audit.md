---
brand: health-for-moms
doc: monthly-organic-tiktok-audit
month: 2026-09
generated_on: 2026-09-04
refresh_by: 2026-10-04
context_docs_read: [running-notes/missing-context.md, running-notes/brand-rules.md, audits/2026-09/monthly-hook-audit.md, source-pulls/ad-account.md, BUILD-STATUS.md, brand context document via get_brand_persona]
knowledge_docs_read: [parker-system/creative-strategy-context/organic-social-analysis.md, parker-system/creative-strategy-context/adapting-scripts.md, parker-system/creative-strategy-context/hooks.md, parker-system/creative-strategy-context/problem-solution-video-ad-formats.md, parker-system/creative-strategy-context/expertise-routing.md, parker-system/creative-strategy-context/visuals.md]
tools_used: [Parker TikTok mining library via search_tiktok_videos with with_video_report true, brand Meta ad library via search_facebook_ads_sql, brand context via get_brand_persona, Parker chat history via search_chat_history]
library_read: 23 of 23 videos in the brand's TikTok mining library, every one at full video-report depth — audio script, visual text script, creator demographics and environment, hook analysis, visual hook, audio hook, text hook, camera and production setup, text overlay analysis, visual elements, and additional observations. No video in the library was read at title or metadata level only.
library_composition: 19 Relevant, 2 Potentially Relevant, 2 Not Relevant, as scored by Parker's own relevancy pass
prior_audit: none — this is the baseline cycle for this doc type
data_limitations:
  - "This is not a read of the brand's own organic. Health For Moms runs no organic TikTok account that Parker can see. No brand-owned organic social surface is connected, and `search_and_manage_organic_social` is not in Parker's tool inventory for this brand. Every video below belongs to a creator with no relationship to the brand. Treat this doc as a category and inspiration read only. Any sentence that reads like brand organic performance would be a fabrication."
  - "The library is a fixed scrape, not a live feed pull. All 23 videos were ingested into Parker on 2026-09-03 from one keyword set of 18 phrases. Parker has no way to run a fresh TikTok keyword, hashtag or creator-handle search from this environment, so the pull could not be widened beyond what the scraper already holds. The next cycle should widen the keyword set — the six queries queued in the hook audit are the place to start."
  - "The scrape is not date-indexed. Post dates come from each video's `global_video_created_at` field, which Parker captured. Those dates are trustworthy. What is missing is any guarantee that the scrape represents what is viral in the niche right now, as opposed to what ranked well on those keywords at scrape time. Recency below is measured, but representativeness of the current feed is not."
  - "View counts are a single snapshot taken at scrape time on 2026-09-03. There is no earlier reading, so no video's growth rate can be read, and a recent post's view count is not comparable to an older post's on equal terms. A video from 2026-08-31 has had three days to accumulate views. One from 2025-11-12 has had ten months."
  - "No comment text is available. Parker holds comment counts for all 23 videos but not a single comment body. Under `organic-social-analysis.md` the comment read is one of the main tests for whether reach is real or boosted, and for what the audience actually took from a video. That test could not be run. Comment-to-view ratios are used instead and are a weaker proxy."
  - "The brand's relevancy reasoning references two ICP names, `Megan` and `Kelsey`, that do not exist in the current brand context document. That document names five ICPs: Jen, Danielle, Marissa, Courtney and Nicole. The relevancy scoring appears to have run against an older persona set. Persona-fit claims sourced from relevancy reasoning alone are marked accordingly below."
  - "No competitor or affinity organic accounts are tracked. The competitor branch is deferred at the team's request. So this niche read has no rival-account baseline to sit against."
  - "The brand runs no organic account, so there is no in-house creator roster, posting cadence or audience to compare the feed's creators against. Casting reads below compare the feed to the brand's paid talent only."
---

# Monthly organic TikTok audit — Health For Moms — 2026-09

## Scope and how this was read

**Read this first, because it changes what the rest of the doc means.** Health For Moms does not run an organic TikTok account that Parker can see. There is no brand handle, no brand posts, no brand followers and no brand comment section in any surface Parker can reach. So nothing below is a report card on the brand's organic performance. It is a read of the open feed in the brand's category — other people's videos about health insurance, medical bills and the cost of having a baby in America — captured as raw material for the next round of paid creative. When this doc says a video "worked," it means it worked for the stranger who posted it. Every claim about the brand itself comes from the paid ad account or the brand context document, and is labelled as such.

**What I read.** Parker's TikTok mining library holds **23 videos** for this brand, all ingested on 2026-09-03 from a single keyword set of 18 phrases covering marketplace tips, pregnancy insurance, deductibles, self-employment and medical debt. I read **all 23 at full video-report depth** — the transcribed audio script, the timestamped on-screen text map, the creator and environment description, the separate hook, visual-hook, audio-hook and text-hook breakdowns, the camera and production notes, and the format observations. That is the whole library, not a sample, so the denominator for every count below is 23 unless I say otherwise. Parker's own relevancy pass scores **19 Relevant, 2 Potentially Relevant and 2 Not Relevant**. *Verified* from `search_tiktok_videos`.

**How I sequenced it, and why that order matters.** `organic-social-analysis.md` is firm that the account read and the idea read are two different jobs, and that engagement should be loaded second, after the work has been read on its own terms. So I read each video's hook, script and visual beats before looking at its view count. That ordering changed two calls. The single most-saved and most-shared video in this library relative to its reach is not the 6.2 million view breakout — it is a 175,800 view video about hospital indemnity coverage. And the second-biggest view count in the library belongs to a video almost nobody engaged with. Sorting by views first would have buried both.

**How I judged engagement.** Raw view counts in a 23-video library are close to meaningless on their own, so I computed like, comment, share and save rates against each video's own views and read every video against the library's own middle. Across the 19 Relevant videos the median is **83,900 views, a 5.78% like rate and a 1.31% save rate**. Those three numbers are the yardstick used throughout. *Verified*, computed from the library's engagement fields.

**The one video that dominates the distribution.** Dr. Ashley Hendry's hospital cold-call video holds **6,200,000 views, which is 66.1% of all 9,376,300 views in the entire 23-video library**. The next largest is 916,200. So one video is roughly seven times the second and two-thirds of everything. *Verified*. That concentration is why the hook audit flagged it, and it is the first thing I went and checked rather than repeated.

**The boosted-post check.** `organic-social-analysis.md` says never to take a big view count as proof of organic strength without testing the engagement shape behind it, because a post with huge reach and thin conversation is usually not a clean organic win. Hendry passes that test convincingly: **10.67% like rate, 3.35% share rate, 1.75% save rate and 22,700 comments**, with `is_ad` recorded as false. Those are the numbers of a real breakout, not a boost. One other video fails the same test and is handled in the underperformers section below.

**Two things this feed does that I did not expect and that shape the whole doc.** First, **it is nearly silent on trending audio.** The video reports explicitly note "no background music" on **10 of the 19 Relevant videos**, and exactly one Relevant video has a music bed described as a real audio choice. The prompt for this doc warns against recommending a concept built on borrowed audio, because the sound cannot be licensed for paid. In this category that warning barely applies. The feed's default sound design is a woman's unaccompanied voice in a quiet room, which is a sound the brand can reproduce for free. *Verified* from the audio-hook fields.

Second, **the feed is anchored to pregnancy and the newborn window far harder than the brand's paid creative is.** **12 of the 19 Relevant videos** are built around pregnancy, delivery costs or a baby's first year. The brand's paid ad library returns **zero** results for the keyword "pregnant" across every ad name, hook, headline, body copy, script, angle and AI analysis field in the account. Not a low number — zero. *Verified* from `search_facebook_ads_sql`, lifetime, all ad types.

**A constraint that has to travel with every recommendation in this doc.** The brand's compliance section is marked non-negotiable and it collides with this feed in three specific places. The brand cannot make government or ACA references, and "ACA" is on its list of words never used in creative. It cannot use political or partisan framing, and the team stated plainly that "Anything political doesnt work." And a doctor character in a script requires a real licensed physician or language adjusted so no false credential is implied. *Stated*, from the brand context document. Those three rules disqualify or reshape a meaningful share of what this feed does well, and I have marked each affected video rather than quietly recommending something the brand has already ruled out.

---

## Recent viral videos in the niche

Sorted newest first. "Recent" here means posted on or after roughly 2025-09-03, which is twelve months back from today. **15 of the 23 videos in the library fall inside that window.** The other 8 are in the carryover section below.

### 1. "How are regular families supposed to keep up?" — @salina_sunshine, 2026-08-31

**Source:** https://www.tiktok.com/@salina_sunshine/video/7680344555161521421
**235,800 views, 17,700 likes, 84 comments, 178 shares, 716 saves.** Like rate 7.51%, above the library's 5.78% median. Share rate 0.08% and comment rate 0.04%, both near the bottom of the library.

**Off-brief, and I am logging it anyway rather than deleting it.** This is a political advocacy ad naming a sitting Georgia congressman. The brand's guardrails ban political and partisan framing outright and the team said political content does not work for them. So the video cannot be adapted. But the prompt for this doc is clear that dropping a video because part of it is unusable throws away the part that is usable, so here is what is in it.

**The creator.** A Black woman in her late thirties or early forties, playing a concerned mother, with a son who looks late teens and a toddler daughter. The video moves through an ER waiting room, a hospital bed, a suburban living room and kitchen, a parking lot and a grocery store.

**The hook, exactly.** Spoken: "My son started to have really bad headaches and then fainted." On screen at the same time, in a white text box: "My son went to the emergency room and the bills started to pile up."

**The visual beats.** It opens on the mother and her son sitting in a doctor's waiting room, then cuts fast to the son lying in an ER bed being treated. Later a real medical bill from TEAMHealth fills the frame with "Total due $130.07" readable on it, then a Walmart self-checkout screen showing $323.88, then home-cooked eggs and sausage on a stove. The pacing is brisk with many jump cuts between ordinary parts of a life.

**The script, as transcribed.** "My son started to have really bad headaches and then fainted. We ended up in the ER and then had to see several specialists and do more testing. And even with health insurance, these bills just keep coming. Every time I open another one, I'm like, how are regular families supposed to keep up? Because it's not just healthcare cost going up, it's everything. Groceries, everyday necessities..." From there it turns to Washington and the congressman, which is where the brand cannot follow.

**Takeaway type: visual.** The salvageable element is the first eleven seconds and one specific device — cutting from the hospital moment straight to a grocery checkout total, so medical debt and the weekly shop are shown as the same problem. That is the "Second Mortgage" angle the team's own Reddit research already surfaced, executed visually instead of said out loud. **The execution note that matters:** even with the sharpest opening in the recent set, this video has a 0.08% share rate against a library median far above it. People liked it and did not pass it on, which is what usually happens when the payload is a political ask.

### 2. "Everyone asks what remote life insurance sales actually pays" — @bestkeptprivate, 2026-07-04

**Source:** https://www.tiktok.com/@bestkeptprivate/video/7658794981456432397
**56,500 views, 4,679 likes, 365 comments, 436 shares, 1,244 saves.** Scored **Not Relevant** by Parker's own pass, and I agree.

This is agent recruitment, not consumer insurance. A Black man in his mid twenties in a cream ARMY thermal shows five days of bank deposits totalling $8,692 and pitches life insurance sales as a career. It appears in the library because the keyword set includes phrases like "everquote reviews" that catch industry content. It serves the wrong audience entirely — the brand sells to mothers, not to people who want to sell insurance. **No takeaway. Logged so the next cycle knows why the keyword set is pulling it in.**

### 3. "When it comes to health insurance during pregnancy, even if you already have insurance, sign up for Medicaid." — @camryunique, 2026-06-27

**Source:** https://www.tiktok.com/@camryunique/video/7656091476400672031
**20,200 views, 1,472 likes, 30 comments, 178 shares, 838 saves.** The **save rate is 4.15%**, more than three times the library's 1.31% median and the third highest in all 23 videos. On the smallest recent view count. That gap between low reach and very high save rate is the signal.

**The creator.** A Black woman in her early to mid twenties, long wavy dark hair, glasses, small hoop earrings, white zip-up hoodie. She is in a plain room with a white door and a few notes pinned to the wall. Even, natural light. Camera on a tripod, chest up, steady.

**The hook, exactly.** Spoken: "When it comes to health insurance during pregnancy, even if you already have insurance, sign up for Medicaid." On screen, black text on a white box across the top, held for the entire 1:07: "What Medicaid pays for during pregnancy."

**The visual beats.** There is almost nothing to look at, and that is the point. She gestures toward the lens on the first word, which puts motion in frame zero. Then she counts benefits off on her fingers while dynamic captions fire word by word along the bottom, switching to red on the specific words "POSTPARTUM CARE" and "DELIVERY COST." Her hands do the work a list graphic would normally do.

**The script, as transcribed.** "When it comes to health insurance during pregnancy, even if you already have insurance, sign up for Medicaid. If you're a mom-to-be, you're gonna wanna save this video so you can come back to it. So Medicaid almost always approves pregnant moms and they will cover you for a year after you have a baby and your child... Some states even give you a free car seat or a playpen. They also have gift cards with money... Additional benefits is they'll give you transportation if you need it."

**Takeaway type: both, with a hard compliance block on the messaging half.** The payload is Medicaid, which the brand cannot name. What transfers cleanly is the structure and one line. The structure is a Question-free Educational open that immediately overturns an assumption the viewer already holds — she thinks having insurance disqualifies her, and the first sentence says it does not. That exact move maps onto the brand's own strongest true claim, that having insurance is not the same as being covered. The line "you're gonna wanna save this video so you can come back to it" is an explicit save instruction, and the video has the third-highest save rate in the library. **What is weak:** at 20,200 views it barely travelled. The idea is stronger than the reach, which is exactly the "strong idea, weak account" case `organic-social-analysis.md` says to preserve rather than discount.

### 4. "Do you really know what your health insurance pays for?" — @nothingeversticks, 2026-06-15

**Source:** https://www.tiktok.com/@nothingeversticks/video/7651751227738410253
**13,100 views, 296 likes, 33 comments, 0 shares, 3 saves.** Like rate 2.26%, well under the 5.78% median. Zero shares. This one did not work, and the reason is instructive.

**The creator.** A woman in her thirties, long dark hair, striped tank top, a tattoo on her shoulder, sitting on a bed or couch in soft daylight. Handheld, close on her face, slight movement. She laughs and sighs a lot.

**The hook, exactly.** Spoken and captioned identically: "Do you really know what your health insurance pays for?" She points a finger at her own face as she says it.

**The script, as transcribed.** "Do you really know what your health insurance pays for? I just... I just finally signed up, I had to pick a new one, but I have searched and searched and searched for weeks now, on and off, and every now and then I got really sick and tired of comparing plans. But let's be honest, do you really know? If you go to the emergency room, do you have to pay, like, a flat fee? Do you pay a certain percentage of it? Does your insurance pay for everything? Is it... do you have to pay your deductible first, which can be 10,000 more or less? It's insane."

**Takeaway type: messaging.** This is a textbook Question hook in the `hooks.md` sense, and the doc is specific that the ad has to answer the question it asks. This one never does. She asks whether you really know, spends ninety seconds proving nobody knows, then says "I just chose one and fingers crossed" and signs off. There is no payoff. **That is the whole execution gap, and it is the most useful thing in this entry.** The brand has the answer this video is missing. A corrected execution keeps her exact opening question and her exact stacked list of unanswerable sub-questions, then resolves them where she gives up. Same hook, same rhythm, an ending.

### 5. "I wish somebody told me about Medicaid sooner during pregnancy." — @camryunique, 2026-05-29

**Source:** https://www.tiktok.com/@camryunique/video/7645420799112842527
**105,300 views, 6,158 likes, 149 comments, 531 shares, 1,763 saves.** Like rate 5.85% and save rate 1.67%, both just above the library median. Same creator as entry 3, five times the reach.

**The creator.** The same Black woman in her mid twenties, this time in a black tank top and black-rimmed glasses, filming from the driver's seat of a car in daylight with sunroof light coming in.

**The hook, exactly.** Spoken: "I wish somebody told me about Medicaid sooner during pregnancy." On screen, white text on a black rectangle across the top, held the full 1:03: "Medicaid coverage during pregnancy." She waves a hand toward the lens on the first syllable.

**The visual beats.** A car interior in bright sun. She leans slightly in. Her hand crosses the frame at zero seconds, which is the only motion the first second gets and is doing real work. She touches her glasses when she reaches vision coverage, so the body language annotates the list.

**Takeaway type: messaging.** The mechanic is regret framing, and it is quieter and sharper than it looks. "I wish somebody told me" does not threaten the viewer. It implies she is currently the person nobody has told, which is a loss-aversion play with no fear in it. **That matters a great deal for this brand**, because the hook audit found the account's high-distress crying openers producing its most expensive leads at $29.85 to $38.09, while its calm openers produced its cheapest at $13.29 to $16.01. This is a way to carry loss without carrying distress. **What is weak:** the payload is again Medicaid, and the hand-wave is the only visual event in sixty-three seconds.

### 6. "If you're pregnant and you're looking for insurance and you didn't qualify for Medicaid like me, listen up." — @yolys.world, 2026-04-16

**Source:** https://www.tiktok.com/@yolys.world/video/7629381899118546206
**14,700 views, 470 likes, 23 comments, 79 shares, 288 saves.** Like rate 3.20%, save rate 1.96%. Modest reach, above-median saves.

**The creator.** A woman in her mid twenties with curly dark hair, a black Vans sweatshirt and a silver heart necklace, sitting on a bed with a dark wood headboard behind her in warm dim light. She is in Florida and says so.

**The hook, exactly.** Spoken: "If you're pregnant and you're looking for insurance and you didn't qualify for Medicaid like me, listen up." On screen, white serif with a drop shadow, held for the full 4:55: "Aetna Pregnancy Insurance Review ✨🤰🏻 | Enhanced Maternity Program Explained."

**The script, as transcribed, at the part that matters.** "Because of my household income, I didn't qualify for Medicaid... we pay like about 298 a month, almost 300 dollars, but it is so worth it. They have a maternity enhanced program that it's amazing. So they have a 24-hour nurse that you can communicate with, which recently I spoke with her. Girl, she asked me everything that I wouldn't even imagine... Then, I get six lactation sessions per month, no copay... Then they cover 100 percent of your breast pump... This is a 300 dollar pump and I only have to pay 59 dollars."

**Takeaway type: messaging, and it is the most direct persona match in the entire library.** She describes, unprompted, the exact woman the brand's ICP Marissa is built around — someone who "makes just enough to fall into that infuriating gap where she doesn't qualify for much help but can't comfortably afford what's available." That is the brand context document's own wording, and this creator narrates it from the inside. **The other thing worth stealing is the register.** She recommends an insurance plan by name for nearly five minutes and it never once sounds like a sale, because she keeps saying "girl" and admits she has anxiety and high blood pressure. That is the mom-to-mom voice the brand names as its own moat, performed by someone with no incentive.

**What is weak:** it names a specific carrier repeatedly, which the brand cannot do under its no-named-competitor rule, and 4:55 is far longer than any ad the account runs.

### 7. "I am finally quitting the insurance industry after 3.5 years. Just kidding." — @itsliterallyjustliz, 2026-04-02

**Source:** https://www.tiktok.com/@itsliterallyjustliz/video/7624310816052972813
**41,200 views, 2,761 likes, 90 comments, 61 shares, 691 saves.** Scored **Potentially Relevant** at 0.6.

Another agent-recruitment video, so the audience is wrong. But the structure is worth two lines because it is the only genuine bait-and-switch in the library. She opens on a career-ending announcement, leans hard into the lens, says "Just kidding," and reveals she is quitting the old *way* of doing the job. On-screen text carries only the false opening and then vanishes, which forces the ear to take over.

**Takeaway type: messaging.** The transferable shape is a false quit, then a turn. A mother saying she is done with health insurance, then clarifying she is done with the *kind* she had, is the same move in the brand's world and lands inside its "system is the villain" positioning without naming anyone. **What is weak:** the reveal happens at about four seconds, which is slow for a paid open, and the hook only works if the false statement is shocking enough to hold.

### 8. "We have not had health insurance for three years." — @kaseyjaneanderson, 2026-03-13

**Source:** https://www.tiktok.com/@kaseyjaneanderson/video/7616717859724545311
**872,100 views, 75,400 likes, 1,316 comments, 12,100 shares, 17,993 saves.** Like rate 8.65% and share rate 1.39%, both strongly above the library median. The second-largest view count in the library.

**The creator.** A woman in her late twenties or early thirties, long brown hair, a ribbed maroon long-sleeve top, sitting at a wooden dining table. Behind her is a wall of framed family photos in warm lamplight. A coffee mug sits at the bottom of frame. It reads like a kitchen-table conversation at the end of a day.

**The hook, exactly.** Spoken, flat and unhurried: "We have not had health insurance for three years." On screen, bold white serif across the top, held for the full 1:28: "WE DON'T HAVE HEALTH INSURANCE family of 4."

**The visual beats.** She is holding a small silver ring near her mouth, close enough that the eye reads it as a microphone for a beat before resolving it as jewellery. That is a small format-break visual in the `hooks.md` sense — the brain stops on the thing it cannot immediately place. Then nothing changes for eighty-eight seconds. The framing never moves. The whole video is her face and that sentence.

**The script, as transcribed.** "We have not had health insurance for three years. This is the reason why I can be a stay-at-home mom. Prior to having kids, I was a nurse. I had the big benefits. I had the big paychecks. When I got pregnant, I wanted to keep working but I also knew in the back of my mind that I wanted to be at home with my kids. It would be so painful for me to go back to work, I think I would have a complete mental crush-out. And so we sacrificed. We sacrificed the benefits, we sacrificed the big paychecks. My husband owns his own business so he doesn't have benefits. And we couldn't afford private benefits. So we're uninsured. And it's been the best decision we've ever made."

**Her caption adds the line the video withholds:** "I've wanted to make this video for so long but was embarrassed that we couldn't afford regular health insurance."

**Takeaway type: both.** This is a Controversy hook in the `hooks.md` sense, and the mechanic is entirely in the delivery. She breaks a social norm about family safety and says it in the tone of someone reporting the weather. `hook-psychology.md` calls this easy to process and hard to predict — the sentence is six words long and the content is genuinely shocking. Nothing in the account does this. **Second thing worth taking:** she establishes she was a nurse at fourteen seconds, which is credential-after-confession rather than credential-first. The viewer has already decided to listen before the qualification lands. **What is weak for paid:** she resolves into a health-sharing group by name, which is a different product than the brand sells, and the video is one static shot for its full run.

### 9. "I just had a baby four months ago and while I was pregnant I was always wondering like how much is this going to cost?" — @dannitangie, 2026-02-28

**Source:** https://www.tiktok.com/@dannitangie/video/7611735950615498014
**28,200 views, 945 likes, 76 comments, 380 shares, 147 saves.** Like rate 3.35%, under the median. But a **1.35% share rate**, which is fourth highest in the library and roughly ten times the share rate of several videos with far more reach.

**The creator.** A woman in her late twenties or early thirties, long dark hair, floral loungewear, filming with a green-screen effect so she stands in front of her own medical bills.

**The hook, exactly.** Spoken: "I just had a baby four months ago and while I was pregnant I was always wondering like how much is this going to cost?" On screen for the first fifteen seconds: "How much does it cost to have a baby in the US with insurance?"

**The visual beats.** She green-screens through four documents in sequence. First the hospital bill, "Total Charges $40,789.94" and "Balance Due $1,925.38." Then the anesthesia bill, billed $10,000, due $1,139.29. Then the baby's own separate bill, billed $523.00, owed $132.03. Then, at 1:11, the iPhone calculator app with the sum being typed live: 1,952.38 + 132.03 + 1,139.29 = 3,223.7. She points at each figure as she reads it.

**The script, at the beat that carries it.** "So the first bill is definitely a jumpscare when it comes into the mail... the total charges were 40,000 dollars... And those were all my bills, but what I didn't realize is that you also get billed for the baby. Like the baby gets billed and they send it to you."

**Takeaway type: visual.** Green Screen is on the brand's own untested video-format list. This is a proven version of it inside the exact category. The specific device to lift is **doing the arithmetic on camera in a phone calculator** — it is slow, it is unglamorous, and the viewer's brain finishes the sum before she does, which is the cleanest possible open loop. **The line worth keeping verbatim** is "you also get billed for the baby," which is a surprise most of the audience has not had yet. **What is weak:** her like rate is below median because the video is long and front-loads a number that is not the real payload.

### 10. "If you're watching this and you're pregnant, don't shop for anything until you call your health insurance." — @paumod, 2026-01-08

**Source:** https://www.tiktok.com/@paumod/video/7593050209676987662
**916,200 views, 81,400 likes, 599 comments, 20,400 shares, 52,376 saves.** Like rate 8.88%, share rate 2.23%, and a **5.72% save rate, the second highest in the entire library**. The third-largest view count.

**The creator.** A woman in her late twenties or early thirties in a cream fleece zip-up with gold jewellery, in a living room with soft window light behind blinds. Handheld selfie, minor shake, direct eye contact.

**The hook, exactly.** Spoken with real urgency: "If you're watching this and you're pregnant, don't shop for anything until you call your health insurance." On screen, high-contrast text held across the centre for the full 1:13: "PSA IF YOU'RE PREGNANT do this before you start shopping." **No music at all**, which makes it land like a voice note from a friend rather than a post.

**The script, as transcribed.** "I'm going to tell you the things that my health insurance covered that I was about to purchase, things that I had put on my baby registry that I'm glad that I didn't have other people buy for me... My breast pump. I had a breast pump on my registry because I did not realize that the health insurance that I was paying for would partially if not fully cover a pump... My insurance covered 70% of it, I think I paid maybe 30, 40 dollars out of pocket. Okay so check for that. Breast milk storage bags. My insurance sent me a hundred a month, more than I could ever get through, 100% covered. Compression socks, 100% covered. A belly band, covered. Every health insurance is different, yours may not cover anything at all but it's worth a quick check."

**Takeaway type: both, and this is the sleeper of the whole library.** The "PSA" framing is a Trigger Word hook that promises need-to-know rather than nice-to-know, and it is welded to a Demographic callout and a command in one sentence. `hooks.md` calls that stacking, and it is why the first second works with no visual event at all. **But the reason to care is the save rate.** 52,376 people saved this. A save is the closest thing organic has to intent, and it is running at four times the library median here. The thing people saved is a checklist of specific things a plan might quietly pay for. **The brand's whole pitch is that most moms do not know what their plan does and does not do.** This video is proof that the category's single most-saved behaviour is exactly that discovery. **What is weak:** it sends people to a third-party website, and it is entirely benefit-listing with no story.

### 11. "A hill that I will die on as a second-time mom is you need that hospital indemnity insurance." — @friencine, 2025-12-17

**Source:** https://www.tiktok.com/@friencine/video/7584916120965008671
**175,800 views, 25,100 likes, 308 comments, 6,978 shares, 15,858 saves.** This video has the **highest like rate in the library at 14.28%, the highest share rate at 3.97% and the highest save rate at 9.02%** — every one of the three above Hendry's, on 2.8% of Hendry's reach. Measured relative to its own reach, this is the strongest video in the library. *Verified*, computed against all 23.

**The creator.** A Black woman in her late twenties or early thirties in a patterned head wrap and gold-rimmed glasses, filming from her bed with a headboard and a decorative rainbow pillow behind her. Soft window light. No music.

**The hook, exactly.** Spoken with real conviction: "A hill that I will die on as a second-time mom is..." and then she stops the sentence. On screen, bold white with a black outline across the top, held for the full 0:46: "A HILL I WILL DIE ON A SECOND TIME MOM!"

**The visual beats.** Almost nothing happens, and it does not need to. Tight on her face, chest up. At seven seconds a second white box drops into the middle of frame with the answer, "Hospital Indemnity Insurance," so the loop she opened stays open for a full seven seconds before the payoff lands as a graphic rather than a line.

**The script, in full, because it is only forty-six seconds.** "A hill that I will die on as a second-time mom is you need that hospital indemnity insurance. You're basically getting paid to have this baby. You're basically getting paid extra free-ish money to have this baby. Sign up, just sign up. Obviously, you need to do it before you have the baby, or you're pregnant, maybe a year or so or a few months before you have this baby, but get it. Even if you don't have the baby, if you end up in the hospital, you get money. Sign up for hospital indemnity insurance. That is a hill I will strongly stand and die on."

**Takeaway type: both.** The unfinished sentence is the entire hook — she tells you she will die on a hill before telling you what the hill is, and "second-time mom" qualifies her and the audience in the same breath. That is self-reference and an open loop stacked into eight words. **The single most valuable thing in this library for the brand may be the phrase "free-ish money."** It is customer language doing a compliance job by accident. It makes a financial promise while hedging it in the same word, which is precisely the shape the brand's own rules demand when they insist on "up to 30%" and "$0 deductible option" rather than flat guarantees. **What is weak:** hospital indemnity is a different product from what the brand matches people to, so the payload does not transfer even though the structure and the phrase do. And at forty-six seconds it is the shortest substantial video in the set, which is a point in its favour, not against it.

### 12. "Hey, how are y'all affording kids?" — @molly_daw, 2025-11-23

**Source:** https://www.tiktok.com/@molly_daw/video/7576033059330329886
**31,200 views, 999 likes, 557 comments, 30 shares, 49 saves.** Like rate 3.20%, but a **1.79% comment rate, tied for the highest in the entire library** and roughly twelve times the library's typical rate.

**The creator.** A woman in her late twenties or early thirties, hair pulled back, in a blue and white tie-dye sweatshirt on a neutral couch. A large round wall mirror behind her, warm indoor light. Her hand rests on her head, which reads as exhaustion before she says a word.

**The hook, exactly.** Spoken and captioned together: "Hey, how are y'all affording kids?"

**The script, in full. It is eighteen seconds.** "Hey, how are y'all affording kids? I can barely take care of myself, but me and my husband can barely afford ourselves. I feel like everywhere I turn and look, a new friend, family member or neighbor is having a baby. How. How? What's going on? How are y'all doing this?"

**Takeaway type: messaging.** Eighteen seconds, one question, no answer, 557 comments. **This video is the clearest evidence in the library about what actually drives conversation in this category, and it is not the solution — it is the shared complaint asked as a genuine question.** She is not performing outrage. She sounds like she actually wants to know. **What is weak, and it is the whole thing:** there is no product, no payoff and no next step. She asks and stops. That is why 557 people answered and only 49 saved it. **What a corrected execution looks like:** keep the eighteen-second length, keep the exhausted posture and the repeated "How," and let the answer arrive from a second voice rather than from her. The comment section is where the audience already wants to be.

### 13. "You ever wonder why we don't want insurance?" — @readra21, 2025-11-15

**Source:** https://www.tiktok.com/@readra21/video/7572985864435879181
**213,100 views, 3,807 likes, 97 comments, 246 shares, 124 saves.** Like rate **1.79%**, second lowest in the library. Save rate **0.06%**, the lowest of all 23. This is the second-biggest view count among recent videos and almost nobody engaged with it. It is handled in full in the underperformers section below, because that gap is the finding.

**Short version here so the recency order stays intact.** No person on screen at all. A top-down handheld shot of a real itemised medical bill on a table under flat light, the camera panning slowly down a column of dollar amounts as a woman's voice, mildly disgruntled, asks the question. The whole script is four sentences: "You ever wonder why we don't want insurance? Here's our bill prior. And here's our bill cash pay. This is why the insurance companies need to be out." The document shows total charges of $55,623.00, an adjustment of minus $54,219.00, and a final balance of $1,404.00. **Takeaway type: visual.**

### 14. "This is Dr. Ashley Hendry. I was calling to get a quote for a self-pay patient." — @drashleehendry, 2025-11-12

**Source:** https://www.tiktok.com/@drashleehendry/video/7571648042147908894
**6,200,000 views, 661,800 likes, 22,700 comments, 208,000 shares, 108,770 saves.** Like rate 10.67%, share rate 3.35%, save rate 1.75%. **66.1% of all views in the 23-video library.**

**The hook audit found this one. My job was to verify it and go further, so here is what I checked and what changed.**

**What the hook audit said, and what holds.** It called this a pure Authority hook and the category's top organic performer, and said the brand has never run an Authority hook and lists it as untested. The format call is **confirmed** — a credentialed professional using insider language is the textbook Authority hook in `hooks.md`, and Authority sits on the brand's own video-formats-to-test list at number three, unticked. *Stated* by the brand.

**What I found that changes the recommendation.** Two things.

First, **the brand has already put a doctor on screen, and it did not work, because the doctor never spoke.** Ad group `MOMS30 - 1 - V20` opens on what Parker's own creative analysis describes as "a pediatrician in a white lab coat and mask performing a heartbeat check on a calm baby in a medical office." The group spent **$7,407.34 lifetime for 381 leads at a $19.44 CPL on a 39.38% hook rate and a 2.44% hold rate**. The full transcript of that ad is **one line**, at 0:11, from an unnamed female narrator: "Finally, insurance that actually feels like it has our back." *Verified* from `search_facebook_ads_sql` with the script block. So the lab coat has been used as wallpaper. It has never been used as a voice. That is a much sharper gap than "Authority untested," and it is a cheaper thing to fix.

Second, **the mechanic that actually drives the Hendry video is not the lab coat. It is the phone call.** And the brand has run phone-call ads three times. The numbers are below in the cross-check section, and they are the most interesting thing I found this cycle.

**The creator.** Dr. Ashley Hendry, a woman in her thirties in glasses, a navy medical polo and a white lab coat, in her own clinic. A neutral wall, an abstract painting, an examination table visible behind her. Bright clinical overhead light. Her practice logo for Mid-South Direct Primary Care stays visible in frame.

**The hook, exactly.** She is already mid-call when the video starts, which is the whole trick: "This is Dr. Ashley Hendry. I was calling to get a quote for a self-pay patient to see what the global vaginal delivery fee would be." On screen, black text on a white box top-centre, held for the full 5:32: "Pregnancy Self pay pricing."

**The visual beats, in order.** She sits at her desk, phone on speaker, notebook open, pen in hand. As each figure comes back down the line she writes it down, and the number appears on screen at the same moment. The colour coding does the arguing for her — **red for the billed price, green for the cash price**, stacked one under the other so the gap between them is visible without a word of commentary. Over five and a half minutes the screen accumulates a ledger: SVD everything $5,730 in green, then C-section everything $7,574, then SVD $2,760 in red against SVD $2,208 in green, then C-section $3,103 red against $2,482 green, epidural $1,071, circumcision $250, and at the end SVD $5,840 red against $2,244 green. She never editorialises. The two colours do it.

**The script, at the beat that broke it open.** Hendry: "How much of a discount is that from the normal price?" Rep: "That is the normal price. Actually gives all self-pay patients that rate. If you mean a normal price, it would depend on the insurance. So that is what any patient who doesn't have insurance would pay." Hendry: "Is the insurance price usually more?" Rep: "It depends on the insurance." Later, with a second hospital: Hendry: "So the higher number is what's charged if they have insurance?" Rep 2: "If you have insurance and everything, it just depends on what insurance you have."

**Why it stops the scroll, in mechanism terms.** `hooks.md` names **precognitive sound** as one of the four things the brain stops on in the first second: familiar audio with half of it missing, one side of a phone call, audible pauses with no reply yet. That is exactly what the first second of this video is. Stacked on top of it is a **format-break visual** — a doctor in a lab coat doing the thing patients are told they cannot do. And a **short open-loop text overlay**, three words, "Pregnancy Self pay pricing." Three of the four mechanics in the first second, and the spoken credential does its work at the one-to-three-second re-hook, exactly as the doc predicts.

**Takeaway type: both.** **What is weak, and it is the reason this cannot be copied straight:** the brand's compliance section says a doctor character requires a real licensed physician or adjusted language that does not imply a false credential. *Stated*, non-negotiable. So the brand cannot hire an actor in a coat. It can either partner with a real clinician or move the credential to a role it genuinely owns — its own licensed partner agents, who are real and licensed and currently invisible in every ad in the account.

### 15. "Stop scrolling if you're having a baby in 2026." — @kclairemoore, 2025-10-30

**Source:** https://www.tiktok.com/@kclairemoore/video/7567018980993469710
**131,200 views, 5,725 likes, 63 comments, 945 shares, 2,938 saves.** Like rate 4.36%, save rate 2.24%, above median.

**The creator.** A woman in her late twenties or early thirties in a tan button-down and a small gold necklace, standing in a white-tiled bathroom with a glass shower door behind her. A baby sits in a bouncer in the bottom-left corner of frame. Bright natural light. She is holding a mascara wand and doing her makeup throughout.

**The hook, exactly.** Spoken as a direct command: "Stop scrolling if you're having a baby in 2026 because I have ways to save you money." On screen, bold black on a white box, held for the full 2:02: "HAVING A BABY IN 2026."

**The script, at the beat that carries it.** "It pretty much paid for my entire hospital stay almost. I just got my check in the mail this morning and literally $300... yeah, only $300 is what I have to pay for having Riggan's and that's crazy. I just paid off my first child who's three because I was on a payment plan because it was so expensive."

**Takeaway type: visual, and the visual is the format itself.** The makeup is not decoration. It is the device that makes two minutes of dense billing information watchable. The eye has somewhere to go while the ear does the hard work. `hooks.md` puts this exactly: match the visual load to the text load, and when the message is mechanical and informational the visual has to give the eye something easy. **The comparison beat is the other thing to take:** she contrasts her first child, still on a payment plan three years later, against her second, $300 and done. That is a Before/After Contrast built out of two of her own children, which is on the brand's untested format list. **What is weak:** the dated hook, "in 2026," is a real filter that qualifies hard, but it ages out. In four months it is wrong.

---

## Older carryovers worth keeping in play

Eight of the 23 videos were posted before roughly 2025-09-03. They are not discredited by age — the prompt is explicit that an older viral concept the brand has never tested can still be a strong adapt. But the age is a risk the strategist has to weigh, so it leads each entry.

### 16. "As you all know I am currently pregnant so I wanted to share with you guys exactly how much I'm currently paying." — @asap.kristy, 2025-08-09, about 13 months old

**Source:** https://www.tiktok.com/@asap.kristy/video/7536693373290270007
**120,200 views, 8,560 likes, 59 comments, 40 shares, 228 saves.** Like rate 7.12%, above median. Share rate 0.03% and save rate 0.19%, both near the bottom.

A woman of Asian descent in her mid twenties in glasses and a white off-shoulder sweater, filming from a car seat in bright daylight. On screen, held the full 1:06: "IM CURRENTLY 5 MONTHS PREGNANT SO HERES HOW MUCH I PAY FOR MY MONTHLY DOCTOR VISITS."

The mechanic is a **two-number reveal**. She screenshots her bill twice: "Amount Billed $1,100.00" at 0:32, then "What I Owe $28.11" at 0:41. Her line under it: "That is a huge difference. That is why it's so important to have insurance because if I didn't I literally cannot imagine paying $1,100 just for a monthly visit."

**Takeaway type: visual.** Two screenshots, nine seconds apart, arithmetic the viewer does themselves. **This is the only video in the library where good insurance is the hero rather than the villain**, which makes it the closest structural match to what the brand actually sells. **The age risk is real but low** — a doctor's bill screenshot does not date. **What is weak:** the high like rate with a near-zero share rate says people enjoyed it and did not think anyone else needed it, which is what happens when a video ends on gratitude rather than on a thing to do.

### 17. "How much money should you be prepared to spend as a single mom by choice?" — @amandatalksalot, 2025-08-15, about 12.5 months old

**Source:** https://www.tiktok.com/@amandatalksalot/video/7538841869065768247
**14,400 views, 590 likes, 16 comments, 4 shares, 188 saves.** Like rate 4.10%, save rate 1.31%, exactly at the library median. Low reach.

A woman in her late twenties or early thirties with ginger hair, a black headband and a red-and-white striped button-up, in a living room with a dark wood shelf and framed photos behind her. On screen, held the full 6:33: "expenses as a single mom by choice."

At 0:23 a **two-column spreadsheet takes over the centre of frame, 25 expense categories and a total of $9,274 a month**. She walks the list line by line. The line the brand should care about, verbatim: "I pay $200 for me and Evie in insurance, this is one place that you should double check with your job to see how much insurance would cost if you add on a dependent or if you need to go to the marketplace, um, because you're going to want to have insurance with a newborn."

**Takeaway type: visual.** A real spreadsheet on screen, held long enough to read, is the strongest version of the document device in this library because it lets insurance be found inside a wider budget rather than argued about on its own. **The strategic value is the framing:** she does not attack insurance. She lists it beside rent, daycare and groceries, which is the "Second Mortgage" angle from the team's own research, shown rather than claimed. **What is weak:** 6:33 is unusable at that length, her income level is far above the brand's ICPs, and 14,400 views means the idea is unvalidated at scale.

### 18. "Let me tell you my experience having United Healthcare as an insurance provider." — @goojiepooj, 2024-12-05, about 21 months old

**Source:** https://www.tiktok.com/@goojiepooj/video/7444916814754237742
**83,900 views, 3,772 likes, 222 comments, 92 shares, 149 saves.** Like rate 4.50%, comment rate 0.26%, share rate 0.11%.

A woman in her twenties or thirties in glasses, a long side braid and a bright purple fuzzy robe, sitting on a bed with purple patterned sheets. Her dog Beaugart wanders into frame at 0:37 and she talks to him mid-sentence: "Beaugart, come here, I'm telling them about insurance."

**The hook** names a company out loud, which is the entire mechanic and the entire reason the brand cannot copy it. The story runs 2:41 through a bureaucratic maze: she gives birth, qualifies for a different program the moment the baby is born, gets dropped by her insurer, gets billed for a plan she does not have for a full year, and ends on "the hospital did end up sending multiple of my bills to collections, it ruined my credit score and I still haven't paid some of them. America! Love you guys, drink water, bye."

**Takeaway type: messaging.** The salvageable element is the **robe**. `hooks.md` and `visuals.md` both hold that native context beats polish, and a purple fuzzy robe with a dog wandering through is about as unplanned as a frame can look. Everything the brand runs is lit and composed. **What is weak beyond the age:** it names a specific insurer repeatedly, which the brand's no-named-competitor rule blocks, and it has no resolution at all — the story ends in defeat. That is exactly the shape `emotional-delivery-and-timing.md` warns about, a threat opened and never closed, and it matches what the hook audit found in the account's own distress lane.

### 19. "we talk about some like real life stuff" — @kennyslifejourney, 2024-11-28, about 21 months old

**Source:** https://www.tiktok.com/@kennyslifejourney/video/7442341495849471275
**21,300 views, 1,272 likes, 381 comments, 15 shares, 14 saves.** Like rate 5.97%, and a **1.79% comment rate, tied for the highest in the library** with @molly_daw.

A Black woman in her twenties or thirties in glasses, a black hair bonnet and a beige bathrobe, in a bright kitchen. She makes coffee through the whole video, pouring and handling a bottle of almond creamer from about 0:45 to 0:58. On screen, held the full 1:25: "I just joined my husband's benefits...this to expensive 😩 (this blew my mind this morning)."

**The script, at the number that made it.** "the family plan was $52 and it said okay to continue the family plan it'll be 55 and I was like well let me finally put myself on there wait guess how much it was to put me on there just me $240 plus the 53 for the family so now I'm paying... $300 out of each check for some medical do y'all hear that $300 I'm not gonna have anymore that is crazy."

**Takeaway type: messaging.** This is the family glitch described from the inside without the term ever being used, and it is the brand's ICP Courtney's exact situation — the brand context has Courtney priced out of her husband's plan at an extra $480 a month, and this creator is living the same arithmetic at $240. **The most important structural detail is the coffee.** Same device as @kclairemoore's mascara: a second task that gives the eye somewhere to go while the ear handles money. Two of the library's most comment-heavy videos use it. **What is weak:** at 21,300 views the reach is small and it is nearly two years old, so this is a low-confidence signal carried for its language, not its performance.

### 20. "If you're signing up for health insurance and you're confused about what plan to get, I got you." — @venteurhealth, 2024-11-14, about 22 months old

**Source:** https://www.tiktok.com/@venteurhealth/video/7437207239217319214
**14,700 views, 272 likes, 9 comments, 58 shares, 96 saves.** Like rate 1.85%, near the bottom of the library. Scored **Potentially Relevant** at 0.6.

A woman in her late twenties or early thirties in a navy sweatshirt in a domestic kitchen with a window behind her, explaining high deductible plans for eighty-two seconds. On screen: "Pros and Cons of getting a HDHP."

**Logged mainly as a counter-example, and that is worth something.** Parker's own relevancy note flags the conflict: the video explains why a high deductible plan can be a good idea, which runs directly against the brand's "$0 deductible option" claim. It also has the second-lowest like rate in the library. **Takeaway type: none the brand should use.** The read is that neutral, balanced explainer content underperforms badly in this category. Every video in the top half of this library takes a side.

### 21. "I am shocked how many people are in your exact situation." — @adulting_with_kim, 2024-10-29, about 22 months old

**Source:** https://www.tiktok.com/@adulting_with_kim/video/7431177503483415839
**25,500 views, 309 likes, 126 comments, 53 shares, 147 saves.** Like rate **1.21%, the lowest in the entire library**. But a 0.49% comment rate, fourth highest. That inversion is the whole story.

A blonde woman in her late thirties or early forties in a green tank top, filming from the driver's seat of a clean white-leather car in bright light. **She is the only creator in the entire library who reads as over 40.**

**The visual hook is a TikTok comment sticker pinned top-left for the full sixty seconds**, quoting a real viewer: "I've been out of insurance for a year because I can't afford it out of pocket and don't qualify for Medicaid." She answers it directly.

**The proof beat, verbatim:** "A lot of people think 'Well, my income is too high, I'm not gonna qualify for a subsidy.' And that's not true either. I just got a family of three with two working parents a zero premium on their health insurance."

**Takeaway type: visual.** Comment Response is on the brand's untested video-format list. This is the format executed in-category, and the mechanic is that the hook is written by a customer rather than a copywriter. The brand has a live and rich Facebook ad comment corpus, which `missing-context.md` names as one of its few working evidence surfaces. **The lowest like rate in the library with the fourth-highest comment rate says something precise:** this format does not earn admiration, it earns replies. For a lead-generation account, replies are closer to the thing being sold. **What is weak beyond the age:** the payload is a government subsidy programme the brand cannot name, and 25,500 views is thin.

### 22. "It is December. Why is nobody talking about this right now? Have you heard about the family glitch?" — @insurancebyalexa, 2022-12-02, about 45 months old

**Source:** https://www.tiktok.com/@insurancebyalexa/video/7172410850244988206
**29,000 views, 1,675 likes, 51 comments, 364 shares, 460 saves.** Like rate 5.78%, exactly the library median. Share rate 1.26% and save rate 1.59%, both above it. **Nearly four years old and still out-sharing most of the recent set.**

A woman in her early twenties with red hair and freckles in a grey hoodie, in a plain room with a beige wall and a planner whiteboard. On screen, bold black on a white box held the full 1:31: "HAVE YOU HEARD OF THE 'FAMILY GLITCH'?"

**She does live arithmetic on screen.** From 0:40 the numbers stack in the top right, one line at a time: "$80,000/yr", then "x .09", then "= $7,200/yr", then "÷ 12", then "= $600/mo." She holds her phone up with the calculator app visible while she talks. Her closing register is worth keeping: "If you need any help with this, this stuff is confusing, I get it."

**Takeaway type: visual.** The staged calculation is the same device @dannitangie uses and the same one Hendry uses with her red and green columns. **Three separate creators, across four years, independently landed on "do the maths on screen, one line at a time."** That is a pattern, not a coincidence. **What is weak, and the age matters here specifically:** the seasonal urgency is tied to a 2022 open enrollment window and the whole payload is an ACA rule the brand is forbidden from mentioning. The number-staging device transfers. Nothing else does.

### 23. "My father Apostle Selman started telling me..." — @fweinations, 2024-11-27, about 22 months old

**Source:** https://www.tiktok.com/@fweinations/video/7441944206538526007
**12,700 views, 1,466 likes.** Scored **Not Relevant** at 0. A recorded sermon about caring for the body, in black and white, from a stage. It matched the keyword set on the word "healthy." **No takeaway.** Logged only so the next cycle knows the keyword set is loose enough to pull in religious content.

---

## Underperforming videos with a strong takeaway

Three videos in this library carry a strong element that their own execution let down. `organic-social-analysis.md` is direct about why these matter: the execution is not the idea, and a low view count is not proof the idea is bad.

### The bill on the table — @readra21, 213,100 views, 1.79% like rate, 0.06% save rate

**What the takeaway is.** This is the purest **Faceless "Ugly Ad"** in the library, and that format sits on the brand's own untested video-format list at number nine. There is no person on screen at any point. The visual event is a real itemised medical bill lying on a table, shot top-down and handheld, with the camera panning slowly down a column of dollar amounts the way a reader's eye would travel. The document does the whole job. Total charges $55,623.00. An adjustment of minus $54,219.00. A final "Balance You Owe Now" of $1,404.00.

**What the execution gap was.** 213,100 views is the second-highest recent view count in the library, and it produced a **1.79% like rate against a 5.78% median and a 0.06% save rate against a 1.31% median**. That is a lot of reach and almost no engagement, which is the exact shape `organic-social-analysis.md` says to treat as an unclean signal rather than as proof of organic strength. The reason is in the script. There are four sentences in the whole video: "You ever wonder why we don't want insurance? Here's our bill prior. And here's our bill cash pay. This is why the insurance companies need to be out." The document is arresting and then the video ends on a slogan aimed at an institution. Nobody is given anything to do, and nobody is given a reason to care about their own bill.

**What a corrected execution looks like.** Keep the shot exactly — top-down, handheld, real paper, slow pan, one voice over it. Keep the two-number structure, before and after. Replace the closing slogan with the thing the viewer can check on her own bill. The brand's compliance rule that the villain is always the system rather than a named company already points this way, and this video's failure is that it made the villain the point instead of the viewer.

### The unanswered question — @nothingeversticks, 13,100 views, 2.26% like rate, zero shares

**What the takeaway is.** The stacked question run in the middle of this video is the best articulation of the brand's core problem anywhere in the library, in a real person's words: "If you go to the emergency room, do you have to pay, like, a flat fee? Do you pay a certain percentage of it? Does your insurance pay for everything? Is it... do you have to pay your deductible first, which can be 10,000 more or less? It's insane." That is four unanswerable questions in eighteen seconds, and it is the audience's confusion transcribed rather than described.

**What the execution gap was.** She never answers any of them. `hooks.md` is explicit on Question hooks: answer the question in the ad, do not leave it hanging. She ends with "I just chose one and fingers crossed that this one is the right one." **Zero shares out of 13,100 views.** Nobody forwards a video that only confirms the problem.

**What a corrected execution looks like.** Lift the question run verbatim, keep her laughing exasperation and the handheld closeness and the absence of music, and put the resolution where she puts the shrug. The brand's own strongest paid line already answers this: "this is why you can't simply just say oh I have insurance I'm covered." Same idea, said from the other side.

### The lament with 557 answers — @molly_daw, 31,200 views, 1.79% comment rate

**What the takeaway is.** Eighteen seconds, one repeated question, and the joint-highest comment rate in the library. The mechanic is a genuine question asked without performance, plus the posture of a tired woman on a couch with her hand on her head. She is not selling anything or claiming anything. She is asking.

**What the execution gap was.** No product, no payoff, no next step. 557 people commented and 49 saved. The conversation happened entirely below the video, where nothing could be done with it.

**What a corrected execution looks like.** Keep the length, keep the register, and let the answer come from a second voice — another mother, not the brand. This connects directly to the strongest thing in the brand's own account: the "moms-53 3" ad, whose opening line credits another mother rather than the brand, produced a **$16.01 CPL with a 3.15% CTR and a $0.67 CPC**, the highest CTR of any ad in the account's top 20. *Verified*, from the hook audit's pull of the 2026-08-04 to 2026-09-02 window.

---

## Scripts worth lifting

Read sequentially. Each is a direct transcription from the video report, not a paraphrase.

**1. The cold call, @drashleehendry.** The whole script is a real recorded phone call. The structural spine is a question, a number, then a follow-up question that will not let the number stand alone.

> "This is Dr. Ashley Hendry. I was calling to get a quote for a self-pay patient to see what the global vaginal delivery fee would be." / "$5,730.37. This is for a routine vaginal delivery with pre and post-care in the hospital." / "Does that cover the hospital facility fee or is that just the OBGYN group fee?" / "It's both. It includes all of it." / "How much of a discount is that from the normal price?" / "That is the normal price. Actually gives all self-pay patients that rate. If you mean a normal price, it would depend on the insurance. So that is what any patient who doesn't have insurance would pay." / "Is the insurance price usually more?" / "It depends on the insurance."

**2. The forty-six second manifesto, @friencine, in full.**

> "A hill that I will die on as a second-time mom is you need that hospital indemnity insurance. You're basically getting paid to have this baby. You're basically getting paid extra free-ish money to have this baby. Sign up, just sign up. Obviously, you need to do it before you have the baby, or you're pregnant, maybe a year or so or a few months before you have this baby, but get it. Even if you don't have the baby, if you end up in the hospital, you get money. Sign up for hospital indemnity insurance. That is a hill I will strongly stand and die on."

**3. The confession, @kaseyjaneanderson.**

> "We have not had health insurance for three years. This is the reason why I can be a stay-at-home mom. Prior to having kids, I was a nurse. I had the big benefits. I had the big paychecks. When I got pregnant, I wanted to keep working but I also knew in the back of my mind that I wanted to be at home with my kids... And so we sacrificed. We sacrificed the benefits, we sacrificed the big paychecks. My husband owns his own business so he doesn't have benefits. And we couldn't afford private benefits. So we're uninsured. And it's been the best decision we've ever made."

**4. The eighteen-second lament, @molly_daw, in full.**

> "Hey, how are y'all affording kids? I can barely take care of myself, but me and my husband can barely afford ourselves. I feel like everywhere I turn and look, a new friend, family member or neighbor is having a baby. How. How? What's going on? How are y'all doing this?"

**5. The checklist, @paumod.**

> "If you're watching this and you're pregnant, don't shop for anything until you call your health insurance if you have it obviously. I'm going to tell you the things that my health insurance covered that I was about to purchase, things that I had put on my baby registry that I'm glad that I didn't have other people buy for me so that they could put that money towards things that I actually needed that were not covered by my health insurance. My breast pump... My insurance covered 70% of it, I think I paid maybe 30, 40 dollars out of pocket. Okay so check for that. Breast milk storage bags. My insurance sent me a hundred a month, more than I could ever get through, 100% covered. Compression socks, 100% covered. A belly band, covered. Every health insurance is different, yours may not cover anything at all but it's worth a quick check."

**6. The stacked unanswerable questions, @nothingeversticks.**

> "But let's be honest, do you really know? If you go to the emergency room, do you have to pay, like, a flat fee? Do you pay a certain percentage of it? Does your insurance pay for everything? Is it... do you have to pay your deductible first, which can be 10,000 more or less? It's insane."

**7. The paycheck arithmetic, @kennyslifejourney.**

> "the family plan was $52 and it said okay to continue the family plan it'll be 55 and I was like well let me finally put myself on there wait guess how much it was to put me on there just me $240 plus the 53 for the family so now I'm paying an inch we're gonna be paying what's two 50 plus 50 basic yeah that's $300 $300 out of each check for some medical do y'all hear that $300 I'm not gonna have anymore that is crazy to do bills like how are we surviving"

**8. The bill jumpscare, @dannitangie.**

> "So the first bill is definitely a jumpscare when it comes into the mail. Yeah. So this is the first bill we got from the hospital and the total charges were 40,000 dollars. But thankfully insurance covered the majority of it and total that I had to pay out of pocket was 1,900... And those were all my bills, but what I didn't realize is that you also get billed for the baby. Like the baby gets billed and they send it to you."

**9. The two-number reveal, @asap.kristy.**

> "My total that I got billed per month is $1,100 for that specific doctor visit. Because I have insurance through my employer and because I have already hit my deductible, my out of pocket cost was $28.11. That is a huge difference. That is why it's so important to have insurance because if I didn't I literally cannot imagine paying $1,100 just for a monthly visit."

**10. The comment answered out loud, @adulting_with_kim.**

> "I am shocked how many people are in your exact situation. You can't qualify for Medicaid and the cost of healthcare is too expensive. But there is a solution... A lot of people think 'Well, my income is too high, I'm not gonna qualify for a subsidy.' And that's not true either. I just got a family of three with two working parents a zero premium on their health insurance."

---

## Hooks worth lifting

The opening lines, pulled out so they can be read in a row. Format names are from `hooks.md`.

| # | Exact opening line | Creator | Format | Views |
|---|---|---|---|---|
| 1 | "This is Dr. Ashley Hendry. I was calling to get a quote for a self-pay patient to see what the global vaginal delivery fee would be." | @drashleehendry | Authority, over precognitive sound | 6,200,000 |
| 2 | "If you're watching this and you're pregnant, don't shop for anything until you call your health insurance." | @paumod | Demographic plus command, Trigger Word "PSA" | 916,200 |
| 3 | "We have not had health insurance for three years." | @kaseyjaneanderson | Controversy / Anti-Traditional | 872,100 |
| 4 | "You ever wonder why we don't want insurance?" | @readra21 | Question, faceless | 213,100 |
| 5 | "A hill that I will die on as a second-time mom is..." | @friencine | Controversy plus unfinished sentence | 175,800 |
| 6 | "Stop scrolling if you're having a baby in 2026." | @kclairemoore | Command plus dated Demographic filter | 131,200 |
| 7 | "As you all know I am currently pregnant so I wanted to share with you guys exactly how much I'm currently paying." | @asap.kristy | Storytelling, price transparency | 120,200 |
| 8 | "I wish somebody told me about Medicaid sooner during pregnancy." | @camryunique | Regret framing, quiet loss aversion | 105,300 |
| 9 | "Let me tell you my experience having United Healthcare as an insurance provider." | @goojiepooj | Storytelling opened by naming a company | 83,900 |
| 10 | "Hey, how are y'all affording kids?" | @molly_daw | Question, genuine rather than rhetorical | 31,200 |
| 11 | "It is December. Why is nobody talking about this right now? Have you heard about the family glitch?" | @insurancebyalexa | Question plus Trigger Word, named mechanism | 29,000 |
| 12 | "I just had a baby four months ago and while I was pregnant I was always wondering like how much is this going to cost?" | @dannitangie | Storytelling into a curiosity gap | 28,200 |
| 13 | "I am shocked how many people are in your exact situation." | @adulting_with_kim | Comment Response | 25,500 |
| 14 | "we talk about some like real life stuff" | @kennyslifejourney | Conversational, deliberately low-stakes | 21,300 |
| 15 | "When it comes to health insurance during pregnancy, even if you already have insurance, sign up for Medicaid." | @camryunique | Educational, overturns an assumption | 20,200 |
| 16 | "If you're pregnant and you're looking for insurance and you didn't qualify for Medicaid like me, listen up." | @yolys.world | Demographic, exclusion-based | 14,700 |
| 17 | "Do you really know what your health insurance pays for?" | @nothingeversticks | Question, unanswered | 13,100 |

**The pattern across all seventeen.** Not one opens on crying, shouting or visible distress. Six are questions. Four name a demographic in the first sentence. Three are flat statements of a fact that breaks a norm. **The strongest performers put the shock in the fact and keep it out of the delivery.** That is the same conclusion the hook audit reached from the brand's own CPL data, arriving here from a completely independent source. *Verified* across 17 of 19 Relevant videos, the two exclusions being the political ad and the sermon.

---

## Visuals worth lifting

A library the strategist can read as a shot list. Every entry is observed in a specific video.

**The document as the visual event.** Six of the 19 Relevant videos put a real piece of paper or a real screen in frame and let it carry the message. The itemised bill panned top-down on a table, @readra21. Two bill screenshots nine seconds apart, billed then owed, @asap.kristy. Four green-screened documents in sequence ending on a phone calculator, @dannitangie. A 25-line budget spreadsheet held on screen for over three minutes, @amandatalksalot. Numbers written into a notebook and mirrored on screen as a hospital says them out loud, @drashleehendry. Staged calculator arithmetic in the corner of frame, @insurancebyalexa. **The brand's own account already proves this works in paid** — the "Approved State List ✔️" ad, whose visual event is a wall of state names the viewer scans for her own, delivered a **$16.01 CPL** against a $22.10 account average. *Verified*, from the hook audit.

**Colour as the whole argument.** Hendry writes every price on screen in one of two colours, red for what is billed with insurance in play and green for the cash price, stacked so they sit side by side. She never says the word "expensive." The two colours do it. This is the single most efficient visual device in the library and no ad in the brand's account uses colour to make a comparison.

**The second task that frees the eye.** A woman doing her makeup with a mascara wand while she explains billing, @kclairemoore. A woman pouring coffee and handling a creamer bottle while she reads out her paycheck deductions, @kennyslifejourney. Both videos run well over a minute on dense financial information and both hold. `hooks.md` puts the rule plainly: when the message is mechanical and informational, the visual has to be simple and give the eye somewhere easy to rest. The second task is how these creators buy the time.

**Motion in frame zero, with nothing else in the shot.** @camryunique waves a hand toward the lens on her first syllable. @itsliterallyjustliz leans hard into the camera for the reveal. Both are seated talking heads with no set and no props, and both put physical motion in the first half-second because it is the only thing available. This costs nothing to reproduce.

**The persistent topic banner.** Fourteen of the 19 Relevant videos hold a single text block on screen for the entire runtime rather than letting the hook text disappear after three seconds. Hendry holds hers for all 5:32. @amandatalksalot holds hers for 6:33. @yolys.world for 4:55. The function is that a viewer who arrives mid-video still knows what she is watching, which matters more on a long video than a short one.

**Unplanned rooms.** A purple fuzzy robe with a dog walking through frame, @goojiepooj. A bonnet and a bathrobe in a kitchen at breakfast, @kennyslifejourney. A head wrap on a bed with a rainbow pillow, @friencine — the highest engagement rates in the library. A bathroom mid-makeup with a baby in a bouncer in the corner, @kclairemoore. **Not one of the 19 Relevant videos looks lit or composed.** The brand's own best paid ad opens on a mother and baby in white bedding in soft beige light, which is a beautiful frame and a different species of image entirely.

**The single clinical frame in the library.** Hendry's examination room — neutral wall, abstract painting, examination table, bright overhead light, a practice logo in shot. It is the only professional setting in 23 videos, and it belongs to the video with 66.1% of all the views.

---

## Creator demographics in the feed

This is the read the strategist needs before casting, and it is unusually clean because the library is small enough to count every creator.

**Gender: 19 of the 19 Relevant videos feature a woman.** Eighteen appear on camera. One is a woman's voice over a document with no face, @readra21. Both Not Relevant videos feature men, and both are outside the category — an agent-recruitment pitch and a sermon. *Verified* from the creator-demographics field on all 23 reports.

**Age: the feed skews younger than the brand's paid delivery, and it is not close.** Reading the age description on each of the 19 Relevant videos, **17 read as mid-twenties to mid-thirties**. Exactly **one** reads as over 40: @adulting_with_kim, described as late thirties to early forties. One is unclear because there is no face. **Zero creators in the library read as over 45.** *Verified* that the video reports describe them this way, on all 19. The ages themselves are *inferred* from appearance by the report, since no creator states her age, so treat the band as a casting read rather than a fact about any individual.

**Hold that against the account.** The brand's paid delivery in the 2026-08-04 to 2026-09-02 window ran **43.8% aged 35-44 and 35.7% aged 25-34**, so roughly four in five leads sit between 25 and 44. On that band the feed and the account agree well. **But the hook audit found one ad family putting 30.4% of its spend on women aged 45-54 and 9.3% on 55-64, against 14.3% and 3.6% for the account overall** — the "I wish this was a joke" skit. *Verified*. So the account has found a woman in her late forties that this organic feed does not contain a single example of. **The feed cannot help the brand cast for her.** That is a real limit on this doc and it is worth saying out loud rather than implying the feed covers the whole audience.

**Race and ethnicity.** Among the 18 distinct creators behind the 19 Relevant videos, the reports identify **four as Black** — @friencine, @camryunique who has two videos here, @kennyslifejourney and @salina_sunshine — and **one as of Asian descent**, @asap.kristy. The remaining creators are not identified by ethnicity in the reports, so I am not guessing at them. What is worth noting is where those creators land: **@friencine holds the highest like, share and save rates in the entire library**, and @camryunique's two videos hold the third and sixth highest save rates. The creators of colour in this library are over-represented at the top of the engagement table, not the bottom.

**Setting.** Bedrooms and beds, five videos. Living rooms and couches, four. Cars, three. Kitchens and dining tables, three. A bathroom mid-makeup, one. A clinic, one. A tabletop with no person, one. **The car is a specific and repeatable choice** — @asap.kristy, @camryunique and @adulting_with_kim all film from a driver's seat in daylight, and the reports read it the same way each time, as a quick thought shared during a busy day.

**Delivery register.** The reports describe the tone on the 19 Relevant videos as conversational, calm, matter-of-fact, helpful, relatable or confident. **Not one is described as distressed, crying or panicked.** The nearest is @kennyslifejourney, described as disbelief and frustration, and even she is making coffee while she says it.

**Sound.** Ten of the 19 Relevant videos are explicitly noted as having no background music at all. Exactly one has a music bed treated as a real choice, the lo-fi track under @camryunique's second video. **This is the most commercially useful demographic fact in the section**, because it means the format that wins here does not depend on borrowed audio and therefore carries into paid with no licensing problem.

**Production level.** Every one of the 19 is described as raw, low-fidelity, handheld or lo-fi except Hendry's, which is described as a stable desk tripod in bright clinical light, and @camryunique's second video, described as prosumer. **The casting implication is direct.** The brand's paid creative is polished, lit and composed. The feed the brand is trying to blend into is a woman in a robe in her own bedroom with no music and one static shot.

---

## Cross-check against the ad account

For each candidate idea, whether the brand has already tested it in paid and what happened. All account figures are Meta-reported, lifetime unless stated, from `search_facebook_ads_sql` on 2026-09-03. Northbeam is not connected, so none of this is multi-touch attribution.

### The phone call. Tested three times. This is the finding of the cycle.

The hook audit read Hendry's video as an Authority hook and pointed at the lab coat. Reading the video report closely, the lab coat is the *credential* but the **phone call is the mechanic** — one side of a conversation, an audible pause, a stranger's voice supplying an answer the viewer wants. `hooks.md` names that precisely as precognitive sound and lists it as one of only four things that reliably stop a scroll in the first second. So I went looking for phone calls in the account, and found three.

| Ad | Hook | Lifetime spend | Leads | CPL | Hook rate | Hold rate |
|---|---|---|---|---|---|---|
| `MOMS38 - 2 - V3`, ad set "Moms38 - 2 - 1 (when you call your insurance)" | "I'm calling to see why this wasn't covered when y'all said it would be." | $1,823.59 | 59 | **$30.91** | **51.78%** | **24.48%** |
| `MOMS38 - 3 - V7`, ad set "Moms38 - 3 - 2 (20k skit v2)" | "Hi hospital, I just received a $20,000 bill in my email for a surgery a few weeks ago" | $801.40 | 35 | $22.90 | 33.89% | **17.43%** |
| `OMC-Health for Moms-[B2-C13-V2]` | "Hi, I need to see our family doctor." | $1,149.03 | 69 | **$16.65** | 36.94% | 9.15% |

*Verified.* **The 24.48% hold rate on `MOMS38 - 2 - V3` is the highest hold rate anywhere in this account by a wide margin.** For reference, the account's biggest spender, the POV husband ad, holds at 3.30%, and the craft floor in `ad-account-analysis.md` is 12%. Two of these three clear that floor. **Nothing else in the account does.**

**But all three are scripted, and the team's own ad set name says so — "20k skit v2."** I pulled the full transcript of `MOMS38 - 2 - V3` and both voices are performed by actors. It is a comedy sketch, and a genuinely funny one: "Our system only approves that type of visit on Mondays, Wednesdays, and federal holidays that fall on a Friday." "So I pay $800 a month for?" "For access to coverage, not necessarily coverage itself." "You need to be declared clinically dead and revived twice." *Verified* from the script block.

**So the difference between the brand's version and the 6.2 million view version is not the format. It is whether the call is real.** Hendry's rep is a real hospital employee reading a real price. The brand's rep is an actor delivering a punchline. The brand's version stops more people than anything it has ever run, holds them longer than anything it has ever run, and produces a $30.91 lead, which sits in the brand's own "not good" tier. **That is a specific, testable question and it is now the top candidate below.**

### Authority. Half-tested, and the half that was skipped is the important one.

The brand lists Authority as untested at number three on its video-formats-to-test list. *Stated*. That is true of the *hook*, but a doctor has appeared. Ad group `MOMS30 - 1 - V20` opens on "a pediatrician in a white lab coat and mask performing a heartbeat check on a calm baby in a medical office." The group ran **$7,407.34 lifetime for 381 leads at a $19.44 CPL on a 39.38% hook rate and a 2.44% hold rate**. The transcript is a single line at 0:11 from a female narrator. **The doctor never speaks.** *Verified*.

Read that as a partial result rather than a clean blank. Putting a clinician in frame produced a $19.44 CPL, which is inside the brand's "good" band, on a hook rate just under 40%. The 2.44% hold rate says the opener promised authority and the body did not deliver it. **What has never been tested is a credentialed person saying a credentialed thing.**

### Pregnancy and the newborn window. Never tested. Zero.

A keyword search for "pregnant" across every ad name, headline, body copy, text hook, verbal hook, visual hook, angle, creator description, script and AI analysis field in the account returns **totalMatching 0**, lifetime, all ad types. *Verified*. Meanwhile **12 of the 19 Relevant videos in this library are anchored to pregnancy, delivery or a baby's first year**, and the brand's biggest organic performer in the category is entirely about the price of giving birth.

**The brand's own guardrail is narrower than it first looks.** It says "No pregnancy-only targeting — focus on moms with kids, not expectant mothers exclusively." *Stated*. That rules out building the account around expectant mothers. It does not rule out one ad that speaks to the moment a family's costs change.

### The document on screen. Tested, and it is the account's cheapest lead source.

The "Approved State List ✔️" ad, `moms-53 3`, puts a wall of state names on screen as the visual event and produced **110 leads at a $16.01 CPL with a 3.15% CTR and a $0.67 CPC** in the 2026-08-04 to 2026-09-02 window — the highest CTR of any ad in the account's top 20. *Verified*, from the hook audit. The screenshot-overlay ads do a version of the same thing with a stranger's post. **So the device is proven in this account.** What has not been tried is the brand's own version of a *bill*, red against green, or a calculator doing arithmetic on screen.

### Faceless. Never tested.

Faceless "Ugly Ads" sits at number nine on the brand's untested list. *Stated*. Every ad I inspected in this account has a person in frame. @readra21's video is a proven in-category faceless execution with 213,100 views, and it is proven with a caveat, since its engagement rates are among the library's weakest.

### Comment Response. Never tested.

Number seven on the brand's untested list. *Stated*. `missing-context.md` names Facebook ad comments as one of this brand's few live and rich evidence surfaces, so the raw material for a Comment Response ad already exists in a place Parker can read.

### Green Screen. Never tested.

Number ten on the untested list. *Stated*. @dannitangie's bill walkthrough is the in-category proof.

### The distress lane. Tested, and the account's own numbers argue against extending it.

`MOMS38 - 5 - V2`, "My son fell off the monkey bars at school," opens on a woman crying directly into the lens. It ran **$3,859.58 for 163 leads at a $23.68 CPL on a 48.71% hook rate and a 14.33% hold rate**. *Verified*. High stop, decent hold, a CPL just inside the brand's "meh" band. The hook audit found the wider distress family running $29.85 to $38.09 CPLs. **Not one of the 19 Relevant organic videos opens on crying.** Two independent sources pointing the same way.

---

## Brand and user memory connections

Parker's chat history holds six threads for this brand, all created 2026-09-03, one on the web and five on Slack. I read the two that carry creative substance. Three connections matter.

### The seven-angle bank the team already has, held against what the feed rewards

On 2026-09-03 the team asked Parker to pull customer language from Reddit and competitor reviews, since the brand has no review corpus of its own. That thread produced **seven named angles**: the Deductible Trap, "I Did Everything Right and Still Got Screwed," the Second Mortgage, the Fine Print Betrayal, the Mental Load angle, the Fairness angle, and the Discovery angle. *Stated*, from Parker chat history, Slack thread 1788473402.812619.

**Four of the seven are validated by this feed, and one is not.**

- **The Second Mortgage** is the feed's strongest confirmed angle. @kennyslifejourney's "$300 out of each check for some medical," @amandatalksalot's spreadsheet placing insurance beside rent and daycare, and @salina_sunshine's cut from hospital bill to grocery checkout are three independent creators making the same argument.
- **The Fine Print Betrayal** appears verbatim in the account's own script for `MOMS38 - 3 - V7`, "we had to use an out-of-network anesthesiologist for you," and the Reddit pull had the identical sentence: "The hospital was in-network. The anesthesiologist wasn't. Nobody told me." It appears in @goojiepooj's story too.
- **The Discovery angle** is what @paumod's 916,200 view video is, and the fact that it is the second-most-saved video in the library says discovery is the behaviour this category rewards most.
- **The Fairness angle** is @molly_daw's whole eighteen seconds and it drove the joint-highest comment rate in the library.
- **The Mental Load angle was flagged in that thread as untouched by anyone, and this feed does not contradict that.** No video in the library is about the hours on hold, the EOBs, the prior authorisation battles. @goojiepooj gets closest with "I had to get on the phone for like 20 hours," but it is a beat in a longer story, not the subject. **So the whitespace the team identified independently is still whitespace after reading 23 category videos.** That is a stronger signal than the feed confirming an angle, because it means nobody in the category has taken it.

### The user wants to become an agentic marketer, and already has an inspiration tool

In the same Slack thread the user said: "I really do want to become more of a agentic marketer," and separately, "I also have Gethookd should i hook up that to this claude code thing and we can pull from there too for inspo?" *Stated*, 2026-09-03.

**This matters for this doc specifically.** The largest limitation on this audit is that Parker cannot run a fresh TikTok keyword, hashtag or creator search — it can only read the 23 videos already scraped. The user is holding a second inspiration library and asking whether it can be connected. **If Gethookd can be attached, this doc's biggest constraint goes away next cycle.** That is worth putting in front of them as a concrete reason rather than a general integration question.

### The account's own diagnosis, in the team's words

The brand told Parker: "Right now we're mainly on iterations of our state angle that you will see in the account doing well. But not a ton of creative diversity," and "Havent tried a LOT of different ones I checked off on your formats there so sounds like theres lots to test!" *Stated*, from the brand context document.

**This feed is a direct answer to that sentence.** Of the twenty-two video formats the brand listed as wanting to test, this library contains proven in-category executions of at least six: Authority, Faceless "Ugly Ads," Comment Response, Green Screen, Educational, and Testimonial or First-Person Story. The brand does not need to invent the diversity. It needs to adapt six videos it already has in its own Parker library.

---

## Candidates worth testing

Ranked. Each carries the source video, the takeaway type, the persona signal, and the hypothesis a paid test would settle. `adapting-scripts.md` is the method for all of them — trace the skeleton, replace the content, never redraw the structure, and remember that pacing drift is structural failure.

### 1. The real recorded call

**Source:** @drashleehendry, https://www.tiktok.com/@drashleehendry/video/7571648042147908894, 6,200,000 views.
**Takeaway type:** both.
**Persona signal:** Marissa and Nicole, the two ICPs whose fear is a single bill they did not see coming.
**What it is.** A real phone call, recorded, with a real other party, numbers written on screen as they are spoken, red for what is billed and green for the cash or better-plan price. Not a sketch. No punchlines. The brand's compliance rule requires a real licensed physician or adjusted language, and the brand already has a legitimate credential it never uses on camera: **its own licensed partner agents.** An agent calling to check what a family's current plan actually covers is a real credential doing a real thing.
**The hypothesis.** *A recorded call with a real second party will hold at or above the 24.48% hold rate the brand's scripted call already achieves, while landing a CPL under the $30.91 that version produced.* The account has already shown the format stops people. The open question is whether authenticity is what converts the attention into a lead.
**Prior test:** three scripted versions. Hold rates 24.48%, 17.43% and 9.15%. CPLs $30.91, $22.90 and $16.65. *Verified*.

### 2. The credential that speaks

**Source:** @drashleehendry, plus the brand's own `MOMS30 - 1 - V20`.
**Takeaway type:** messaging.
**Persona signal:** Nicole and Danielle, the two ICPs the brand context describes as researchers who want one trusted person to confirm the answer.
**What it is.** The brand has put a doctor in frame and given her nothing to say. Give the credential the first line. `hooks.md` on Authority hooks: state the credential clearly, let the expert use insider language, show expertise through demonstration rather than claim.
**The hypothesis.** *An opener spoken by a credentialed voice will beat the 39.38% hook rate the silent-clinician ad produced, and will fix the 2.44% hold rate, because the body will finally deliver what the opener promised.*
**Prior test:** the silent version. $7,407.34, 381 leads, $19.44 CPL, 39.38% hook, 2.44% hold. *Verified*. Not a failure — an unfinished test.

### 3. The bill, red against green

**Source:** @drashleehendry's colour system plus @readra21's shot, https://www.tiktok.com/@readra21/video/7572985864435879181.
**Takeaway type:** visual.
**Persona signal:** Jen, the ICP who reads the EOB statements.
**What it is.** A real bill, top-down, handheld, slow pan, one voice over it. Two numbers in two colours. This is the Faceless "Ugly Ad" format the brand lists as untested, executed with the device that made the category's biggest video legible.
**The hypothesis.** *A faceless document opener will produce a CPL at or below the $16.01 the state-list ad delivered, because both work on the same mechanic — a document the viewer scans for her own situation — and the document costs nothing to shoot.*
**Prior test:** the state list, $16.01 CPL, 3.15% CTR, $0.67 CPC. *Verified*, from the hook audit. Faceless itself, never run.

### 4. The unfinished sentence

**Source:** @friencine, https://www.tiktok.com/@friencine/video/7584916120965008671. Highest like, share and save rates in the library.
**Takeaway type:** both.
**Persona signal:** Marissa, who the brand context says "makes decisions quickly once she trusts someone" and would act on a recommendation from a mother she trusts.
**What it is.** Forty-six seconds. One shot. No music. A woman states she will die on a hill, then withholds the hill for seven seconds while a text box supplies it. The brand's own creative principles already demand withheld resolution in a hook. *Stated*. **Carry the phrase "free-ish money" across as a model** — it makes a financial claim and hedges it in the same word, which is the exact shape the brand's "up to 30%" rule requires.
**The hypothesis.** *A hook that withholds its subject for several seconds will hold better than the account's current openers, which name the benefit inside the first sentence and give the viewer nothing left to stay for.*
**Prior test:** none. No ad in the account withholds its subject past the first line.

### 5. The unanswered question, answered

**Source:** @nothingeversticks, https://www.tiktok.com/@nothingeversticks/video/7651751227738410253, and @molly_daw, https://www.tiktok.com/@molly_daw/video/7576033059330329886.
**Takeaway type:** messaging.
**Persona signal:** Danielle, the planner who researches for two hours, gets overwhelmed and circles back weeks later.
**What it is.** Lift the stacked run of unanswerable questions verbatim, keep the exasperated laugh and the absence of music, and put the answer exactly where the original shrugs. Both source videos failed for the same reason and both failed loudly enough to be measured — zero shares on one, 557 comments and 49 saves on the other.
**The hypothesis.** *A question opener that resolves will convert the engagement these organic versions generated but could not use, because the audience is already proven to answer the question and the only thing missing is somewhere to go.*
**Prior test:** none in this shape.

### 6. The second task

**Source:** @kclairemoore, https://www.tiktok.com/@kclairemoore/video/7567018980993469710, and @kennyslifejourney, https://www.tiktok.com/@kennyslifejourney/video/7442341495849471275.
**Takeaway type:** visual.
**Persona signal:** all five ICPs. This is a production technique rather than an angle.
**What it is.** Give the on-camera mother something ordinary to do — makeup, coffee, folding, packing a bag — while she talks money. Two videos in this library run well over a minute on dense billing detail and hold, and both use it.
**The hypothesis.** *Adding a second physical task to an existing winning script will raise hold rate without moving hook rate, because the hook is unchanged and only the reason to stay has been added.* This is a clean single-variable test on a script the account already runs.
**Prior test:** none. Every ad I inspected has the talent doing nothing but talking or reacting.

### 7. The comment as the hook

**Source:** @adulting_with_kim, https://www.tiktok.com/@adulting_with_kim/video/7431177503483415839.
**Takeaway type:** visual.
**Persona signal:** Marissa and Courtney, the two ICPs who sit in the gap where they earn too much for help and too little for comfort.
**What it is.** Pin a real comment from the brand's own Facebook ad comments in the top corner and answer it out loud for sixty seconds from a car. Comment Response is on the brand's untested list, and the comment corpus is live.
**The hypothesis.** *Using a real customer's words as the hook will produce a higher comment rate and a lower like rate than the account's current openers, and for a lead-generation account the comment is the closer proxy for intent.* The source video shows exactly that inversion — the library's lowest like rate paired with its fourth-highest comment rate.
**Prior test:** none.

### 8. The moment the costs change

**Source:** @paumod, https://www.tiktok.com/@paumod/video/7593050209676987662, the second-most-saved video in the library, and @asap.kristy's two-number reveal.
**Takeaway type:** both.
**Persona signal:** Nicole explicitly. The brand context has her seven months postpartum, fighting HR over when her coverage resets, telling the pediatrician's office "I'm working on it" in a voice that sounded like she had it under control.
**What it is.** One ad aimed at the moment a family's costs change, framed as a checklist of things a plan might quietly cover, not as a pregnancy campaign. The brand's guardrail bars pregnancy-*only* targeting, not a single ad that speaks to a trigger moment.
**The hypothesis.** *An ad anchored to the moment costs change will reach a younger and newer segment than the account's current creative, because 12 of the 19 relevant videos in this category are anchored there and the account has never once said the word.*
**Prior test:** zero. "Pregnant" returns no matches anywhere in the account. *Verified*.

### 9. The calm confession

**Source:** @kaseyjaneanderson, https://www.tiktok.com/@kaseyjaneanderson/video/7616717859724545311, 872,100 views.
**Takeaway type:** messaging.
**Persona signal:** Courtney, self-employed, on a short-term plan she is about 60% sure covers anything.
**What it is.** A flat statement of a fact that breaks a norm, delivered with no drama at all, at a kitchen table in lamplight. The credential arrives after the confession rather than before it.
**The hypothesis.** *A calm delivery of a shocking fact will produce a lower CPL than the account's distressed delivery of the same fact.* The hook audit found the account's calm openers landing $13.29 to $16.01 and its crying openers $29.85 to $38.09. This feed contains no crying at all. **This is the cheapest way to test the largest disagreement between the account's current production direction and both available bodies of evidence.**
**Prior test:** the distress lane, six ads and growing. *Verified*, from the hook audit.

---

## Open loops

**1. What is a real recorded phone call doing to a viewer that a scripted one is not?**
The brand's scripted insurance call holds 24.48% of viewers, which is the highest hold rate in its entire account and double the 12% craft floor, and it produces a $30.91 lead, which sits in the brand's worst CPL tier. The category's 6.2 million view organic video is the same mechanic with a real hospital employee on the other end of the line. Pull: **tension**. It fired when I read the brand's ad set name, "20k skit v2," and realised the team classifies as comedy the exact structure that a doctor used as documentary. *Question:* What changes for a viewer when the second voice in an ad belongs to a real stranger rather than an actor? Answering it would tell the team whether their best-holding format is being wasted on a punchline, and the account already has the scripted baseline to measure against. Territory: **Messaging**.

**2. Why is the most saved and most shared video in this category one of the smallest?**
@friencine's forty-six second hospital indemnity video holds the highest like rate at 14.28%, the highest share rate at 3.97% and the highest save rate at 9.02% of all 23 videos in the library, on 175,800 views — 2.8% of the reach of the video with the biggest view count. Pull: **surprise**. It fired when I computed rates instead of reading raw counts and the ranking completely inverted. *Question:* What is it about that video that makes people keep it and pass it on at a rate nothing else in this category reaches? The brand's whole business runs on a mother telling another mother, so whatever drives a share here is the closest organic proxy it has for its own referral mechanism. Territory: **Messaging**.

**3. Who is the woman over 45 that this category's creators never are?**
Across the 19 relevant videos in the library, exactly one creator reads as over 40 and none read as over 45. The brand's own account, meanwhile, puts 30.4% of one ad family's spend on women aged 45-54. Pull: **gap**. It fired when I finished counting the age descriptions and realised the feed cannot supply a single casting reference for a demographic the account is already reaching. *Question:* Where does the woman in her late forties go for this kind of information, if she is not on this part of TikTok? The brand said it wants to test "All different ages of moms with ages of kids," and this feed is quietly telling it that one of those ages is somewhere else. Territory: **Personas**.

**4. Why does this category's organic run almost entirely without music?**
Ten of the 19 relevant videos are explicitly noted as having no background music, and exactly one uses a music bed as a real choice. The brand's own biggest paid winner opens on an acoustic track playing mid-phrase over a silent shot, with no spoken line until 0:18. Pull: **surprise**. It fired because the standard warning about organic inspiration is that the audio cannot be licensed, and in this category there is almost no audio to license. *Question:* What is silence doing for a video about money that a music bed is not? If the answer is that silence signals a real person rather than a produced asset, it changes the sound design brief on every ad the brand makes. Territory: **Messaging**.

**5. What is the mental load worth as an angle, when nobody in the category has taken it?**
The team's own Reddit research named the mental load as an untouched angle — the hours on hold, the EOBs, the prior authorisation fights. After reading 23 category videos I found no video that takes it as its subject. Pull: **gap**. It fired when a whitespace the team identified from one source survived a completely independent second source without a single counter-example. *Question:* How much demand is sitting behind the invisible work of managing a family's insurance, and who is feeling it hardest? The brand's lead ICP is defined by carrying more than anyone can see, so an angle nobody in the category speaks to may be the closest thing to open ground it has. Territory: **Messaging**.

**6. Why does this category's attention concentrate so hard on pregnancy when the brand's account never goes there?**
Twelve of the 19 relevant videos are anchored to pregnancy, delivery or a baby's first year, including the three largest by view count. The brand's ad library returns zero matches for the word "pregnant" across every field, lifetime. Pull: **pattern**. It fired when the same anchor kept reappearing across creators with no connection to each other, and then the account search came back empty. *Question:* What is it about the pregnancy window that makes people in this category actually stop and listen to insurance information? The brand's guardrail bars pregnancy-only targeting but not a single ad about a trigger moment, so the size of the answer decides whether that guardrail is currently protecting the brand or costing it. Territory: **Product**.

**7. What are the moms in these comment sections actually saying?**
Two videos in the library have comment rates of 1.79%, roughly twelve times the library's typical rate, and both are pure laments with no solution attached. Parker holds the comment counts and not one comment body. Pull: **curiosity**. It fired when the two highest-conversation videos in the library turned out to be the two that offered the least, which is the opposite of what I expected. *Question:* What do people write underneath a video that only names the problem? Those replies are the closest thing this brand has to a free focus group in its exact category, and right now Parker can count them but cannot read them. Territory: **Messaging**.

**8. What would a licensed partner agent on camera do for this brand?**
The brand's whole model routes to real licensed advisors, its compliance rules require a real credential for any doctor character, and no ad in the account has ever put one of those advisors on screen. The category's biggest video is a credentialed person doing credentialed work in public. Pull: **gap**. It fired when I read the compliance rule about doctor characters and realised the brand already owns a credential it has never once shown. *Question:* Who among the brand's partner agents would be willing and able to appear on camera, and what would they be allowed to say? Only the brand can answer this one, and it gates the two strongest candidates in this doc. Territory: **Creators and talent**. **Routed to the brand.**

---

## Appendix - Parker media links

**M001** — @drashleehendry, "Pregnancy Self pay pricing." 6,200,000 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=a15b7ef7-b29d-467f-8498-893c832bf05a&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@drashleehendry/video/7571648042147908894` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7571648042147908894_1788468281/7571648042147908894_join_me_as_i_call_around_and_get_self_pay_pricing_.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7571648042147908894_1788468281/thumbnail.jpg` — Discussed in: Recent viral videos 14, scripts 1, hooks 1, visuals, cross-check, candidates 1, 2 and 3.

**M002** — @paumod, "PSA IF YOU'RE PREGNANT do this before you start shopping." 916,200 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=94e28178-adf8-4ee5-9de1-a274f54dddf7&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@paumod/video/7593050209676987662` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7593050209676987662_1777257347/7593050209676987662_if_you_have_health_insurance_they_may_cover_matern.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7593050209676987662_1777257347/thumbnail.jpg` — Discussed in: Recent viral videos 10, scripts 5, hooks 2, memory connections, candidate 8.

**M003** — @kaseyjaneanderson, "WE DON'T HAVE HEALTH INSURANCE family of 4." 872,100 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=731bd1a3-8c13-4faa-8c54-ccdce1503972&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@kaseyjaneanderson/video/7616717859724545311` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7616717859724545311_1779072506/7616717859724545311_ive_wanted_to_make_this_video_for_so_long_but_was_.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7616717859724545311_1779072506/thumbnail.jpg` — Discussed in: Recent viral videos 8, scripts 3, hooks 3, candidate 9.

**M004** — @salina_sunshine, "My son went to the emergency room and the bills started to pile up." 235,800 views. Political advocacy, off-brief. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=82407e0c-f8d6-43a4-b320-88f48775a5ba&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@salina_sunshine/video/7680344555161521421` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7680344555161521421_1788468674/7680344555161521421_how_are_we_supposed_to_keep_up_with_all_of_these_c.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7680344555161521421_1788468674/thumbnail.jpg` — Discussed in: Recent viral videos 1, memory connections.

**M005** — @readra21, the itemised bill panned top-down. 213,100 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=d4293d9f-8006-49df-9a76-a9abff310d2b&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@readra21/video/7572985864435879181` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7572985864435879181_1788468482/7572985864435879181_selfpaynoinsurance_emergencyroom.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7572985864435879181_1788468482/thumbnail.jpg` — Discussed in: Recent viral videos 13, underperformers, hooks 4, visuals, candidate 3.

**M006** — @friencine, "A HILL I WILL DIE ON A SECOND TIME MOM!" 175,800 views. Highest like, share and save rates in the library. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=484c7ffd-b990-4ae4-96a9-7c73313736c0&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@friencine/video/7584916120965008671` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7584916120965008671_1788468783/7584916120965008671_when_i_was_pregnant_with_my_first_i_missed_out_of_.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7584916120965008671_1788468783/thumbnail.jpg` — Discussed in: Recent viral videos 11, scripts 2, hooks 5, visuals, creator demographics, candidate 4, open loop 2.

**M007** — @kclairemoore, "HAVING A BABY IN 2026." 131,200 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=f90a6870-b22b-42d1-8b7b-0c9316d2b6ba&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@kclairemoore/video/7567018980993469710` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7567018980993469710_1773512819/7567018980993469710_ever_heard_of_indemnity_insurance_for_moms_its_the.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7567018980993469710_1773512819/thumbnail.jpg` — Discussed in: Recent viral videos 15, hooks 6, visuals, candidate 6.

**M008** — @asap.kristy, the two-number bill reveal. 120,200 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=ae99a5dd-5102-41c2-becb-59c9c414c747&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@asap.kristy/video/7536693373290270007` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7536693373290270007_1788469019/7536693373290270007_revealing_how_much_i_pay_for_my_monthly_doctor_vis.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7536693373290270007_1788469019/thumbnail.jpg` — Discussed in: Older carryovers 16, scripts 9, hooks 7, visuals, candidate 8.

**M009** — @camryunique, "Medicaid coverage during pregnancy." 105,300 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=30d88788-cc8d-4603-ac03-286a3cc62ce3&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@camryunique/video/7645420799112842527` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7645420799112842527_1788469022/7645420799112842527_medicaid_during_pregnancy_pregnant_pregnantlife_me.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7645420799112842527_1788469022/thumbnail.jpg` — Discussed in: Recent viral videos 5, hooks 8, visuals.

**M010** — @goojiepooj, the United Healthcare story in a purple robe. 83,900 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=ce352ab0-932e-4c98-a24b-deaf5c6e4b50&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@goojiepooj/video/7444916814754237742` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7444916814754237742_1788468784/7444916814754237742_literally_scared_to_check_my_credit_unitedhealthca.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7444916814754237742_1788468784/thumbnail.jpg` — Discussed in: Older carryovers 18, hooks 9, visuals, memory connections.

**M011** — @bestkeptprivate, remote life insurance sales income. 56,500 views. Scored Not Relevant. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=d0d4e361-9824-4deb-8891-64bc3df7312b&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@bestkeptprivate/video/7658794981456432397` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7658794981456432397_1788468482/7658794981456432397_everyone_asks_what_remote_life_insurance_sales_act.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7658794981456432397_1788468482/thumbnail.jpg` — Discussed in: Recent viral videos 2.

**M012** — @itsliterallyjustliz, "finally quitting the insurance industry after 3.5 years." 41,200 views. Scored Potentially Relevant. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=3219be85-cd3b-4523-b10c-cc101a7bed59&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@itsliterallyjustliz/video/7624310816052972813` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7624310816052972813_1786762160/7624310816052972813_heres_why_lifeinsurance_virtualsales_sales.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7624310816052972813_1786762160/thumbnail.jpg` — Discussed in: Recent viral videos 7, visuals.

**M013** — @molly_daw, "Hey, how are y'all affording kids?" 31,200 views. Joint-highest comment rate in the library. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=c284bf02-419e-4332-a8a9-aae37bcc4704&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@molly_daw/video/7576033059330329886` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7576033059330329886_1788468277/7576033059330329886_are_we_not_living_in_the_same_economy_childlessmil.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7576033059330329886_1788468277/thumbnail.jpg` — Discussed in: Recent viral videos 12, underperformers, scripts 4, hooks 10, memory connections, candidate 5, open loop 7.

**M014** — @insurancebyalexa, "HAVE YOU HEARD OF THE 'FAMILY GLITCH'?" 29,000 views, posted 2022-12-02. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=f61d6671-3d49-4e61-96d1-97a730a56ca4&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@insurancebyalexa/video/7172410850244988206` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7172410850244988206_1788468596/7172410850244988206_is_your_employer_health_insurance_too_expensive_i_.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7172410850244988206_1788468596/thumbnail.jpg` — Discussed in: Older carryovers 22, hooks 11, visuals.

**M015** — @dannitangie, the green-screened bill walkthrough. 28,200 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=9723d817-f5c9-46d8-829f-996332d76784&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@dannitangie/video/7611735950615498014` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7611735950615498014_1788469122/7611735950615498014_how_much_did_you_pay_for_your_delivery_i_had_a_won.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7611735950615498014_1788469122/thumbnail.jpg` — Discussed in: Recent viral videos 9, scripts 8, hooks 12, visuals, cross-check.

**M016** — @adulting_with_kim, the comment sticker answered from a car. 25,500 views. Lowest like rate, fourth-highest comment rate. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=3b443979-1d81-4537-a25c-a9f44715c240&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@adulting_with_kim/video/7431177503483415839` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7431177503483415839_1788468595/7431177503483415839_replying_to_madratterr_the_affordable_care_act_mad.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7431177503483415839_1788468595/thumbnail.jpg` — Discussed in: Older carryovers 21, scripts 10, hooks 13, creator demographics, candidate 7.

**M017** — @kennyslifejourney, "$300 out of each check for some medical." 21,300 views. Joint-highest comment rate. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=2204a185-fb6d-4470-9f62-efd10d301e93&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@kennyslifejourney/video/7442341495849471275` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7442341495849471275_1788468916/7442341495849471275_is_it_just_me_or_is_that_way_too_expensivelike_why.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7442341495849471275_1788468916/thumbnail.jpg` — Discussed in: Older carryovers 19, scripts 7, hooks 14, visuals, memory connections, candidate 6.

**M018** — @camryunique, "What Medicaid pays for during pregnancy." 20,200 views. Third-highest save rate. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=1368ee20-a5a2-4dff-8040-da1bc9b4b88b&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@camryunique/video/7656091476400672031` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7656091476400672031_1788469018/7656091476400672031_medicaid_benefits_save_and_share_with_someone_who_.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7656091476400672031_1788469018/thumbnail.jpg` — Discussed in: Recent viral videos 3, hooks 15.

**M019** — @venteurhealth, "Pros and Cons of getting a HDHP." 14,700 views. Scored Potentially Relevant. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=f8ca67e9-24a8-40f2-aa48-7cd0085c5b13&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@venteurhealth/video/7437207239217319214` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7437207239217319214_1788468410/7437207239217319214_everything_you_need_to_know_about_high_deductible_.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7437207239217319214_1788468410/thumbnail.jpg` — Discussed in: Older carryovers 20.

**M020** — @yolys.world, the Aetna maternity review. 14,700 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=19a1fcb8-fa59-40fb-b9a5-f76ba6590777&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@yolys.world/video/7629381899118546206` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7629381899118546206_1788468778/7629381899118546206_if_youre_pregnant_and_searching_for_solid_insuranc.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7629381899118546206_1788468778/thumbnail.jpg` — Discussed in: Recent viral videos 6, hooks 16, visuals.

**M021** — @amandatalksalot, the single mom by choice budget spreadsheet. 14,400 views. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=8311a25c-dbdd-48b4-8ae9-b0da327be0ac&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@amandatalksalot/video/7538841869065768247` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7538841869065768247_1788469125/7538841869065768247_dont_let_my_numbers_scare_you_go_through_your_expe.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7538841869065768247_1788469125/thumbnail.jpg` — Discussed in: Older carryovers 17, visuals, memory connections.

**M022** — @nothingeversticks, "Do you really know what your health insurance pays for?" 13,100 views. Zero shares. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=9d665f4b-7c17-4ff0-9ac8-03d35c5ee0c8&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@nothingeversticks/video/7651751227738410253` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7651751227738410253_1788110408/7651751227738410253_picking_a_health_insurance_plan_is_so_much_fun_sin.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7651751227738410253_1788110408/thumbnail.jpg` — Discussed in: Recent viral videos 4, underperformers, scripts 6, hooks 17, candidate 5.

**M023** — @fweinations, the sermon about caring for the body. 12,700 views. Scored Not Relevant. Parker: `https://app.heyparker.ai/dashboard/inspiration?video_report=24590a36-09a4-4738-a7f6-e8815defdebf&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — TikTok: `https://www.tiktok.com/@fweinations/video/7441944206538526007` — Media: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7441944206538526007_1788468679/7441944206538526007_young_believer_take_care_of_your_body_you_see_the_.mp4` — Thumbnail: `https://auth.heyparker.ai/storage/v1/object/public/tiktok-videos/7441944206538526007_1788468679/thumbnail.jpg` — Discussed in: Older carryovers 23.

**M024** — Brand ad `MOMS38 - 2 - V3`, ad 120239427583990519, ad set "Moms38 - 2 - 1 (when you call your insurance)." The scripted insurance call. Highest hold rate in the account at 24.48%. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239427583990519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/ac618198a35cfeb2673e5da1357fffe956395a61101a1885c2e462f2e58c1319.mp4` — Discussed in: Cross-check, candidate 1, open loop 1.

**M025** — Brand ad `MOMS38 - 3 - V7`, ad 120239479306030519, ad set "Moms38 - 3 - 2 (20k skit v2)." The scripted hospital call. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239479306030519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/35982b822033f7ab69446f18f2bea3d3c239c04b07167f7bcf76f4ec4e9c577e.mp4` — Discussed in: Cross-check, candidate 1, memory connections.

**M026** — Brand ad `MOMS30 - 1 - V20`, ad 120238476016180519. The silent pediatrician in the lab coat. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238476016180519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1138af6ab844716ddbcd78a371c0ea9d4897abfc8c71f84bbdadbee2a0bdd3b8.mp4` — Discussed in: Recent viral videos 14, cross-check, candidate 2.

**M027** — Brand ad `OMC-Health for Moms-[B2-C13-V2]`, ad 120232148579730519. The "You" versus "Your Insurance" roleplay. $16.65 CPL. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120232148579730519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/9bf849939ff17a428d03fe393e2bf60286e71ffbac9217b0201c7e4f6fd4dd14.mp4` — Discussed in: Cross-check.

**M028** — Brand ad `MOMS38 - 5 - V2`, ad 120239495413420519. "My son fell off the monkey bars at school." The distress lane. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239495413420519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6fbec056c87dc34a3c90d04c81c17579845941a4f1272ba439cabf927f8eca9e.mp4` — Discussed in: Cross-check.

**M029** — Brand ad `MOMS25 BLAST - X1 - Copy 2`, ad 120238476008110519. The podcast microphone format. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238476008110519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/f3e0c6f7927f739d7e793d498cbd16e18af569e78e8ee6c0c943c20fec7d23c0.mp4` — Discussed in: Cross-check.

**M030** — Brand ad `Moms43 - 4 - V3`, ad 120241073380060519. The POV husband hook, the account's top spender, 3.30% hold rate. Dashboard: `https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977` — Video: `https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4` — Discussed in: Cross-check, visuals, open loop 4.

*this is based on everything I have learned about adapting and re-writing scripts*

*this is based on everything I have learned about visuals in advertising*
