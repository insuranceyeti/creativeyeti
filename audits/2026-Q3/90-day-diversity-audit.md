---
brand: health-for-moms
doc: 90-day-diversity-audit
quarter: 2026-Q3
generated_on: 2026-09-03
refresh_by: 2026-12-02
date_range: 2026-06-06 to 2026-09-03
prior_window_compared: 2026-03-08 to 2026-06-05
data_sources_read: [live ads manager via Parker MCP search_facebook_ads_sql against Meta ad account HealthForMoms act 484897827497337, Parker MCP AI format tags (ad_format category), Parker MCP get_brand_persona brand context document, Parker MCP search_competitor_facebook_ads (tracked library empty; wider ad-library corpus used instead), Parker MCP search_chat_history, running-notes/missing-context.md, running-notes/brand-rules.md, running-notes/success-definition.md, audits/2026-Q3/90-day-performance-audit.md]
prior_quarter_audit: none. This is the t0 baseline run. Trajectory is built by pulling the prior 90-day window directly rather than by carrying a prior audit forward.
formats_active_this_quarter: [POV, Social Interface, Callout, Mashup, Comment Response, Other, UGC Single, Skit, Educational, Graphic Video, AI Animation, Wall of Text, Stitch Hooks, Green Screen, Podcast]
formats_dropped_since_prior_quarter: [Authority Figure, Street Interview, Infomercial / VSL, Humour, Offer Based, B-roll mashup + Voiceover]
formats_new_this_quarter: [Graphic Video]
data_limitations:
  - "AI format tags cover 80 of the 147 ads that carried delivery in the window, or 54.4 percent by count. Those 80 ads carry $93,551.24 of the $99,266.98 spent, or 94.2 percent. So every count share in this doc is a share of the 80 tagged ads, not of all 147, while every spend share is a share of total account spend. The 67 untagged ads are almost all tiny spenders. This is a tagging-coverage gap, not a creative finding."
  - "Ads carry more than one format tag. The 80 tagged ads carry 112 format tags between them, about 1.4 each. That means count shares and spend shares both sum to more than 100 percent across formats, and a dollar spent on an ad tagged both POV and Callout is counted once under each. Read each format's spend share as the share of account spend that touched that format, never as a slice of a pie."
  - "The brand's tagged inspo, affinity and competitor libraries are all empty. A live pull returned zero tracked external brands. Section three is therefore anchored to real ads found in the wider Parker ad-library corpus rather than in a library this brand curated. Those are genuine live ads with genuine links, but nobody at Health For Moms picked these brands as reference points, so the slate is narrower and less brand-fitted than it would be with a real library behind it."
  - "External ads carry Meta Ad Library impression rank, not spend. Rank is a proxy for delivery volume, so read a rival's rank-1 ad as its most-delivered ad, never as a known revenue winner."
  - "Hook rate and hold rate are not returned at account or format level. Both are reported here as spend-weighted figures computed across each format's top-spending ads, with the coverage share named on every use."
  - "ROAS is not reported anywhere in this doc. The account is lead generation with zero purchase events, so ROAS reads 0 on every ad and reporting it would be a fabrication. The metric headers in section two substitute cost per lead, which is the brand's stated north star."
  - "Lead quality is invisible to Parker. It lives with the partner insurance agencies. Every efficiency read below clears gate one of the brand's two-gate winner definition only."
  - "Northbeam is not connected. All attribution is Meta-reported on the Meta default window."
  - "No prior 90-day diversity audit exists, so there are no prior-quarter recommendations to score and no prior open loops to close."
---

# 90-day creative diversity audit (format) — Health For Moms — 2026-Q3

> **CORRECTION, 2026-09-04, verified by lifetime pull.** This audit states that the account has run
> **zero static ads, ever**. That is wrong, and the error is a window artifact — the claim is true of
> the 90-day window it read and false of the account.
>
> Lifetime returns **529 static ads, $168,907.73 spend, 13,735 leads at a $12.30 CPL** — the cheapest
> lead source in this brand's history, against a video CPL of roughly $22. Of that, **$74,539.28 ran
> in the last 365 days and $0.00 in the last 180.**
>
> So statics are **production-proven and dormant**, not untested. The recommendation changes
> accordingly: this is not "try a new format," it is "restart a format that already worked at half
> the cost." Their established grammar is a black frame with white type — either a dark-mode fake X
> post or a serif "Moms...." hook.
>
> The same window artifact applies to **street interviews**, which this audit lists as a dropped
> format. A tag-filtered pull plus a frame-level read of `Moms40 - 3 - V4` shows a branded-mic
> street interview with a male presenter and two women in one shot. Public locations, a man on
> camera, two people in frame and unscripted-sounding strangers therefore all sit in the **proven
> baseline**, not on the frontier — which materially changes where the adjacent-versus-out-of-play
> line falls for this brand.
>
> The rest of this audit's findings — the collapse to 70.6% POV spend, the format count falling 20 to
> 15, and the inverse relationship between spend and hold rate — are unaffected and stand.


## Executive summary

The account has one format now. Over the 90 days from June 6 to September 3, 2026, ads tagged `POV` touched $70,052.94 of the $99,266.98 the account spent, which is 70.6 percent. In the prior 90 days that same format touched 12.2 percent. **Verified** from AI format tags on two matched pulls from the Meta account HealthForMoms, act 484897827497337. Nothing else is close. `Social Interface` is second at 15.8 percent and `Callout` third at 12.8 percent, and because ads carry more than one tag, most of the Callout money is sitting on ads that are also POV. Strip that overlap out and roughly seven of every ten dollars in this account went to one creative container: a warm home scene, a mother with a small child, a text overlay that starts with the letters POV, and often no spoken words at all.

The format list itself got shorter. The account ran 20 distinct formats last quarter and 15 this quarter. Six vanished and only one arrived. Gone are `Authority Figure`, `Street Interview`, `Infomercial / VSL`, `Humour`, `Offer Based`, and `B-roll mashup + Voiceover`. The one arrival is `Graphic Video`, a single claymation ad worth $381.82. **Verified** by comparing the format tag sets across both windows. That matters more than a tidy count, because the brand told us in its own intake that the problem it wants solved is exactly this: *"Right now we're mainly on iterations of our state angle that you will see in the account doing well. But not a ton of creative diversity."* **Stated**, brand context document, Section 10. Since that was said, diversity has gone down, not up.

Here is the finding worth acting on, and it is uncomfortable. In this account, the formats that hold attention are the ones getting no money, and the format getting all the money holds nobody. POV runs a spend-weighted hold rate of 3.21 percent across the ten POV ads that carry 99.7 percent of POV spend. Meanwhile `Graphic Video` holds 13.59 percent, `Educational` holds 12.61 percent, the untagged `Other` bucket holds 11.49 percent, and `Skit` holds 11.08 percent. Those four formats together touched 3.7 percent of account spend. **Verified** from ad-level video metrics, spend-weighted, with per-format coverage named in section two. The glossary floor for a healthy hold rate is 12 to 15 percent. Every format that clears or nearly clears that floor is being starved, and the three formats that take 88.8 percent of the money, once their tag overlaps are netted out, all sit under 6.4 percent, with two of the three under 3.3.

The single biggest blank is that this account has never run a static ad. Zero. A filtered pull for image creative across the 90 days returned no rows at all. **Verified.** The brand said statics are welcome for angle discovery: *"We want to focus mostly on video ads. MAYBE some image ads are fine to find angles."* **Stated**, brand context Section 11. Nobody took the offer. That is a real gap, because the five insurance and finance lead-gen brands in the wider ad library all run large static libraries, and `Headline Only` is the top static format at Ethos at 35.0 percent of 856 statics, at Lemonade at 52.8 percent of 282, and at NerdWallet at 33.7 percent of 817. **Verified** from brand-level tag distributions returned on a live library pull.

The lead recommendation for next quarter's test slate is `Interactive`, anchored to Insurify's rank-1 static of stacked age-range buttons that each say "See prices." It is the highest-conviction call on the list because it is not a new idea for this brand, it is the brand's own proven state angle rebuilt as something a mom can tap. Behind it come `Authority Figure` carried by a real licensed advisor rather than a doctor, then `Headline Only` statics to break the zero, then `Us vs Them`, then `Street Interview`. All five are on the brand's own stated list of formats it wants to test, and all five are anchored below to a specific live ad with a link.

## Current ad formats used

Before the format walk, three things about how to read these numbers. First, the denominators. AI format tags cover 80 of the 147 ads that carried delivery in this window, so every count share below is a share of those 80 tagged ads. Those 80 ads carry $93,551.24 of the $99,266.98 spent, or 94.2 percent, so the spend picture is nearly complete even though the count picture is not. Second, the double counting. Those 80 ads carry 112 format tags between them, about 1.4 tags each, so shares sum past 100 percent and a POV ad that is also a Callout shows up in both. Read a format's spend share as "the share of account money that touched this format." Third, the missing metric. The audit template asks for average ROAS in each metric header. This account has zero purchase events by design, so ROAS reads 0 everywhere and quoting it would be a fabrication. Cost per lead is substituted throughout, graded against the brand's own stated tiers: under $15 fantastic, $15 to $20 good, $20 to $25 meh, over $25 not good. **Stated**, brand context Section 11.

The distribution, stated plainly. By spend, POV took 70.6 percent, Social Interface 15.8, Callout 12.8, Mashup 5.2, Comment Response 2.9, Other 2.1, UGC Single 0.7, Skit 0.7, Educational 0.5, Graphic Video 0.4, AI Animation 0.1, and Wall of Text, Stitch Hooks, Green Screen and Podcast rounded to 0.0 apiece. By count of the 80 tagged ads, POV took 31.2 percent, Social Interface 30.0, Callout 26.2, Educational 8.8, Skit 7.5, and then Comment Response, UGC Single and Stitch Hooks at 6.2 each, Other and AI Animation at 5.0, Green Screen at 2.5, and Mashup, Graphic Video, Wall of Text and Podcast at 1.2 apiece.

