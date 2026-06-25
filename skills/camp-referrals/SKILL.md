---
name: camp-referrals
description: When the user wants a summer camp to turn its happy families into new families and genuine reviews, through referrals, a bring-a-friend or sibling offer, parent ambassadors, or review requests. Use for camp referrals, word of mouth, refer-a-friend, getting more Google reviews, a referral or ambassador program, sibling discounts, or asking families to spread the word. It draws on camp-voice for the asks and camp-emails for the messages. Reviews here also feed camp-seo and camp-aeo.
summary: Turn happy families into referrals and reviews.
category: marketing
icon: heart
examples:
  - "Set up a bring-a-friend offer tied to early-bird enrollment."
  - "Write the end-of-session ask that earns us a Google review."
  - "Get this summer's families to come back with a sibling next year."
order: 6
status: published
version: 1.0.0
---

# camp-referrals

Turn a camp's happy families into new families and genuine reviews. Camps grow on word of mouth and loyalty more than most businesses do: siblings follow siblings, and parents send their kids to the camp they went to. So this is one of the biggest and cheapest levers a camp has. This skill carries referral and review practice with a camp layer on top.

It is written for you, the agent. Use camp-voice for the asks, camp-profile for the camp's facts and voice, camp-overview for how families find and stay with camps, and camp-emails to actually send the messages. One hard rule runs through the review side: follow the FTC's reviews rule (see the guardrail at the end). It is in force and being enforced, and the penalties are real.

## Ask first

Start from what is known, then ask only for the gaps.

**1. Read the camp's context first.**
- If a camp profile exists (`.agents/camp-profile.md` or `.claude/camp-profile.md`), read it for the camp's facts and voice. Do not re-ask what it answers.
- Use camp-voice for the asks and its avoid-list, and camp-overview for the referral, advisor, and loyalty model.
- If no profile exists, offer to capture one with the camp-profile skill, then continue.

**2. Ask only the task-specific gaps:**
- Whether they want referrals, reviews, or both.
- How families hear about them now, how many return each year, and whether families already refer.
- What they can offer as a referral reward and sustain (a discount, camp-store credit, priority registration).
- Where reviews would help (Google first, then the directories families use), and any parent ambassadors or camp advisors they work with.

**3. How far to go (the depth dial).** Match it to the director's goal and how much they want to take on. Default to one well-timed ask, and offer to go deeper.

- **Quick wins (low effort):** a well-timed review request to recent happy families, and a simple bring-a-friend or sibling offer.
- **Solid setup (medium effort):** a referral program (the loop below), a steady review habit across the season, and a push on re-enrollment.
- **Full build (high effort):** a parent-ambassador program, tracking for the camp-advisor channel, and measurement across both referrals and reviews.

## Grow word of mouth

### 1. Keep referrals and reviews separate (all tiers)

These are two different things, and mixing their incentives is where camps get into trouble:

- **Referrals:** a family brings a new family who enrolls. You can reward this freely (a discount, store credit).
- **Reviews:** a family posts a public rating. You can ask for these and even thank people for writing one, but you cannot pay for a positive one. Keep the rules below in mind.

### 2. Ask at the moment of peak goodwill (all tiers)

The ask works when the family is happiest, so time it: the end of a session, visiting day, the proud pickup, a great week, or at re-enrollment. A warm, personal ask works better than a mass message sent whenever.

### 3. Reviews, done right (Quick wins)

Genuine, recent, well-rated reviews are among the strongest things a camp can have, and they feed both search and AI recommendations (see camp-seo and camp-aeo).

- Ask recent happy families for an honest review on Google first, then the directories families actually use, with a direct link so it takes a moment.
- Reply to every review, including the critical ones. A calm public reply reassures the next parent reading.
- Keep a steady flow into each season rather than one burst, since recency matters.
- Stay inside the FTC rule below: ask broadly, but never tie a reward to a positive review.

### 4. The referral loop for a camp (Solid setup)

A simple loop, timed to goodwill:

- **Trigger:** the happy moment (end of session, re-enrollment).
- **Share:** make it easy with a personal link or code, or a plain bring-a-friend offer the family can pass on.
- **Enroll:** the referred family signs up, tracked to the family who referred them.
- **Reward both sides:** a sibling or referral discount, camp-store credit, or a session credit. A small reward for the new family too lifts conversion.

Keep the ask personal. A note from a director or a familiar counselor outpulls a generic blast.

### 5. Lean on loyalty and siblings (Solid setup)

Returning families refer the most, so the loyalty base is where referrals grow. Make re-enrollment easy and worth it, offer a sibling discount, and remember that many alumni are now parents who will send their own kids. These are warm asks, not cold ones.

### 6. Parent ambassadors and the advisor channel (Full build)

- **Ambassadors:** a handful of enthusiastic parents who happily refer. Give them an easy link and a genuine thank-you, and do not over-formalize it.
- **Camp advisors and referral services:** independent services that match families to camps and take a commission when a family they referred enrolls. If you use them, track which enrollment came from which advisor, so you pay the right fee and can see whether the channel is worth it.

### 7. Measure it (Full build)

Watch the share of new families that came from referrals, the referral conversion rate, and the count, recency, and rating of reviews. Compare the cost of a referred enrollment to your other channels. Referred and returning families tend to stay longer, which is the real value.

### 8. The FTC reviews rule (all tiers, non-negotiable)

The Consumer Reviews and Testimonials Rule is in force and the FTC is enforcing it, with penalties in the tens of thousands of dollars per violation. Stay well clear:

- Never write, buy, or use fake reviews, including AI-written ones that pose as real families.
- You may offer an incentive for writing a review, but never condition it on the review being positive or a certain star rating.
- Disclose clearly when a review is written by staff, the owner, or their family.
- Do not present testimonials on your own site as if they were independent reviews.
- Do not hide, gate, or suppress negative reviews. Respond to them instead.

Honest reviews are the only ones worth having, and the only ones a parent will trust.

## Deliver the asks

- Write the review request, the referral offer, and any ambassador note in camp-voice, with the FTC-safe wording above.
- For a program, give the loop, the reward, and the timing, scaled to the tier.
- Hand the messages to camp-emails to send, and remember the reviews feed camp-seo and camp-aeo.
- Run every ask through camp-voice's avoid-list and self-audit before handing it over.

## What this skill will not do

- Write, buy, or use fake reviews, or condition any reward on a positive review.
- Hide or suppress negative reviews.
- Promise a number of referrals or reviews.
- Send the messages or handle family data (see camp-emails), or restate the voice rules (see camp-voice).

## Grounded in

Word-of-mouth and referral practice, plus the FTC's rules on reviews and endorsements, which are current and enforced. Referrals and reviews must be real and voluntary, and any incentive must never be tied to a positive review.

- FTC Consumer Reviews and Testimonials Rule, questions and answers: https://www.ftc.gov/business-guidance/resources/consumer-reviews-testimonials-rule-questions-answers
- US FTC advertising and marketing guidance: https://www.ftc.gov/business-guidance/advertising-marketing
