---
name: camp-ads
description: When the user wants to run paid ads to fill a camp's sessions, on Meta (Facebook and Instagram) or Google Ads, aimed at parents. Use for camp ads, paid social, Facebook or Instagram ads, Google Ads or PPC for a camp, retargeting parents who did not enroll, ad copy or creative for a camp, or deciding what to spend and when. It draws on camp-voice for the ad copy and camp-website-copy for the pages ads point to. For organic search see camp-seo, and for unpaid social posts see camp-social.
summary: Paid social and search ads that fill your sessions.
category: marketing
icon: cursor
examples:
  - "Write a Meta ad to fill our last eight spots in July."
  - "Plan a starter Google Ads setup targeting parents in our county."
  - "Set up retargeting for parents who started enrolling but didn't finish."
order: 4
status: published
version: 1.0.0
---

# camp-ads

Run paid ads that fill a camp's sessions, on Meta and Google, aimed at the parents who decide. This carries standard paid-media practice with a camp layer on top.

It is written for you, the agent. Use camp-voice for the ad copy, camp-profile for the camp's facts and voice, and camp-website-copy for the pages the ads point to. Ads spend real money and reach families with children, so two things hold throughout: the claims must be true (see the guardrails below), and a small camp should not overspend. Never promise enrollments or a return on spend.

## Ask first

Start from what is known, then ask only for the gaps.

**1. Read the camp's context first.**
- If a camp profile exists (`.agents/camp-profile.md` or `.claude/camp-profile.md`), read it for the camp's facts and voice. Do not re-ask what it answers.
- Use camp-voice for the ad copy and its avoid-list, and camp-overview for the camp year.
- If no profile exists, offer to capture one with the camp-profile skill, then continue.

**2. Ask only the task-specific gaps:**
- The budget, and which sessions or programs need filling.
- The one conversion that counts (an enrolled camper, a started application, a booked tour, a real inquiry), and roughly what a camper is worth.
- The landing page the ads will point to, and whether it is ready (see camp-website-copy).
- Whether they have last year's family list or a website pixel, which the strongest targeting relies on.
- What they have run before, and what happened.

**3. How far to go (the depth dial).** Match it to the director's goal and how much they want to take on. Default to one focused campaign, and offer to go deeper.

- **Quick wins (low effort):** one tightly-targeted campaign at the highest-intent moment, usually Google Search for parents looking now, or Meta retargeting of recent site visitors. Small budget, pointed at the right page.
- **Solid setup (medium effort):** the seasonal plan across Meta and Google, with lookalike audiences from last year's families and retargeting.
- **Full build (high effort):** the full account, creative testing, conversion tracking wired to enrollment, and ongoing optimization.

## Run the ads

### 1. Decide the conversion and what it is worth (all tiers)

Pick the one action that counts, usually an enrolled camper, sometimes a qualified inquiry or a booked tour. Work out roughly what a camper is worth to the camp (tuition, times the years a family tends to return), so the spend stays sane. If a camper is worth a few hundred dollars in margin, the cost to win one through ads has to sit well under that.

### 2. Pick the platform for the job (all tiers)

- **Google Search** reaches parents looking right now. Bid on the terms they type ("summer camp near [town]," "[sport] camp for [age]," your camp's name). High intent, and it pairs with the organic work in camp-seo.
- **Meta (Facebook and Instagram)** reaches and re-reaches parents. Use it for the research window, for lookalike audiences built from your own families, and for retargeting people who visited the site but did not enroll.

Most camps start with Google Search for intent and Meta retargeting for efficiency, then add Meta prospecting once those work.

### 3. Target the right parents (Solid setup)

- **Lookalikes from your own families** are the strongest signal. Seed them from last year's deposits or your email list, not broad interest targeting.
- **Retargeting** people who visited the site and did not register is usually the most efficient spend you have.
- **Geography:** the towns and radius the camp actually draws from.
- **Exclude** families who have already enrolled, so you stop paying to reach them.
- Target parents and other adults, never children. Follow each platform's current rules for ads related to minors.

### 4. Spend in the windows that matter (all tiers, scaled)

Camp demand is seasonal, so put the budget where the parents are. Two windows do most of the work:

- **September to November:** parents start researching next summer.
- **January to February:** the main decision and deposit season.

Pull back in the dead months rather than spending evenly all year. This matches the camp year and the calendar in camp-seo.

### 5. Creative that works for a camp (Solid setup)

- **Short video wins.** A 15 to 30 second clip of real kids doing real activities at the camp converts better than anything polished. Captions on (most parents watch without sound), shot to feel native, with the hook in the first three seconds.
- **Images:** real faces and real moments from this camp, not stock, with short readable text.
- **Lead with what the parent wants**, shown concretely (a child learning to sail, a calm first night), not a promise of "the best summer ever."
- Write the copy in camp-voice, and build three to five distinct angles so you are testing real differences, not reworded versions of one idea. Good camp angles: reassurance for a first-time camper, a specific program or age, local ("a [town] day camp"), the early-bird deadline, and what makes the camp itself (non-competitive, the arts, the lake).

### 6. Write the ad copy to spec (Solid to Full build)

Each platform truncates copy that runs long, so write to its limits and lead with the hook. Google Search ads and Meta ads have different shapes and character counts. The limits, the camp ad angles, and copy templates with examples are in `references/ad-copy.md`. Write every line in camp-voice, and make only claims the camp can stand behind.

### 7. Track to enrolled campers, not clicks (Full build)

Clicks and form-fills are not enrollments. Wire conversion tracking through to the action that counts, and ideally back to the camp-management software, so the camp knows its cost per enrolled camper, not its cost per click. Then watch budget pacing, cost per inquiry or enrollment, and creative fatigue, and move spend to what is working.

### 8. The guardrails (all tiers)

These are not optional, because this work involves children and parents' trust:

- No fake urgency. "Only two spots left" only if it is true.
- Get consent before using any child's photo, name, or words in an ad.
- Advertise to parents and adults, not to minors, and follow the platform's rules for ads involving children.
- Every claim about safety, results, or reviews has to be true and able to be backed up.

## Deliver the plan

Scale it to the tier the director chose, and make it concrete:

- The campaigns to run, on which platform, with the targeting and the budget split.
- The ad copy, in camp-voice, with character counts and two or three angle options per ad, run through the avoid-list and self-audit.
- The tracking to set up so spend ties to real enrollments.

Hand the landing pages to camp-website-copy, and remember the organic side (camp-seo, camp-aeo, camp-social) carries the off-season when the ads are paused.

## What this skill will not do

- Spend more than the camp can afford, or promise a number of enrollments or a return on spend.
- Use fake urgency or scarcity.
- Use a child's photo, name, or words without consent, or target children.
- Invent claims, reviews, or results.
- Write the landing page (see camp-website-copy) or run the unpaid channels (see camp-seo, camp-aeo, camp-social).

## Grounded in

Standard paid-media practice, the ad platforms' own policies, and honest-advertising rules. Platform rules and ad products change often, so check the current policy before relying on it.

- US FTC advertising and marketing guidance: https://www.ftc.gov/business-guidance/advertising-marketing
- Google Ads policies: https://support.google.com/adspolicy
- Meta advertising standards: https://transparency.meta.com/policies/ad-standards/