The gap between those two lists is the story of the quarter. POV holds 31.2 percent of the ads and 70.6 percent of the money. Social Interface holds almost the same share of ads, 30.0 percent, and gets 15.8 percent of the money. Educational holds 8.8 percent of the ads and gets 0.5 percent of the money. Read through the breakdown effect in `ad-account-analysis.md`, that is not a mistake anyone made by hand. Meta pushed budget toward the pocket it predicted would stay cheapest, and POV is where it landed. **Inferred** from the concentration pattern against a shrinking format menu, not from any delivery readout Meta exposes. But the same doc is clear that the top spender is Meta's own verdict on the account's most potent creative, and this verdict was cast against a shrinking, narrowing menu. Seven of every ten dollars went to one container because there was not much else in market to spend it on.

Against the prior 90 days, the movements are large. POV rose from 12.2 percent of spend to 70.6. `Other` collapsed from 36.9 percent to 2.1. `Social Interface` slipped from 22.6 to 15.8. `Stitch Hooks` went from 8.8 percent and $32,885.20 to effectively nothing, $8.14 across five ads. `Skit` fell from 8.1 percent to 0.7. `Educational` fell from 3.2 percent to 0.5. `Callout` rose from 8.8 to 12.8. Six formats left the account entirely and one arrived. **Verified** from matched tag pulls on both windows. The account did not just concentrate. It also stopped trying things.

One more read before the walk. The account is 100 percent video. A filtered pull for image creative returned zero ads across the whole 90 days. **Verified.** So there is no static section below, because there is nothing to write about. Per the funnel-stage caveat in `ad-account-analysis.md`, statics usually skew toward the bottom of the funnel and demand capture, which means this account has no bottom-of-funnel format at all and every dollar is being asked to do cold-audience work through a video opener.

### POV

- Count share: 25 of 80 tagged ads, 31.2 percent
- Spend share: $70,052.94, 70.6 percent of account spend
- Cost per lead: $21.31 across 3,287 leads. Brand tier: meh
- Spend-weighted hook rate: 44.46 percent (top 10 ads, 99.7 percent of format spend)
- Spend-weighted hold rate: 3.21 percent (same basis)
- Trajectory: risen hard. 12.2 percent of spend prior quarter to 70.6 percent now

POV is doing all of this account's acquisition work, and it is doing it with a single line of text. Per `ad-formats/both/index.md`, the format is defined by a literal cue: the characters POV appear on screen followed by a situational statement. That is a thin definition, and it is worth saying out loud that POV describes a text convention rather than a creative container the way `Skit` or `Street Interview` do. What actually unifies these 25 ads is not the format tag, it is one sentence. Seven of the ten highest-spending POV ads, carrying $63,394.54 of the format's $70,052.94, run some version of the same overlay: *"POV: Telling your husband you found better health insurance, saved $400 a month, AND the deductible is zero. Wife of the year energy."* The account's largest ad by far, `Moms43 - 4 - V3` at $43,002.86, opens on a mother and baby lying in bed on white bedding, looking peacefully into the camera, soft beige background, and the verbal hook field reads "None (music only)." **Verified** from its full media fields.

Judged against the bar in `killer-performance-ads.md`, this is a format doing the first job brilliantly and the second job not at all. The 44.46 percent spend-weighted hook rate is well above the 30 percent floor and near the 45 percent ceiling that doc describes as strong. People stop. Then, in the words of the 80/20 rule, seconds one through three owe the viewer a reason to keep watching and seconds three through five owe them the best benefit or a re-hook, and a silent lifestyle montage delivers neither. Average play time on the top ad is 4.04 seconds. Hold rate sits at 3.21 percent against a 12 to 15 percent floor. The ad wins the thumb and then has nothing to say to the person it just stopped.

The trajectory inside the format is worth watching too, because it is not uniformly bad. The two newest POV builds, `moms-63 2b` and `moms-63 3e`, both created August 14, swap the bedroom for a mother and young son walking out of a house, and they return cost per lead of $13.26 and $15.47. **Verified** from ad records. Those are the brand's fantastic and good bands, against $22.24 on the giant bedroom ad. So the format is not exhausted, the specific execution is. What the account has been buying at scale is the oldest POV asset, created April 15, and what it has been starving is the newer POV work that converts cheaper. Both of those newer ads still hold badly, at 2.39 and 2.87 percent, so they clear gate one of the brand's winner definition on cost and say nothing yet about gate two, lead quality, which Parker cannot see.

### Social Interface

- Count share: 24 of 80 tagged ads, 30.0 percent
- Spend share: $15,684.05, 15.8 percent of account spend
- Cost per lead: $26.49 across 592 leads. Brand tier: not good
- Spend-weighted hook rate: 35.68 percent (top 8 ads, 98.9 percent of format spend)
- Spend-weighted hold rate: 6.35 percent (same basis)
- Trajectory: fallen. 22.6 percent of spend prior quarter to 15.8 percent now

Social Interface is the account's second engine and its most interesting one. Per `ad-formats/both/index.md`, the format is defined by a recognizable platform interface appearing inside the creative, and here it is almost always the same device: a viral-style tweet or X post about health insurance, pasted over a woman talking to camera. The recurring artifact is a complaint post reading *"My deductible is $6000... I have to pay $6000 before my insurance even kicks in...but yet...I pay $1000/mo for that insurance?! Make that make sense..."* The top spender in the format, `Moms43 - 5 - V1` at $10,125.67, is a selfie video with that screenshot laid over it and the spoken opener *"This is why you can't simply just say 'Oh, I have insurance, I'm covered.'"* **Verified** from its media fields.

This format holds people roughly twice as well as POV, at 6.35 percent against 3.21, and its top ad holds at 7.59 percent with a 2.14 percent CTR against the account's 1.80. The reason is mechanical and it is worth naming. The tweet overlay is borrowed proof. It puts someone else's grievance on screen in the first frame, which gives the viewer something to read while the creator starts talking, and it makes the complaint feel found rather than written. That is the format doing real work, not decoration.

And yet the money is leaving it, from 22.6 percent of spend down to 15.8, and its blended cost per lead of $26.49 sits in the brand's not-good band. Those two facts pull against each other and the honest read is that the format is being judged on a blended number that one bad ad is wrecking. `Moms Nahuel WV#1 - V9 - Copy` spent $1,639.35 for six leads, a $273.23 cost per lead, and it drags the format average up on its own. Strip it and the remaining Social Interface spend converts far closer to the account norm, with `MOMS39 - 2 - V2 - Copy` at $18.95 and `Moms Nahuel WV#1 - V9 - Copy` in its other ad set at $19.25. The format is not broken. One ad inside it is, and the format is being punished for it. **Inferred** from the per-ad cost spread inside the format, not from anything the account states.

### Callout

- Count share: 21 of 80 tagged ads, 26.2 percent
- Spend share: $12,695.46, 12.8 percent of account spend
- Cost per lead: $19.99 across 635 leads. Brand tier: good, at the very edge
- Spend-weighted hook rate: 37.32 percent (top 8 ads, 97.1 percent of format spend)
- Spend-weighted hold rate: 2.88 percent (same basis)
- Trajectory: risen modestly. 8.8 percent of spend prior quarter to 12.8 percent now

Callout is the best-converting format in the account and almost nobody is treating it as a format. Per `ad-formats/both/index.md` it is defined by the hook directly addressing a specific audience or life stage in second person, and at $19.99 per lead it is the only format above trivial spend sitting in the brand's good band. That is a full $2.65 cheaper per lead than the account's $22.64, and $6.50 cheaper than Social Interface. **Verified** from a tag-filtered pull.

The catch is that Callout barely exists on its own here. Of its $12,695.46, some $7,734.68 sits on ads that are also tagged POV and $2,459.32 on ads also tagged Social Interface. So most of what looks like Callout performance is really a POV ad whose overlay happens to name its audience. That is still a finding, and a useful one: the POV ads that also call their audience out convert better than the ones that only set a scene. The clearest pure example is `moms-53 3`, the "Approved State List ✔️" ad, a woman in a grey tank top standing in front of a white screen listing US states, opening on the spoken line *"I'm so thankful for the mom that told me about this."* It ran a 3.14 percent CTR, the highest among the top spenders, at a $16.44 cost per lead on $1,956.50. **Verified.**

Hold rate is the weak spot at 2.88 percent, the lowest of the three big formats. So Callout gets the click cheaply and loses the watch. Read against the awareness ladder in `killer-performance-ads.md`, that fits: a callout hook qualifies hard and fast, which is efficient for a lead form but does not carry a cold viewer through a story. This is the format to iterate on for cost and the wrong one to lean on for depth. And on the brand's own two-gate rule, $19.99 clears gate one only. Whether a lead that arrived through a fast qualifying hook holds up downstream is exactly the gate-two question Parker cannot answer.

### Mashup

- Count share: 1 of 80 tagged ads, 1.2 percent
- Spend share: $5,141.80, 5.2 percent of account spend
- Cost per lead: $25.45 across 202 leads. Brand tier: not good
- Hook rate: 46.32 percent (the single ad, 100 percent of format spend)
- Hold rate: 2.38 percent (same basis)
- Trajectory: roughly flat in spend, collapsed in count. 5.3 percent of spend on 2 ads prior quarter, 5.2 percent on 1 ad now

Mashup is a single ad carrying more than five percent of the account. `MOMS34 - N1 - 3a`, created back on February 21, opens on a mother playing hide and seek with her toddler in a bright sunlit hallway, under the overlay *"POV: At peace...because my family finally has the best health insurance and I pay less."* Per `ad-formats/video/index.md`, Mashup means the ad is compiled from multiple independent clips to create volume and variety rather than one linear scene, and that is what this is: a montage of mom moments cut together. **Verified** from its media fields and the ad set name, "MOMS34 - N1 - A (Mom Moment Montage)."

