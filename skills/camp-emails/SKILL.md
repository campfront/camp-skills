---
name: camp-emails
description: When the user wants to write or plan the everyday emails a summer camp sends families — enrollment and nurture emails, re-enrollment and retention, the season newsletter and in-season parent updates, lifecycle reminders (deposits, balances, forms, packing), and the email calendar across the camp year. Use for camp emails, an email sequence or drip, a newsletter, an enrollment or early-bird email, a re-enrollment or sibling offer, or a balance or forms reminder, and for email deliverability and CAN-SPAM or CASL basics. It draws on camp-voice for the writing and camp-overview for the enrollment journey. It does not write messages about an injury, a serious incident, a behaviour concern, abuse, or anything with safety or legal exposure — those are drafted by the camp's own experienced staff, not an AI assistant (see "What this skill will not do").
summary: Enrollment, re-enrollment, newsletters, and reminders, in your voice.
category: marketing
icon: envelope
examples:
  - "Write an early-bird enrollment email to last summer's families."
  - "Plan our email calendar across the camp year."
  - "Draft the week-three newsletter for parents while their kids are away."
order: 7
status: published
version: 1.0.0
---

# camp-emails

Write and plan the everyday emails a camp sends families — enrollment nurture, re-enrollment, the season newsletter, in-season updates, and the lifecycle reminders tied to the camp year. This carries email best practice with a camp layer on top.

It is written for you, the agent. Use camp-voice for the writing, camp-profile for the camp's facts and voice, and camp-overview for the enrollment journey and the camp year. Families' and children's data is sensitive, so handle it carefully (see the compliance step).

**What this skill is not for.** It does not write the hard messages — anything about an injury, a serious incident, a behaviour concern, suspected abuse, or any situation with safety, safeguarding, or legal exposure. Those are not marketing emails. They are drafted by the camp's own experienced staff, following the camp's incident protocols, its accreditation body's guidance, legal or PR review, and the reporting duties and privacy laws of its jurisdiction — and a serious incident is a phone call first, never an email. If you are asked for one of these, do not draft it. Say plainly that it needs the right people at the camp, and point to them: the director, the camp's crisis-communication plan, its accreditor (such as the ACA), and legal counsel.

## Ask first

Start from what is known, then ask only for the gaps.

**1. Read the camp's context first.**
- If a camp profile exists (`.agents/camp-profile.md` or `.claude/camp-profile.md`), read it for the camp's facts and voice. Do not re-ask what it answers.
- Use camp-voice for the writing and its avoid-list, and camp-overview for the enrollment journey and camp year.
- If no profile exists, offer to capture one with the camp-profile skill, then continue.

**2. Ask only the task-specific gaps:**
- Who the email is for, and where they are in the camp year (a prospect, an enrolled family, a returning or lapsed one), the goal, and the one action you want.
- Any facts that must be exact: dates, amounts, deadlines, names.
- The camp's jurisdiction, since email consent and privacy duties differ between the US and Canada.

**3. How far to go (the depth dial).** Match it to the director's goal and how much they want to take on. Default to one email done well, and offer to go deeper.

- **Quick wins (low effort):** one email written well (an enrollment nudge, a newsletter, a re-enrollment ask).
- **Solid setup (medium effort):** the core sequences and templates the camp reuses (a welcome and nurture sequence, a newsletter format, the lifecycle reminders, the re-enrollment flow).
- **Full build (high effort):** the full email calendar across the camp year, with the sequences and segments mapped out.

## The camp email year

Email is a year-round channel for a camp, and the cadence follows the season rather than a fixed weekly slot. Map any plan to where the camp is in its year (see camp-overview for the full calendar). A steady **two to four emails a month** keeps a camp present without wearing families out; lean heavier only through the registration push.

- **Off-season (after camp ends through mid-winter):** keep the bond warm. Share last summer's moments, publish next year's dates early, gather reviews while the experience is fresh, and grow the list. This is relationship time, not selling time.
- **Decision window (mid-winter):** family interest in summer plans peaks around January, so the registration push and any early-bird should be live by then, not after. This is when an enrolled-and-engaged list converts.
- **Peak booking (early spring):** spring is one of the busiest stretches for camp registration. Shift to gentle urgency — filling sessions, closing windows, waitlists where real.
- **Pre-arrival (late spring into the start of the season):** the logistics run — confirmation, the welcome packet, a reminder a week or two out, and a day-before note. This sequence answers questions before families ask them.
- **In-season:** the parent-reassurance loop and a light weekly update (see In-season parent updates).
- **Re-enrollment (as each session ends):** the highest-value send of the year. Invite families back while the summer is still fresh (see Re-enrollment and retention).