The numbers say the montage approach has run its course in this account. A 46.32 percent hook rate is the third highest among the top spenders, so the opening frame still stops people. A 2.38 percent hold rate is the second lowest of any format here, and a $25.45 cost per lead puts it in the brand's not-good band. The pattern is identical to POV and it comes from the same cause: a wordless sequence of pretty family moments gives the viewer nothing to follow.

What makes this format worth flagging despite its single ad is age. February 21 is more than six months before the window closed, and this ad is still absorbing $5,141.80. The account is not choosing Mashup, it is failing to replace it. Per `iterations.md`, the discipline on a fatiguing asset is to hold the thing that works and vary the thing that does not, and here the thing that works is plainly the opening frame, not the body. A Mashup with the same hide-and-seek opener and an actual spoken script behind it has never been tried.

### Comment Response

- Count share: 5 of 80 tagged ads, 6.2 percent
- Spend share: $2,882.96, 2.9 percent of account spend
- Cost per lead: $28.26 across 102 leads. Brand tier: not good
- Spend-weighted hook rate: 30.76 percent (4 ads with video data, 100 percent of format spend)
- Spend-weighted hold rate: 5.56 percent (same basis)
- Trajectory: risen in share, shrunk in dollars. 1.7 percent of spend prior quarter to 2.9 percent now, but $6,261.31 down to $2,882.96

Comment Response is a small format punching above its weight on attention and below it on cost. Per `ad-formats/both/index.md` the format is built around answering a specific piece of user feedback that is visually displayed, and here it overlaps heavily with Social Interface, since three of the five ads carry both tags. The strongest of them is `Moms43 - 5 - V4`, a woman talking to camera with the $6,000 deductible complaint overlaid, opening on the text hook *"STOP paying your insurance deductibles before you watch this.,, Seriously."* It holds 7.05 percent on $1,393.32, which is more than double the POV average. **Verified.**

The cost picture is worse. At $28.26 per lead the format sits in the brand's not-good band, and its worst ad, `moms54-2`, spent $1,467.48 at $34.94 per lead despite a decent 4.18 percent hold. So this is a format that keeps people watching and then does not convert them at a price the business likes. Read against the hook-to-body contract the brand names in its own guidelines, the likely culprit is the gap between an aggressive stop-what-you-are-doing opener and a body that resolves into the same generic savings pitch every other ad in the account uses.

The trajectory is the interesting part. In dollars this format shrank by more than half. In share of a much smaller account it grew. That is what a format looks like when it is neither killed nor backed: it is still in market, still cheap to keep alive, and nobody has decided anything about it. With five ads and $2,882.96 behind it, there is not enough volume here to settle whether the format works. There is enough to say it holds attention better than the account average and costs more per lead than the account average, and that combination deserves one properly funded test rather than another quarter of drift.

### Other

- Count share: 4 of 80 tagged ads, 5.0 percent
- Spend share: $2,050.72, 2.1 percent of account spend
- Cost per lead: $33.62 across 61 leads. Brand tier: not good
- Spend-weighted hook rate: 53.95 percent (3 ads with full video data, 99.9 percent of format spend)
- Spend-weighted hold rate: 11.49 percent (same basis)
- Trajectory: collapsed. 36.9 percent of spend on 29 ads prior quarter to 2.1 percent on 4 ads now

This is the most important small format in the account, and the tag name hides it. Per `ad-formats/both/index.md`, `Other` is the label applied when no defined format can be confidently assigned. So what is sitting here is creative the taxonomy could not name, and it holds attention better than anything else the account runs at meaningful spend. `moms54-3` opens on a young woman with a red, tear-stained face speaking straight into her phone camera in a tight close-up, visibly distressed, and the first spoken words are *"Just got off a two hour call fighting for them to cover my newborn son's hospital stay."* It ran a 57.02 percent hook rate, a 13.66 percent hold rate and an 8.08-second average play time on $1,283.69. **Verified** from its full media fields and period metrics. Its sibling `moms54-4` opens on a close-up of a woman crying, tears visible, saying *"My son fell off the monkey bars at school and broke his arm."* That one holds 8.62 percent with a 6.94-second play time.

Describe the execution first and then name the closest format, which is what the taxonomy asks for in gray cases. What these ads actually are is a person picking up a phone and talking, raw, unpolished, no graphics, no edit pattern. In `ad-formats/video/index.md` that is `Yapper`, and the reason the tagger did not reach for it is probably that these are scripted and emotionally staged rather than spontaneous. **Inferred**, since the tags cannot name it and the classification here is concluded from the visual hook, verbal hook and play-time signals rather than stated by the source. Either way, this is the only creative in the account clearing the 12 percent hold floor at any real spend, and it is the only creative where average play time crosses eight seconds. Held against `killer-performance-ads.md`, it is the one place the account obeys rule one: it targets an emotion, and the clips match the emotion.

The cost is the other half of the truth and it has to be said in the same breath. At $33.62 per lead, blended, this format is the most expensive in the account, and `moms54-4` came in at $38.09. So deep attention here is not translating into cheap leads. That is a genuine tension, not a rounding error, and it is one of the open loops below. What is not in doubt is the trajectory: the account went from 29 ads and $138,175.25 in this bucket to 4 ads and $2,050.72. Whatever the account was doing last quarter that the tagger could not classify, it has almost entirely stopped doing it, and it stopped doing the thing that held attention best.

### UGC Single

- Count share: 5 of 80 tagged ads, 6.2 percent
- Spend share: $722.40, 0.7 percent of account spend
- Cost per lead: $20.64 across 35 leads. Brand tier: meh, at the edge of good
- Spend-weighted hook rate: 41.13 percent (all 5 ads, 100 percent of format spend)
- Spend-weighted hold rate: 4.27 percent (all 5 ads). Excluding one ad with 135 impressions whose 74 percent hold is noise, 4.14 percent across 99.8 percent of format spend
- Trajectory: fallen in dollars, risen in share. 1.1 percent of spend and $3,939.65 prior quarter to 0.7 percent and $722.40 now

Per `ad-formats/video/index.md`, UGC Single is the fallback label for a single creator making organic-feeling content when no more specific format fits, and that is exactly how it reads here. The format's whole spend is essentially one ad. `moms55-1`, created August 28, is a woman in her thirties wearing large orange-tinted sunglasses and a Budweiser muscle tank, filming from the driver's seat of her car, opening with *"Currently waiting in line to pick up my girls from school, and I'm doing the math on how much I pay for health insurance every single year."* It took $655.43 of the $722.40 and returned a $20.48 cost per lead on a 43.24 percent hook rate. **Verified.**

That ad deserves more attention than its budget suggests, and the reason is the setting. Every other meaningful ad in this account is filmed in a bedroom, a hallway, a kitchen, or a house exterior. This one is filmed in a school pickup line, which is the single most specific mom moment in the account and one the brand's own context document names as a core association: *"Trusted mom friends, family dinner table, school pickup line, pediatrician visits."* **Stated**, brand context Section 7. The account has been advertising the outcome, a peaceful home, and here it briefly advertised the moment, a woman doing math in her car while she waits for her kids.

The hold rate of 4.14 percent is only slightly better than POV, so this is not the fix for the attention problem. What it is, at $655.43 and eleven days in market, is the cheapest live evidence in the account that a plainly-shot single creator in a real place can convert at the good band. Per the evidence-first prioritization in `persona-research-and-creative-strategy-process.md`, that is high-confidence, fast-to-ship work sitting untouched: a proven customer moment already tested at small spend, ready to be redeployed rather than reinvented.

### Skit

- Count share: 6 of 80 tagged ads, 7.5 percent
- Spend share: $698.09, 0.7 percent of account spend
- Cost per lead: $20.53 across 34 leads. Brand tier: meh, at the edge of good
- Spend-weighted hook rate: 27.02 percent (3 ads with hold data, 99.9 percent of format spend)
- Spend-weighted hold rate: 11.08 percent (same basis)
- Trajectory: collapsed. 8.1 percent of spend on 33 ads prior quarter to 0.7 percent on 6 ads now

Skit is the clearest case in this audit of a format being abandoned while it was working. It fell from 33 ads and $30,195.39 to 6 ads and $698.09, a drop of 97.7 percent in dollars. **Verified** across both windows. And what it left behind is a 11.08 percent hold rate, third best in the account, on a $20.53 cost per lead that is better than the account's $22.64.

The surviving ad worth studying is `Moms36 - 3 - A - 2 - V4c - Copy`. A woman looks directly at the camera with a sigh and a frustrated expression, warm domestic lighting, and says *"I wish this was a joke."* The text hook reads *"I wish this was a joke... (health insurance)."* It ran a 11.16 percent hold rate on $671.21 with an average play time of 9.69 seconds, the longest watch time of any ad in this window. **Verified** from its period metrics. For context, the account's biggest ad plays for 4.04 seconds. This one nearly triples that on one hundredth of the budget.

There is also a demographic signal in this format that nothing else in the account produces. Skit put 34.7 percent of its spend on women aged 45 to 54 and only 11.9 percent on 25 to 34. **Verified** from the format's age breakdown. Compare that with POV, which put 43.6 percent on 25 to 34 and 9.4 percent on 45 to 54. Those are close to mirror images. The brand said it wants to test *"All different ages of moms with ages of kids"* and named older second-chapter moms specifically. **Stated**, brand context Section 10. The format that reaches those women best is the one the account almost switched off.

### Educational

- Count share: 7 of 80 tagged ads, 8.8 percent
- Spend share: $511.98, 0.5 percent of account spend
- Cost per lead: $32.00 across 16 leads. Brand tier: not good
- Spend-weighted hook rate: 28.55 percent (5 ads with hold data, 99.6 percent of format spend)
- Spend-weighted hold rate: 12.61 percent (same basis)
- Trajectory: fallen. 3.2 percent of spend on 18 ads prior quarter to 0.5 percent on 7 ads now

Educational is the only format in the account whose hold rate clears the 12 percent floor, and it is getting one dollar in every two hundred. Per `ad-formats/both/index.md` the format teaches the viewer the why behind a problem and lets the product arrive after the reframe, and the execution here is claymation. `Moms46 - V1` opens on a claymation woman at a desk buried in stacks of unpaid bills under a single lamp, looking exhausted, and asks *"Did you know your hospital bill is cheaper if you don't use your insurance?"* It holds 13.59 percent with a 6.77-second play time and a 43.55 percent 15-second retention on $381.82. **Verified.** Its sibling `Moms46 - V2` opens on the same character and the line *"Same scan, same hospital. One price for cash, a much bigger one if you hand over your card."* That one holds 11.15 percent.

This is the account being genuinely good at the thing its own brand guidelines say to be good at. The guidelines name a "pool-pricing mechanic" as the causal explanation for why deductibles are high and instruct that the education beat should explain why rather than define terms. **Stated**, brand context Section 7. These three claymation ads are the only creative in the account that actually does that. They do not tell a mom what a deductible is. They tell her the hospital charges two different prices for the same scan, which is a fact she did not have and cannot unhear.

The problem is cost, and it is real. Sixteen leads at $32.00 apiece puts the format in the not-good band, and the volume is far too thin to call. Per `ad-account-analysis.md`, low-spend ads with unusual numbers should be read carefully rather than crowned, and $511.98 across seven ads is not a verdict on anything. What can be said with confidence is narrower and still useful: at the top of the funnel, where this account is starving, this format holds attention four times better than the one taking 70 percent of the budget, and it has never been given enough money to find out whether that attention converts.

### Graphic Video

- Count share: 1 of 80 tagged ads, 1.2 percent
- Spend share: $381.82, 0.4 percent of account spend
- Cost per lead: $31.82 across 12 leads. Brand tier: not good
- Hook rate: 31.20 percent (the single ad, 100 percent of format spend)
- Hold rate: 13.59 percent (same basis)
- Trajectory: brand new. Absent entirely from the prior quarter

This is the only format that arrived this quarter, and it is one ad: `Moms46 - V1`, the claymation woman at the bill-covered desk described just above. It carries both the `Graphic Video` and `Educational` tags, which is right, since per `ad-formats/video/index.md` Graphic Video means the whole frame is built rather than filmed, with no real people on camera. **Verified** from its visual hook and media fields.

At 13.59 percent it holds attention better than any other ad in the window, and it does so with nobody's face in it. That is worth sitting with, because the account's stated top bottleneck is casting. The brand listed *"Casting/UGC Creators"* as bottleneck number one and *"Production/Filming"* as number four. **Stated**, brand context Section 11. A format that needs no creator, no shoot and no talent release is the one format whose supply is not capped by the constraint the brand says hurts most, and it happens to be the creative that holds attention best in the account.

The honest counterweight is that this is a single ad with twelve leads at $31.82. That is not a performance claim, it is a signal. Per `killer-performance-ads.md`, assumptions are the death of ads and the market has to be allowed to tell you. What this one ad earns is a real budget and three or four more executions, not a conclusion. The trajectory marker "new this quarter" is doing a lot of work in a metric header, and it should read as an invitation rather than a result.

### AI Animation

- Count share: 4 of 80 tagged ads, 5.0 percent
- Spend share: $124.60, 0.1 percent of account spend
- Cost per lead: $31.15 across 4 leads. Brand tier: not good, on volume too thin to grade
- Spend-weighted hook rate: 19.81 percent (2 ads with hold data, 98.2 percent of format spend)
- Spend-weighted hold rate: 9.62 percent (same basis)
- Trajectory: risen from almost nothing to slightly more than nothing. 1 ad and $78.34 prior quarter to 4 ads and $124.60 now

Per `ad-formats/video/index.md`, AI Animation means generated characters that speak, act or carry the story, and the defining feature is character creation rather than product motion. Two distinct concepts sit here. The first is the claymation set, `Moms46 - V2` and `V4`, which are the same bill-covered-desk character discussed above. The second is more inventive: `Animation Agency #4 - H1` personifies the bill itself. A grumpy medical bill with folded arms stands on a blue insurance card on a wooden kitchen counter, and it speaks: *"I am your deductible. And if you think having insurance means your family is covered, listen up."* **Verified** from its visual hook and verbal hook fields.

That is the most creatively ambitious idea in the entire account, and it received $2.19 across two ad sets. Its hook rates of 5.88 and 13.33 percent are the worst in the window, but on 34 and 15 impressions those numbers mean nothing at all. This is not a format that failed. It is a format that was never actually put in market.

The claymation half does have signal: 11.15 and 6.00 percent hold rates, spend-weighted to 9.62. That is roughly three times the POV hold rate. Read alongside Graphic Video, the pattern across all the animated work is consistent and points the same direction. When this account puts something built rather than filmed in front of a mom, she watches longer. The account has spent $506.42 total testing that idea, against $70,052.94 on the format that holds worst.

### Wall of Text

- Count share: 1 of 80 tagged ads, 1.2 percent
- Spend share: $23.49, 0.0 percent of account spend
- Cost per lead: no leads recorded, so no cost per lead exists
- Hook rate: 54.08 percent (the single ad, 100 percent of format spend)
- Hold rate: 3.24 percent (same basis)
- Trajectory: fallen. 3 ads and $2,188.51 prior quarter to 1 ad and $23.49 now

One ad, $23.49, and the second-highest hook rate in the entire window. `MOMS34 - N1 - 4a` shows a mother in a red tank top sitting behind a toddler in a red t-shirt who is jumping on a small white bench, under a long overlay: *"Moms... I used to dread checking the mail because of surprise medical bills. Switched to HealthForMoms. Haven't gotten one since."* It hooked 54.08 percent of viewers. **Verified.**

Per `ad-formats/video/index.md`, Wall of Text means on-screen text dominates and stays fixed while footage plays behind it, so the reading is the experience. On 710 impressions a 54.08 percent hook rate is directional at best, and the 3.24 percent hold and zero leads say nothing survived the read. But the shape of the result is consistent with everything else here: a specific, concrete sentence about dreading the mail stops people harder than a peaceful bedroom does.

The trajectory is a near-death. From $2,188.51 across three ads to $23.49 across one. Nobody decided to kill this format, it simply stopped being made. Given that the brand's own guidelines prize specificity as credibility and name odd exact numbers as more believable than round ones, a text-led format is a natural home for the strongest customer sentences this brand has, and right now it is a rounding error.

### Stitch Hooks

- Count share: 5 of 80 tagged ads, 6.2 percent
- Spend share: $8.14, 0.0 percent of account spend
- Cost per lead: no leads recorded across the format
- Spend-weighted hook rate: 31.59 percent (4 ads with hold data, 98.9 percent of format spend)
- Spend-weighted hold rate: 9.49 percent (same basis)
- Trajectory: the steepest collapse in the account. 19 ads and $32,885.20 prior quarter to 5 ads and $8.14 now

This is the single most dramatic movement in the audit. Last quarter Stitch Hooks was the fourth largest format in the account by spend, at 8.8 percent and $32,885.20 across 19 ads. This quarter it is five ads sharing eight dollars and fourteen cents. That is a fall of 99.98 percent. **Verified** across matched pulls on both windows.

Per `ad-formats/video/index.md`, the format opens with external content and then has the creator respond directly to that specific clip, with the first clip and the response clip visually distinct. What survives in this window are the crying "monkey bars" ads, `moms-65 2d` and `moms-65 2e`, which hold 9.52 and 12.50 percent on $2.78 each. Those hold rates are strong and the spend behind them is meaningless, so they cannot carry a claim. What can carry a claim is the disappearance itself.

An account that spent $32,885.20 on a format one quarter and eight dollars the next either learned something decisive or lost the ability to make it. Nothing in the data says which. Stitch Hooks needs source content to react to, which means it needs someone finding clips and someone filming responses, and both of those sit inside the casting and production bottleneck the brand named. That makes this the format most likely to have died of supply rather than of performance. **Inferred** from the format's production needs read against the bottlenecks the brand named, and carried to an open loop below rather than treated as settled.

### Green Screen

- Count share: 2 of 80 tagged ads, 2.5 percent
- Spend share: $7.95, 0.0 percent of account spend
- Cost per lead: 1 lead at $7.95, on volume far too thin to grade
- Spend-weighted hook rate: 32.36 percent (both ads, 100 percent of format spend)
- Spend-weighted hold rate: 4.26 percent (same basis)
- Trajectory: risen from one ad to two, and from $121.42 to $7.95. Down in dollars, up in count

Two ads, eight dollars. Per `ad-formats/video/index.md`, Green Screen means the creator appears as an overlay on top of other content and the visible layer separation is the format. The stronger of the two, `moms54-6`, is a woman speaking to camera with a screenshot of a medical bankruptcy research paper laid behind her, opening on *"This is why you cannot settle for mediocre insurance."* It holds 4.76 percent on $5.63. **Verified.**

The reason this sliver is worth a paragraph is that Green Screen is the natural next step from the format the account already leans on. Social Interface here is almost always a tweet pasted over a talking head, which is a static overlay. Green Screen is the same move with the creator layered on top of a document she can point at and walk through. The research-paper ad is the account reaching for authority through a source, and it is the only place in the account where a document, rather than a complaint, does the proving.

At $7.95 there is nothing to conclude. There is something to notice: the brand's compliance rules forbid fabricated statistics and require that the villain always be the system rather than a named company. **Stated**, brand context Section 8. A format built on showing a real published source is unusually well suited to a brand that has to make system-level claims it can stand behind, and it has been tested with less money than a sandwich costs.

### Podcast