## Write the emails

### 1. One email, one job (all tiers)

Each email has a single purpose and one main action. If an email asks for five things — register, pay, send forms, sign the photo release, buy merch — parents do none of them. Decide the one thing this email is for, and write toward it. Put the deadline or the ask near the top, not in the third paragraph.

### 2. The subject line and first line do the work (all tiers)

Most parents read on a phone — roughly two in three camp registrations happen on mobile — and skim in seconds, deciding from the subject line and preview. So:

- Keep the subject clear rather than clever, around 40 to 50 characters, and make the one action obvious. Personalize where it is genuine ("[Name], [child]'s forms are due Friday").
- Write the preview text as a second line that extends the subject, not a repeat of it.
- Design for one-thumb scanning: a single column, short paragraphs, one tappable button. Push the detail to the website (see camp-website-copy) rather than cramming it into the email.

### 3. Segment so it stays relevant (Solid setup)

The same email to everyone wastes the channel — a returning family and a first-time prospect need different messages. Segment at least by where a family sits in the camp year:

- **Prospects** (enquired, not registered) need reassurance and proof: what the camp is like, how registration works, what other families say.
- **Enrolled families** need prep and logistics, then the in-season loop, then the re-enrollment ask.
- **Returning and lapsed families** need what is new, whether their counselor is back, and the loyalty or priority window.
- Tag further where it changes the message: session type, camper age, returning versus new, and **financial-aid or campership families**, so payment-plan and campership options reach the families who need them rather than going out as a blast.

### 4. Enrollment and nurture (Solid setup)

For prospective and enquired families, a short sequence beats one blast: a warm welcome and the key facts, then reassurance on what parents actually weigh (a first time away, safety, cost), then the early-bird or deadline, and a gentle nudge to anyone who started registering and did not finish. A few specifics that matter for camps:

- **The welcome is the most-opened email you will send** — use that attention to set expectations and drive the first action, not to say everything at once.
- **Send an instant confirmation** after any registration or payment. A missing "you're in" leaves parents wondering whether it went through, and is a common source of anxious follow-ups.
- **Recover abandoned registrations.** Camp sign-up is long — health forms, payments — so families drop off mid-way. A short, friendly "your spot is still saved, here's the one step left" brings many back. Naming a payment plan, where the camp offers one, removes the most common reason families stall.
- **Early-bird works because it is time-limited.** Give the rate, the deadline, and one link; let the window create the urgency.

Space the emails a few days apart, and point links at the page that does the selling (see camp-website-copy).

### 5. Re-enrollment and retention (Solid setup)

Bringing a family back is far cheaper than winning a new one — by most estimates several times over — which makes re-enrollment the highest-leverage email a camp sends. Treat it as a priority, not an afterthought:

- **Send it as each session ends,** while the summer is still vivid — within a couple of weeks, not in the autumn.
- **Offer returning families something real:** priority access before public registration, a returning-family window, a sibling discount, or multi-session pricing.
- **The referral ask belongs here too.** A happy family at the end of a great summer is the moment to ask them to refer a friend or leave a review (hand the mechanics to camp-referrals).

### 6. The season newsletter (Solid setup)

A warm, scannable update to current families. Lead with a real moment, keep the upcoming dates and any deadline front and centre for busy parents, and add two or three short highlights. Include one clear action only if there is something to act on. Get consent before any camper photo or name (see camp-social and the compliance step).

### 7. In-season parent updates (Solid setup)

When children are away, the question underneath every parent's inbox is "is my kid okay?" Photos and short updates answer it and ease the worry. The hard-won camp lesson: a parent does not care about a hundred beautiful photos if they cannot find *their own child* in any of them.

- **Guarantee early coverage of every camper** — for example, a required first-night shot of each cabin group — so every parent sees their child in the first update.
- **Label and sort more than you shoot,** so a parent can find their child without hunting.
- **Curate, do not dump:** cut the blurry, duplicate, and unflattering shots. Volume of mediocre photos hurts more than it helps.
- Keep the written update short and warm; the photos and the website carry the rest.

### 8. Lifecycle and operational reminders (Solid setup)

The emails tied to the enrollment journey, where getting the facts exactly right matters most: the instant confirmation, a welcome packet a few weeks out, deposit and balance reminders, forms-due nudges, the pre-camp instructions and packing list, a day-before logistics note, and the re-enrollment ask. Keep these warm and plain, and double-check every date and amount. Handle a balance kindly — a friendly reminder with payment or campership options if they exist, never pressure.