- Count share: 1 of 80 tagged ads, 1.2 percent
- Spend share: $5.38, 0.0 percent of account spend
- Cost per lead: no leads recorded
- Hook rate: 20.11 percent (the single ad, 100 percent of format spend)
- Hold rate: 4.02 percent (same basis)
- Trajectory: fallen. 4 ads and $227.01 prior quarter to 1 ad and $5.38 now

The smallest format in the account. `Moms43 - 1 - V12` shows a woman in a podcast studio with a tweet graphic overlaid, saying *"Your insurance is not protecting your family."* **Verified** from its media fields. Per `ad-formats/video/index.md`, the format needs visible people in a podcast or interview setting with microphones and studio cues, and it is meant to feel like a conversation between people rather than one person talking to camera beside a microphone.

That last distinction is where this execution falls down, and it is worth being precise about. Looking at the sibling ads `Moms43 - 1 - V13` and `V14`, both show a single woman speaking into a studio microphone in a cozy room. That is a podcast setting without a podcast. There is no second person, no conversation, no interview. The account has borrowed the visual furniture of the format without the thing that makes the format work, which is two people talking and a viewer eavesdropping. **Inferred** from the visual hooks on all three studio ads, each of which describes one person alone.

So the honest read on Podcast is not that it failed. It is that it has not been tried. Five dollars and thirty-eight cents bought one impression-level look at a solo talking head in a studio chair. The brand listed *"Podcast Ads"* on its own stated list of video formats to test. **Stated**, brand context Section 10. A real two-person execution, with a licensed advisor across the table from a mom, remains untested and is a close cousin of the Authority Figure recommendation below.

## Recommended ad formats to test

A note on the sourcing before the slate, because it changes how much weight these carry. This brand has no tagged inspo, affinity or competitor library. A live pull returned zero tracked external brands. **Verified.** So the ads anchoring these recommendations were found in the wider Parker ad library rather than in a set of reference brands this team chose. They are real, live, currently-delivering ads with real links, and the five brands they come from are genuine category neighbors: insurance comparison platforms and financial lead-gen products that run the same match-and-quote model Health For Moms runs. But nobody here nominated them. The slate is narrower for it, and it will get sharper the moment the team adds real competitors and inspiration brands in the Parker app. Every brand-fit judgment in this section is therefore **data-limited**: the formats are anchored in real delivering ads, but the reference set behind them is Parker's corpus rather than this team's considered choice of who to learn from. That is the single highest-value fix available to this section.

One shared piece of evidence sits under recommendations one, three and four, so it is worth stating once. All five external brands run large static libraries, and Health For Moms runs none. Ethos has 856 statics with `Headline Only` at 35.0 percent, Lemonade has 282 with `Headline Only` at 52.8 percent, NerdWallet has 817 with `Headline Only` at 33.7 percent, Insurify has 191 with `Us vs Them` at 29.8 percent, and Compare Rates Today has 545 with `Interactive` at 73.6 percent. **Verified** from brand-level tag distributions returned on a live library pull. Every serious lead-gen advertiser in this category treats statics as core inventory. This account has zero.

### 1. Interactive — highest conviction

**Source ad.** A tall, plain, off-white frame. At the top sits the Insurify wordmark, orange dots over the letter I. Under it a headline in heavy black type reads "Car insurance cost for" and then, in bright orange, "seniors in 2026." Below that, the entire lower two thirds of the ad is a stack of five identical pill-shaped rows. Each row holds an age range in big bold black type, 55-59, 60-64, 65-69, 70-74, 75-79, with the words "years old" trailing in lighter weight. To the right of every row sits a small rounded orange button that says "See prices" in white. There is no photograph, no person, no product. It looks like a calculator someone built, not an ad someone bought.

- Source library: wider Parker ad-library corpus. The brand's own inspo, affinity and competitor libraries are empty
- Source brand: Insurify, an insurance comparison and quote-matching platform
- Reference: https://app.heyparker.ai/dashboard/ad-library?adId=1765001758269651&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/f4a62dbe-bc7a-4f7e-95ae-d1a670038652/1765001758269651.jpg
- Delivery signal: Meta Ad Library impression rank 1, stable at 1 across the seven readings from August 21 to September 2. Launched July 2, 2026, running 63 days

**Conviction: highest, and it is not close.** Per `ad-formats/both/index.md`, `Interactive` means the creative looks like something the viewer can tap, select, or answer even though the creative itself is not interactive. It uses buttons, quizzes, decision paths, or tappable-looking elements. Health For Moms has never run one, and yet the brand already owns the exact mechanism this format is built to carry. The state angle is, in the brand's own words, its best performer: *"State angle has worked very well if you see the account."* **Stated**, brand context Section 9. And the way it currently appears in the account, in `moms-53 3`, is a woman standing in front of a screen listing states while she talks. That is a state list being narrated. This format turns the same list into something a mom can point at.

The gap it fills is the one this whole audit is about. The account is 100 percent video, and every video it runs asks a viewer to watch for four seconds before it says anything useful. Hold rate is the account's broken metric at 3.83 percent spend-weighted. An Interactive static does not have a hold rate to break. It fails or succeeds in the half-second scan that `visuals.md` calls the first job of any visual, and it converts on a tap rather than on a watch. That makes it the only recommendation on this list that routes entirely around the account's worst weakness rather than trying to fix it.

The lever it pulls that nothing in the current mix pulls is self-selection before the click. Every ad this account runs today addresses "moms" as one undifferentiated group, and the delivery data shows the consequence: 81.2 percent of spend lands on a twenty-year age band and the format mix cannot tell a 28-year-old with a newborn from a 45-year-old with teenagers. A row of tappable states, or of family sizes, or of "what my deductible is now" brackets, sorts the viewer before Meta has to guess. On awareness stage this reaches the problem-aware mom who knows her premium hurts but has not decided anything, which is the largest pool the account can address and the one the state angle already proves converts. The nearest category analogue is the strongest evidence of all: Compare Rates Today runs `Interactive` on 401 of its 545 statics, 73.6 percent of its whole static library. **Verified.**

### 2. Authority Figure — high conviction

**Source ad.** A close-up of a woman in navy blue medical scrubs with a white zip-up jacket over them, standing in a brightly lit exam room. She has shoulder-length brown hair and she is looking straight down the lens. Her first line is *"You know it breaks my heart as a veterinarian? When pet parents can't afford the pet care that their pets desperately need."* The camera pans across a clinic counter, sharps container, otoscope on the wall. It cuts to a large grey Old English Sheepdog lying on the clinic floor with a red text box reading "unexpected emergencies." She comes back to camera: *"Trust me when I say the last thing you wanna think about when your pet is really sick is how you're gonna pay for that visit."* Only then, at 21 seconds of a 38-second ad, does a hand appear holding a phone with the product on screen. She closes with *"If you're a pet parent, I strongly recommend insurance."*

- Source library: wider Parker ad-library corpus
- Source brand: Lemonade, pet insurance
- Reference: https://app.heyparker.ai/dashboard/ad-library?adId=2168773877290882&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/27c8be1e-bce2-4ecf-a730-91b3e40b6f9c/2732968667067890.mp4
- Delivery signal: Meta Ad Library impression rank 14, improved from 16 on September 2. Launched April 23, 2026, running 133 days

**Conviction: high.** Per `ad-formats/both/index.md`, `Authority Figure` centers a credible expert whose credentials make the explanation carry weight, signaled through title, setting, wardrobe or spoken intro. Health For Moms ran four of these last quarter for $8,884.74 and ran zero this quarter. It is a dropped format, not an untried one, which raises the confidence: the machinery to make one exists and somebody stopped.

The gap it fills is the account's total absence of anyone qualified on screen. Every single face in this account is a mom talking about her own bill. That is one proof shape, repeated 147 times, and per `killer-performance-ads.md` an ad needs a promise and proof, with credibility and authority named among the elements the video should carry. The brand has a real trust problem to solve here, not a theoretical one: its own context document notes people search *"is Health for Moms legit"* and names the awareness and trust gap as a place the brand loses. **Stated**, brand context Section 6. A peer saying "this worked for me" does not answer a legitimacy question. Someone licensed does.

The lever is credibility transfer, and the specific casting call is the part that makes this fit this brand rather than any brand. The compliance rules say a doctor character requires a real licensed physician or adjusted language that does not imply a false credential. **Stated**, brand context Section 8. So do not cast a doctor. Cast a licensed insurance advisor, which is exactly who the partner agencies employ, and whom the brand already describes as *"like your Mom BFFs - friendly and approachable."* That is an authority figure who is compliant by construction, already part of the funnel, and on-brand in voice. Note what the Lemonade ad does with its 38 seconds: it spends 21 of them establishing the problem through the expert's eyes before the product appears. That is the structural answer to a 3.21 percent hold rate. The category agrees, too. Ethos runs 24 Authority Figure videos and Lemonade runs 9, and it is the top video format for both. **Verified.**

### 3. Headline Only — high conviction

**Source ad.** A vertical photograph of a clinical exam room, shot slightly off-angle. A medical exam table with dark blue vinyl padding runs across the lower half of the frame, a fresh sheet of white crinkle paper draped over it. On the beige wall behind sit an otoscope, an ophthalmoscope and a digital blood pressure monitor with black cords hanging down. The light is bright and sterile. In the top left corner, a small red badge reads "Exclusive." Across the middle of the image, in large bold white type, sits the whole ad: *"Women in their 60s can get $200K life insurance with no med exam for $57/mo through Ethos — find out how."* Below it, in small white text, a disclaimer names the sample rate and the policy terms. There is no person in the photo. The room is the argument: this is the thing you were dreading, and you do not have to do it.

- Source library: wider Parker ad-library corpus
- Source brand: Ethos, term life insurance sold online
- Reference: https://app.heyparker.ai/dashboard/ad-library?adId=1388982813144880&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/fcc3a6f6-46ae-40f4-8071-6341dbd5e1fb/1388982813144880.jpg
- Delivery signal: Meta Ad Library impression rank 1, improved from rank 3 on September 2. Launched August 4, 2026, running 30 days

**Conviction: high.** Per `ad-formats/static/index.md`, `Headline Only` means one dominant headline carries the message with no meaningful benefit list under it. The account has never run a static of any kind, so this is not a format gap, it is a whole modality gap. The brand explicitly permitted it and nobody acted: *"MAYBE some image ads are fine to find angles."* **Stated**, brand context Section 11.

The gap it fills is speed of learning, which is the constraint the brand actually named. Health For Moms listed five creative bottlenecks and four of them, casting, research, production and scripting, are upstream of every video the account makes. A headline static needs none of them. It needs one sentence and one photograph. The brand's stated volume is 1 to 5 net-new concepts a month, which is a very small number of shots on goal for an account trying to scale, and per `creative-strategy-fundamentals.md` and the low-spend-level plays in `creative-strategy-by-brand-size.md`, getting more shots on goal and finding angles is the priority at this stage. Statics are how you take twenty swings in the time a video shoot takes one.

The lever is angle discovery divorced from production, and it unlocks the awareness stage the video mix cannot serve. Look at what the Ethos headline does that no ad in this account does: it names a demographic, a coverage amount, a friction removed and a price, all in one sentence, and then qualifies the claim in small print. Health For Moms already has the raw material for this and is burying it inside 30-second videos. The exact deductible complaint that anchors the Social Interface ads, *"My deductible is $6000... but yet...I pay $1000/mo for that insurance?! Make that make sense..."*, is a headline. The brand's own guidelines say odd specific numbers read as more believable than round ones. **Stated**, brand context Section 7. Compliance is straightforward here as long as savings stay "up to 30%" and the deductible stays "$0 deductible option," exactly as the Ethos ad qualifies its own sample rate. And the category consensus is loud: Headline Only is the number one static format at three of the five brands checked.

### 4. Us vs Them — medium-high conviction

**Source ad.** Three stacked bands. On top, white background, the Insurify wordmark, then a headline reading "Stop overpaying for home insurance." with the word "overpaying" picked out in orange. The middle band is split down the centre. On the left, a grey background, a white pill-shaped bubble reading "$1352/yr Old insurance," and beneath it the left half of an isometric suburban house drawn entirely in grayscale, dull and lifeless. On the right, a bright orange background, a matching white pill reading "$699/yr Insurify," and beneath it the right half of the very same house in full colour, orange siding, white trim, brown shingles, green grass. It is one house, cut in two, half drained and half alive. At the bottom, a wide orange button: "Check my rate."

- Source library: wider Parker ad-library corpus
- Source brand: Insurify
- Reference: https://app.heyparker.ai/dashboard/ad-library?adId=1546880869622488&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/f4a62dbe-bc7a-4f7e-95ae-d1a670038652/1546880869622488.jpg
- Delivery signal: Meta Ad Library impression rank 7, climbed six places from rank 13 over 12 days. Launched August 4, 2026, running 30 days

**Conviction: medium-high.** Per `ad-formats/static/index.md`, `Us vs Them` is a side-by-side static comparing the brand against a competitor, a category alternative, or an old behaviour, with the two sides explicitly contrasted. The brand put "Us vs. Them" on its own list of video formats to test. **Stated**, brand context Section 10. It has never run one in either window.

The reason conviction is medium-high rather than high is a compliance question that this particular source ad happens to answer. Health For Moms cannot attack a named competitor; its rules state the villain is always the system or the mechanism, never a named company or individual. **Stated**, brand context Section 8. That would kill most Us vs Them executions. It does not kill this one, because Insurify does not name anybody either. The left side simply says "Old insurance." That is a category alternative, not a rival, and it maps precisely onto the system-as-villain frame this brand has already built its whole positioning on.

The gap it fills is proof of the savings claim, which the account currently asserts and never shows. Every POV ad in this account says the number out loud, "saved $400 a month," over a picture of a peaceful bedroom. There is no visual evidence anywhere. This format makes the number the picture. The lever it pulls is loss aversion, which the brand's own reference frameworks already name, listing Kahneman and Tversky among its standing references. **Stated**, brand context Section 7. "Stop overpaying" tells a mom she is losing money right now, which is a different and sharper motivator than "you could save." On awareness stage this speaks to the solution-aware mom who knows better plans exist and has not compared, and that is a stage the current mix, sitting at 55.7 percent solution-aware by spend but almost entirely in wordless lifestyle POV, addresses emotionally and never once with a number she can check.

### 5. Street Interview — medium conviction

**Source ad.** A sunny parking lot. A dirty black pickup truck fills the frame with a man in the driver's seat, and yellow on-screen text reads "HEY DUDE, EXCUSE ME." An off-camera voice asks *"Hey dude, excuse me. How do you afford a truck like this? What's the deal?"* The driver, mid-thirties, burnt orange crew-neck sweater, sunglasses tucked in the collar, leans out the window and answers *"I'm a car insurance broker."* The interviewer pounces: *"So I'm actually happy I found you. How do I get my car insurance rate to go down? I'm with the same carrier for years, dude, but it just keeps on going up."* The broker gives two answers, and the second is the product. At 18 seconds the shot cuts to a phone screen scrolling real quotes side by side. Back to the truck, the interviewer asks *"Is that legit?"* and the broker says *"100%. See, every company calculates rates differently, so they could be hundreds of dollars apart. And staying with the same carrier doesn't mean you'll be saving. That's where they get you,"* pointing a finger at the lens. It ends with him repeating the name.

- Source library: wider Parker ad-library corpus
- Source brand: Insurify
- Reference: https://app.heyparker.ai/dashboard/ad-library?adId=932020529912203&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
- Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/f4a62dbe-bc7a-4f7e-95ae-d1a670038652/932020529912203.mp4
- Delivery signal: Meta Ad Library impression rank 8, improved from rank 9. Launched July 2, 2026, running 63 days. All six of Insurify's Authority Figure videos are also Street Interviews

**Conviction: medium.** Per `ad-formats/video/index.md`, `Street Interview` means someone with a microphone interviews people in a public setting and that interaction appears in the hook. Health For Moms ran three last quarter for $296.58 and none this quarter, so it is a dropped format that was never properly funded in the first place. Conviction is medium rather than high for an honest reason: this is the most production-heavy recommendation on the list, and production is a bottleneck the brand has already named. It requires a location, two people, and a shoot day.

What earns it a place anyway is that it solves the account's exact structural problem in a way nothing else here does. Every ad in this account is one woman alone, talking to her phone. The interview format puts two people on screen and lets the viewer eavesdrop, and it does something clever that this brand needs badly: it separates the person asking the sceptical question from the person answering it. Notice where the trust comes from in the Insurify ad. The expert recommends a tool that replaces his own job. That is the "why would he say that unless it were true" move, and it is the strongest available answer to the *"is Health for Moms legit"* search behaviour the brand context flags.

The gap it fills is objection handling in public. The brand's context names the most culturally loaded objection in insurance marketing plainly: *"I don't want to get on a call and be sold to."* **Stated**, brand context Section 5. Right now no ad in the account addresses that. A street interview lets the objection be spoken out loud by a stranger, in a school pickup line or a grocery store parking lot, and answered by someone who is not selling. On awareness stage it reaches the problem-aware and unaware mom who was not looking for insurance at all, which is the coldest and largest pool and one this account has essentially stopped fishing in. Per `killer-performance-ads.md`, a story lead is how you take a stranger and walk her down the awareness ladder, and an overheard conversation is a story lead with a real setting attached.

## Open loops

**1. The formats that hold attention get almost none of the money.**
The four formats with the best hold rates in the account are Graphic Video at 13.59 percent, Educational at 12.61, Other at 11.49 and Skit at 11.08. Together they touched 3.7 percent of the window's spend. The three biggest formats together touch $88,162.07 of spend once their tag overlaps are netted out, which is 88.8 percent of the account. POV at 70.6 percent holds 3.21, Social Interface at 15.8 percent holds 6.35, and Callout at 12.8 percent holds 2.88.
*Pull: Tension.* Meta's delivery says one set of ads is the most potent thing in the account, and the attention data says the opposite set is, and both cannot be the right description of what is working.
**Question: What is Meta seeing in the low-hold formats that the hold-rate numbers do not show?**
If the answer is that hold rate simply does not predict lead cost for a form-fill product, then the account's whole attention problem is a distraction and the November plan should chase hook rate and cost per click instead. If the answer is that the formats holding attention were never given enough budget to compete, the ranking is an artifact of spend and the fix is a funded test.
*Territory: Messaging.*

**2. This account has never run a static ad.**
Zero image ads across the full 90 days, and zero in the prior 90 as well. Meanwhile every one of the five insurance and finance lead-gen brands checked in the wider ad library runs a large static library, from 191 statics at Insurify to 856 at Ethos. The brand said image ads were acceptable for finding angles and none were made.
*Pull: Gap.* There is an entire modality the whole category treats as core inventory and this account has never once tried it.
**Question: What has kept statics out of this account?**
If it is a production or staffing choice, statics are the cheapest way to raise the brand's 1 to 5 concepts a month before Open Enrollment. If it is something learned, a platform rule, a lead-quality problem from form-fill statics, or an earlier test that failed, that reason needs to be written down because four of this audit's five recommendations assume statics are available. **This one only the brand can answer.**
*Territory: Product.*

**3. Six formats left the account and one arrived.**
Authority Figure, Street Interview, Infomercial / VSL, Humour, Offer Based and B-roll mashup + Voiceover all carried spend last quarter and none carried any this quarter. Stitch Hooks did not technically vanish but fell from $32,885.20 to $8.14, a drop of 99.98 percent.
*Pull: Surprise.* The brand told us its problem was too little creative diversity, and in the three months since, the format count went from 20 down to 15.
**Question: Why did the account stop making these formats?**
Whether these were killed on performance, lost when a creator or agency relationship ended, or simply crowded out while the team leaned on the POV ads that were scaling decides whether they are dead ends or dormant capacity to restart before November 1. **This one only the brand can answer.**
*Territory: Messaging.*