### 9. Get it delivered (all tiers)

A great email that lands in spam does nothing. The basics a camp should get right:

- **Send from a person, not a black hole.** Use a real, monitored address like `director@yourcamp.org` — never `no-reply@` or a generic `info@`. Filters distrust no-reply senders, and it blocks the reply an anxious parent wants to send.
- **Send from the camp's own authenticated domain.** Set up SPF, DKIM, and DMARC for it. Since 2024, Gmail and Yahoo effectively require authentication to reach the inbox, and a free Gmail or Yahoo "from" address will be filtered.
- **Keep the list clean.** Remove hard bounces, suppress people who never open, and only email families who opted in. A clean list protects the inbox placement of every other email.
- **Test your own send times.** There is no universal best hour; watch the camp's own open and click rates by day and adjust. Avoid sending right around long weekends, when inboxes are crowded.

### 10. Protect family data and stay compliant (all tiers)

Camp emails carry health details, payment information, and data about children, and the rules differ by country. Keep it practical:

- **Market to the parent, not the child.** Consent that matters is the parent's, captured at registration (this is how the US children's privacy rule, COPPA, and Canada's PIPEDA work in practice). Do not collect data from a child directly, and only use a camper's name or photo in line with a **signed photo or media release**.
- **United States — CAN-SPAM:** an opt-out regime. Every marketing email needs an honest subject and "from," a valid physical mailing address, and a clear unsubscribe that you honour promptly. A pure logistics email (a confirmation, a balance notice) is largely exempt — but the moment it also promotes something, treat it as marketing.
- **Canada — CASL:** stricter, opt-in. You generally need consent before emailing, and "they signed up once" does not last forever — implied consent from a registration expires. Capture express opt-in at registration for Canadian families.
- **Never put one family's private details in another family's email,** and send sensitive records through the parent portal or a secure channel rather than plain email where you can.

### 11. Write it in the camp's voice, then check it (all tiers)

Draft in camp-voice, then run the self-audit against the avoid-list. A camp email should sound like a person at the camp, warm and plain.

## Deliver the emails

- For one email, give the subject, preview text, body, and one call to action, in camp-voice.
- For a sequence, give the overview (trigger, goal, timing, and the segment it is for) and then each email.
- For a calendar, map the sends across the camp year with each one's trigger, segment, and goal.
- **Measure what matters.** Track clicks and replies over opens — Apple's Mail Privacy inflates open rates, so they read higher than reality. The signal to watch for fatigue is the unsubscribe rate.
- Run every email through camp-voice's avoid-list and self-audit, and hand landing pages to camp-website-copy. The review and referral asks come from camp-referrals.

The templates for each email type are in `references/templates.md`.

## What this skill will not do

- Write a message about an injury, a serious incident, a behaviour concern, suspected abuse, or anything with safety, safeguarding, or legal exposure. These are for the camp's experienced staff and its legal, PR, and accreditation channels, not an AI assistant. If asked, decline and point to the right people.
- Share one child's information in a message to another family.
- Give medical or diagnostic advice.
- Promise an anxious parent an early pickup, which tends to reinforce homesickness.
- Restate the voice rules (see camp-voice).

## Grounded in

Email best practice and the rules that govern family and children's email: the ACA's marketing and retention guidance, US CAN-SPAM and children's privacy (COPPA), Canada's anti-spam law (CASL) and PIPEDA, and the Gmail and Yahoo sender requirements for authentication. Follow the camp's own jurisdiction. Anything involving an incident, safeguarding, or a crisis is out of scope here — follow the camp's protocols and accreditation guidance, and route it through the director and legal or PR review.

- American Camp Association: https://www.acacamps.org
- Ontario Camps Association: https://ontariocampsassociation.ca
- US FTC — CAN-SPAM compliance guide: https://www.ftc.gov/business-guidance/resources/can-spam-act-compliance-guide-business
- US FTC — children's online privacy (COPPA): https://www.ftc.gov/business-guidance/privacy-security/childrens-privacy
- CRTC — Canada's anti-spam legislation (CASL): https://crtc.gc.ca/eng/internet/anti.htm
- Office of the Privacy Commissioner of Canada (PIPEDA): https://www.priv.gc.ca
- Google — email sender guidelines (SPF, DKIM, DMARC): https://support.google.com/a/answer/81126