**4. Different formats are reaching different-aged moms.**
POV put 43.6 percent of its spend on women aged 25 to 34 and 9.4 percent on 45 to 54. Skit did close to the reverse, 11.9 percent on 25 to 34 and 34.7 percent on 45 to 54. Social Interface sat in the middle with 45.7 percent on 35 to 44 and 23.6 percent on 45 to 54. Educational skewed oldest of all, with 24.4 percent on 45 to 54 and 7.6 percent on 55 to 64.
*Pull: Surprise.* The format mix was never designed as a targeting tool, and it appears to be acting as one anyway.
**Question: Who is the format choice actually putting these ads in front of?**
The brand says it wants to test moms of all ages with kids of all ages, and if format is the lever that reaches a 48-year-old mom, then the near-total collapse of Skit and Educational quietly removed the account's only way to reach her.
*Territory: Personas.*

**5. The creative that holds attention best sits in a bucket the tagger could not name.**
The `Other` format holds 11.49 percent, spend-weighted, and its lead ad `moms54-3` holds 13.66 percent with an 8.08-second average play time, the strongest attention numbers in the window. `Other` is the label applied when no defined format can confidently be assigned. Last quarter this bucket was the account's largest at 36.9 percent of spend across 29 ads.
*Pull: Curiosity.* The single thing this account does best is the one thing the shared vocabulary of the craft cannot put a name to.
**Question: What is the thing these ads are actually doing?**
Naming it decides whether the team can brief more of it. Right now a creator cannot be asked to make another `moms54-3` except by being shown the video, and a format nobody can name is a format nobody can scale.
*Territory: Messaging.*

**6. Nobody qualified has ever appeared on camera.**
Across 147 ads with delivery, every face is a mom talking about her own bill. Authority Figure ran four times last quarter and zero times this quarter. Meanwhile Ethos runs 24 Authority Figure videos and Lemonade 9, and it is the top video format for both. The brand's own context flags that people search whether Health For Moms is legitimate.
*Pull: Gap.* There is a trust question the brand knows it has, and no ad in the account is built to answer it.
**Question: Who could speak for this brand with real credentials on camera?**
The partner agencies employ licensed advisors, the compliance rules allow a real licensed professional, and the brand names casting as its top bottleneck. Knowing whether a partner advisor can be filmed decides whether the second recommendation on this list is a shoot or a fantasy. **This one only the brand can answer.**
*Territory: Creators and talent.*

**7. Deep attention is costing more per lead, not less.**
The three formats with the strongest hold rates are also among the most expensive: Educational at $32.00 per lead, Graphic Video at $31.82 and Other at $33.62, against an account average of $22.64 and a POV blended cost of $21.31. The claymation ad that holds 13.59 percent brought 12 leads. The silent bedroom montage that holds 3.28 percent brought 1,934.
*Pull: Tension.* Every instinct in the craft says holding a viewer longer should convert her better, and in this account the relationship is running backwards.
**Question: How much of the cost gap between the formats that hold attention and the POV ads is explained by spend level rather than by the creative?**
All three of those formats sit under $2,100 in spend, which is thin enough that a handful of leads swings the number, so knowing whether the gap survives a real budget decides whether those formats are a discovery worth funding before Open Enrollment or a trap.
*Territory: Product.*

## Appendix - Parker media links

Every ad discussed in the body of this audit, indexed so a strategist can reopen the media without searching. Links and paths are preserved exactly as returned by the Parker MCP. Entries M001 through M032 are this brand's own Meta ads. Entries M033 through M038 are external ads from the wider Parker ad library.

**M001: Moms43 - 4 - V3.** The account's top spender at $43,002.86. Lead POV example throughout section two and the executive summary. Silent bedroom montage, 45.35 percent hook, 3.28 percent hold.
Facebook ad id: 120241073380060519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380060519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/af61037230d4df3fadf1baaa731a878014c2e5969a06cfffc8098393996b7531.mp4

**M002: Moms43 - 5 - V1.** $10,125.67. Top Social Interface ad, the tweet-overlay selfie. 7.59 percent hold, 2.14 percent CTR.
Facebook ad id: 120243987355020519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120243987355020519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0fe2980848d12fe1c6fd107a759e68fe37d8776c34235b5fab3c15e751af171d.mp4
Landing page: https://www.healthformoms.co/save/

**M003: Moms43 - 4 - V1.** $6,993.31. Second POV ad in the bedroom cluster, $26.90 cost per lead.
Facebook ad id: 120241073380110519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380110519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/f18c5a15a13e4412e35f654034f63f147ca73e40b35538419d22500d143b670d.mp4

**M004: moms-63 2b.** $5,529.30 at a $13.26 cost per lead, the cheapest lead cost among top spenders and inside the brand's fantastic band. The newer POV execution, mom and son leaving a house. Discussed in POV and Callout.
Facebook ad id: 120247093361410519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093361410519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/00b743c5291879d067db10caecf53a6123dd5f8b7063712091a6e9f0ff4eb399.mp4
Landing page: https://www.healthformoms.co/save/

**M005: Moms43 - 4 - V4.** $5,468.11 at a $30.21 cost per lead. Part of the POV bedroom cluster.
Facebook ad id: 120241073380050519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120241073380050519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/985c6a8045a5bcfb5e7450ad0f3a00ca783b996f4ba3633337e8c84e1aac8a39.mp4

**M006: moms-63 3e.** $5,243.54 at a $15.47 cost per lead. The other newer POV execution, mother and son holding hands outdoors.
Facebook ad id: 120247093478820519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093478820519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/6a45457e776af311dfb45d100c093bab9d3f90c7575195dfd86b6260763f1670.mp4
Landing page: https://www.healthformoms.co/save/

**M007: MOMS34 - N1 - 3a.** $5,141.80. The account's only Mashup ad, the hide-and-seek mom moment montage. Created February 21.
Facebook ad id: 120238654140050519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238654140050519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1c501ac53c00f4e6b9f3ee87626968c02aa9861c6958bcf6c338644cbaf1fa8d.mp4
Landing page: https://www.healthformoms.co/save/

**M008: moms-53 3.** $1,956.50 at a 3.14 percent CTR and $16.44 cost per lead. The "Approved State List ✔️" ad, the purest Callout execution and the closest thing in market to the brand's proven state angle.
Facebook ad id: 120247254787160519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254787160519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e6225ca24b359ea0ab06bbeafe453b45496c1310c5a736ba3ea560045c6bd093.mp4
Landing page: https://www.healthformoms.co/save/

**M009: Moms Nahuel WV#1 - V9 - Copy.** $1,639.35 at a $273.23 cost per lead, the single ad dragging the Social Interface average into the not-good band.
Facebook ad id: 120247145872230519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247145872230519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/645496c411d82a546a3e2deada69459c716615ad09f635ca0b978625c2778b37.mp4
Landing page: https://go.healthformoms.co/save/

**M010: moms54-2.** $1,467.48 at a $34.94 cost per lead. Comment Response and Social Interface, the $6,000 deductible tweet overlay.
Facebook ad id: 120247063459400519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063459400519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/3a3e8a8b9f24c4b0e70dd7e422561de2773ffc4fd2dfdabd358971ca6be65f98.mp4
Landing page: https://www.healthformoms.co/save/

**M011: MOMS39 - 2 - V2 - Copy.** $1,459.30 at an $18.95 cost per lead, the best-converting Social Interface ad.
Facebook ad id: 120247037227340519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247037227340519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b5709e2fc3c51b32fc818394fcc0d33d94206dccad0c923f953671d48875d937.mp4

**M012: Moms43 - 5 - V4.** $1,393.32 at a 7.05 percent hold rate. The strongest Comment Response ad, "STOP paying your insurance deductibles before you watch this."
Facebook ad id: 120243987799880519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120243987799880519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0a474fa6fad5214df678eb97d7e22d1ef7ff50313ce4dac1c8a398c0347260bd.mp4
Landing page: https://www.healthformoms.co/save/

**M013: moms-65 1a.** $1,284.38 at a $21.41 cost per lead. POV, stylish mom and son in front of a modern house.
Facebook ad id: 120247285907980519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247285907980519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/bb071de9e8d0e46ca498a10528b066d07bf324999cb3e1b0d11d83c83592cc67.mp4
Landing page: https://www.healthformoms.co/save/

**M014: moms54-3.** $1,283.69. The ad that holds attention best in this window, 13.66 percent with a 57.02 percent hook rate and 8.08-second average play time. The "two hour call" crying confessional, lead example for the `Other` format and open loop 5.
Facebook ad id: 120247063711860519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063711860519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/5a62b11062812d9509cb2cd8c95e89777a15d1a6ac1cdb1f6e9a92eb77f93a9d.mp4
Landing page: https://www.healthformoms.co/save/

**M015: moms54-4.** $647.52 at a 52.40 percent hook and 8.62 percent hold. The "monkey bars" crying ad, second `Other` example.
Facebook ad id: 120247063735970519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063735970519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e3aa685999bf4fde82152827c7fc95489462441238ae397a7e24c3a2f8bd7ddc.mp4
Landing page: https://www.healthformoms.co/save/

**M016: MOMS34 - N1 - 1a.** $118.50. Third `Other` ad, the toddler-spinning hallway montage.
Facebook ad id: 120238653990440519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238653990440519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1e2f0882145d5ab66be010427ad0226948766772aa4519ab52bd054e2752260a.mp4
Landing page: https://www.healthformoms.co/save/

**M017: Moms46 - V1.** $381.82 at a 13.59 percent hold rate, the highest in the window. The claymation "cheaper if you don't use your insurance" ad. The account's only Graphic Video and its lead Educational example.
Facebook ad id: 120246046671140519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120246046671140519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/0e843f33de6045345de8bafc06819312831ea5db2037b5a0670dc09af3412597.mp4
Landing page: https://www.healthformoms.co/save/

**M018: Moms46 - V2.** $86.06 at an 11.15 percent hold rate. Claymation, "Same scan, same hospital." Educational and AI Animation.
Facebook ad id: 120246046732760519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120246046732760519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/5658ec375b09b246b0bd732b5c1c7b5eccc7aa5a73358ee66252445be52e38ac.mp4
Landing page: https://www.healthformoms.co/save/

**M019: Moms46 - V4.** $36.35 at a 6.00 percent hold rate. Claymation, "Your insurance company and your hospital are often the same company now."
Facebook ad id: 120246046737390519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120246046737390519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/f3363086ff59dcc4b9d88e5d8fcfbef71843d78dfdca3b29de2e87f4df165b06.mp4
Landing page: https://www.healthformoms.co/save/

**M020: Moms36 - 3 - A - 2 - V4c - Copy.** $671.21 at an 11.16 percent hold rate and a 9.69-second average play time, the longest watch time in the window. The lead Skit ad, "I wish this was a joke."
Facebook ad id: 120247022319520519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247022319520519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/fe4ef9c25b9bd439ba7664d9b004e6a952789df99e759dd325e2a638e364cf42.mp4
Landing page: https://www.healthformoms.co/save/

**M021: moms55-1.** $655.43 at a $20.48 cost per lead. The lead UGC Single ad, filmed in a school pickup line.
Facebook ad id: 120247304910390519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247304910390519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b3ef51c46ea047450eeba20ec707c5b9022d136aa15f90b609da424269526a11.mp4
Landing page: https://www.healthformoms.co/save/

**M022: MOMS34 - N1 - 4a.** $23.49 at a 54.08 percent hook rate, the second highest in the window. The account's only Wall of Text ad, "I used to dread checking the mail."
Facebook ad id: 120238654188960519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120238654188960519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/a799e7eb7ae0c975a8daca5a3bb9635e922d7f337e80d878e3c2445dd5583359.mp4
Landing page: https://www.healthformoms.co/save/

**M023: Moms43 - 1 - V12.** $5.38. The account's only Podcast-tagged ad, a woman at a studio microphone with a tweet overlay.
Facebook ad id: 120243988073760519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120243988073760519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/855439cc6a5bffb2caf60d1b8ed77066afd5d1a3addc0bc7e5d164c336d968bc.mp4
Landing page: https://www.healthformoms.co/save/

**M024: Moms43 - 1 - V14.** $310.84. The studio-microphone Social Interface ad, "Moms, not all health plans are the same. I learned the hard way." Referenced in the Podcast section as a podcast setting without a podcast.
Facebook ad id: 120243988073730519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120243988073730519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/674aaf8fac5f106f72bd05642832fd763b8739ae1497923a2a9cef47fbf99b17.mp4
Landing page: https://www.healthformoms.co/save/

**M025: moms-65 1c.** $46.13 at a $15.38 cost per lead. UGC Single, the "$4,600 MRI" cash-price comparison.
Facebook ad id: 120247286033490519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247286033490519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/e8dacd6894b005061a1465804ff64b8de78c0951ba1491738780d9afe0bbd5ba.mp4
Landing page: https://www.healthformoms.co/save/

**M026: moms54-6.** $5.63. The stronger of the two Green Screen ads, a woman with a medical bankruptcy research paper behind her.
Facebook ad id: 120247063797850519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247063797850519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/aba2b7fe153bb6e9f628e79d88597aab0dd5ec44a1f1fbe4a62bb9250ecf5e67.mp4
Landing page: https://www.healthformoms.co/save/

**M027: moms-63 1c.** $2.32. The second Green Screen ad, a boy dancing in front of a staircase under an explanation-of-benefits POV overlay.
Facebook ad id: 120247093224540519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247093224540519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/b421643f9fee6cc6ececf52d71a30caa52d2bd96be97e151d538e1fe8018caeb.mp4
Landing page: https://www.healthformoms.co/save/

**M028: Animation Agency #4 - H1 - Copy.** $1.12. The personified medical bill, "I am your deductible." The most creatively ambitious idea in the account and effectively never put in market.
Facebook ad id: 120247022230950519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247022230950519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/1fcb56617f1abef55835db4394f845606247c6dc9ddd955792cd7c71d21bd222.mp4
Landing page: https://www.healthformoms.co/save/

**M029: moms-65 2d.** $2.78 at a 9.52 percent hold rate. A surviving Stitch Hooks ad, the crying "monkey bars" cut.
Facebook ad id: 120247286246950519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247286246950519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/8b90dbb955eae4c6858c1dd4684dccc998607ba073f2b37b8de27a27ab71abee.mp4
Landing page: https://www.healthformoms.co/save/

**M030: MOMS38 - 1 - V1.** Prior-window reference only. $54,173.20 at a 17.29 percent hold rate and 7.08-second play time. The talking-head "Health Insurance is a scam" opener that anchored the prior quarter, cited as what the account moved away from.
Facebook ad id: 120239479305920519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120239479305920519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/50a0309be06d87e55299b9e00d7962b88516c847dec96e80cfd47e6ba5959b66.mp4
Landing page: https://www.healthformoms.co/save/

**M031: moms-65 2f.** $6.55. UGC Single, "We are absolutely being scammed and robbed of our money when it comes to health care."
Facebook ad id: 120247286253100519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247286253100519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/33f81a6606150b6966633444b274452e74a5198502766e18e8774e2b719ad0cd.mp4
Landing page: https://www.healthformoms.co/save/

**M032: moms-53 6.** $1.95. A surviving Stitch Hooks ad, "Health Insurance is a scam 🤨."
Facebook ad id: 120247254795280519
Parker dashboard: https://app.heyparker.ai/dashboard/facebook-ads/performance?adId=120247254795280519&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/aed0ff06-555d-4f4f-9bf8-31178e2fb977/d6f1fb6bf29ed48677cf6d23be9dc080e90a10c60788de8eb46fe1a68d788bf7.mp4
Landing page: https://www.healthformoms.co/save/

**M033: Insurify — age-selector static.** External. Recommendation 1, `Interactive`. Meta Ad Library impression rank 1, stable. Launched July 2, 2026.
Meta Ad Library archive id: 1765001758269651
Parker ad library: https://app.heyparker.ai/dashboard/ad-library?adId=1765001758269651&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/f4a62dbe-bc7a-4f7e-95ae-d1a670038652/1765001758269651.jpg
Landing page: https://insurify.com/rlp/754

**M034: Ethos — "no med exam" headline static.** External. Recommendation 3, `Headline Only`. Meta Ad Library impression rank 1, up from rank 3. Launched August 4, 2026.
Meta Ad Library archive id: 1388982813144880
Parker ad library: https://app.heyparker.ai/dashboard/ad-library?adId=1388982813144880&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/fcc3a6f6-46ae-40f4-8071-6341dbd5e1fb/1388982813144880.jpg
Landing page: https://www.ethos.com/life/get-life-insurance/
Ad Library: https://www.facebook.com/ads/library/?active_status=active&ad_type=all&country=ALL&is_targeted_country=false&media_type=all&search_type=page&source=fb-logo&view_all_page_id=284894298576955

**M035: Insurify — "Stop overpaying" split-house static.** External. Recommendation 4, `Us vs Them`. Meta Ad Library impression rank 7, climbed six places in 12 days. Launched August 4, 2026.
Meta Ad Library archive id: 1546880869622488
Parker ad library: https://app.heyparker.ai/dashboard/ad-library?adId=1546880869622488&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/f4a62dbe-bc7a-4f7e-95ae-d1a670038652/1546880869622488.jpg
Landing page: https://insurify.com/rlp/583

**M036: Lemonade — veterinarian Authority Figure video.** External. Recommendation 2, `Authority Figure`. Meta Ad Library impression rank 14. Launched April 23, 2026, running 133 days.
Meta Ad Library archive id: 2168773877290882
Parker ad library: https://app.heyparker.ai/dashboard/ad-library?adId=2168773877290882&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/27c8be1e-bce2-4ecf-a730-91b3e40b6f9c/2732968667067890.mp4
Landing page: https://www.lemonade.com/pet
Ad Library: https://www.facebook.com/ads/library/?active_status=active&ad_type=all&country=US&is_targeted_country=false&media_type=all&search_type=page&source=fb-logo&view_all_page_id=1640971869496619

**M037: Insurify — "How do you afford a truck like this" street interview.** External. Recommendation 5, `Street Interview`. Meta Ad Library impression rank 8, up from 9. Launched July 2, 2026, running 63 days.
Meta Ad Library archive id: 932020529912203
Parker ad library: https://app.heyparker.ai/dashboard/ad-library?adId=932020529912203&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Video: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/f4a62dbe-bc7a-4f7e-95ae-d1a670038652/932020529912203.mp4
Thumbnail: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/f4a62dbe-bc7a-4f7e-95ae-d1a670038652/932020529912203-thumbnail.jpg
Landing page: https://insurify.com/rlp/754

**M038: NerdWallet — "5.99% APR" selector static.** External. Cited in section three as the second example of the tappable-selector pattern. Meta Ad Library impression rank 1, stable. Launched May 28, 2026, running 98 days.
Meta Ad Library archive id: 1688749802321309
Parker ad library: https://app.heyparker.ai/dashboard/ad-library?adId=1688749802321309&brandId=aed0ff06-555d-4f4f-9bf8-31178e2fb977
Image: https://auth.heyparker.ai/storage/v1/object/public/internal-facebook-ads/external-brands/f4d7e791-0ef8-483e-ac5c-f2adbdfde50a/1688749802321309.jpg
Landing page: https://www.nerdwallet.com/prequalify/m/personal-loan/facebook/lp1

*This is based on everything I have learned about making iterations 2.0*

*this is based on everything I have learned about visuals in advertising*

*This is everything I know about tailoring creative strategy to brand size.*
