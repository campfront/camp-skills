---
name: camp-website-copy
description: When the user wants to write or improve the copy on a camp's website, including the homepage, program and session pages, enrollment or landing pages, the about page, or an FAQ. Use for camp website copy, landing page copy, hero or headline help, a page that is not converting, enrollment page wording, or rewriting a program page. It draws on camp-voice for how the copy reads and camp-profile for the camp's facts. For which pages should exist and how they rank see camp-seo, and for paid ad copy see camp-ads.
summary: Landing, enrollment, and program-page copy that converts.
category: marketing
icon: window
examples:
  - "Write the homepage hero and intro for our day camp."
  - "Draft the enrollment page for our two-week overnight session."
  - "Our program page gets visits but no sign-ups, rewrite it."
order: 1
status: published
version: 1.0.0
---

# camp-website-copy

Write the words on a camp's website that turn a visiting parent into an enquiry or a booking. This covers the homepage, program and session pages, enrollment pages, the about page, and FAQs. It carries standard conversion-copywriting practice with a camp layer on top.

It is written for you, the agent. Use camp-voice for how the copy should read, camp-profile for this camp's facts and voice, and camp-seo to know which pages should exist. A page can only sell what is true, so write the real camp well and never invent proof or promise a child a good time.

## Ask first

Start from what is known, then ask only for the gaps.

**1. Read the camp's context first.**
- If a camp profile exists (`.agents/camp-profile.md` or `.claude/camp-profile.md`), read it for the camp's facts and voice. Do not re-ask what it answers.
- Use camp-voice for the writing craft and its avoid-list, and camp-overview for how camps work.
- If no profile exists, offer to capture one with the camp-profile skill, then continue.

**2. Ask only the task-specific gaps:**
- Which page you are writing, and the one action a parent should take on it (enquire, register, book a tour, join the waitlist).
- The offer: ages, dates, price, what is included, deposit and payment terms, any early-bird rate or deadline.
- The proof available: accreditation, staff credentials, ratios, real parent quotes, photos, how many families return.
- The objections this camp hears most (cost, homesickness, safety, fit, food).

**3. How far to go (the depth dial).** Match it to the director's goal and how much they want to take on. Default to one page done well, and offer to go deeper.

- **Quick wins (low effort):** rewrite the homepage hero, the headline, subhead, and primary button. This is the highest-leverage part of the site.
- **Solid setup (medium effort):** a full page built to convert, or the core set: homepage, one program page, and the enrollment page.
- **Full build (high effort):** copy for the whole site, plus the conversion fixes (forms, pricing clarity, friction) below.

## Write to convert

### 1. Start with the one action (all tiers)

Every page needs one main thing you want the parent to do. Decide it first, write the page toward it, and repeat the call to action where a parent is ready to act. If a page asks for five things, parents do none of them.

### 2. The hero, above the fold (Quick wins)

A parent decides in a few seconds whether they are in the right place. The top of the page has to answer, in plain words, what kind of camp this is, who it is for, and where.

- **Headline:** say it straight. "A traditional overnight camp on a lake in the Blue Ridge Mountains, for ages 8 to 14." A plain, specific line works better than a clever one here.
- **Subhead:** one or two lines adding what a parent wants next, like session lengths and dates, or what is particular about the camp.
- **Primary button:** name what they get. "See session dates," rather than "Learn more."

For camp-shaped headline patterns, see `references/page-templates.md`.

### 3. Build the page as a story (Solid setup)

A strong page leads a parent from "is this right for us" to "let's book," instead of listing features. A workable order:

- Hero (above).
- A line of proof near the top: accreditation, years running, or how many families return.
- What the parent is hoping for, shown through what the child actually does at camp.
- How it works: register in a few clear steps, or what a day at camp looks like.
- The trust and proof (below).
- The common objections, answered.
- A final call to action.

Full section-by-section templates per page type are in `references/page-templates.md`.

### 4. Make trust easy to find (Quick wins to Full build)

For a camp, trust is the main thing that converts, because a parent is deciding whether to hand over their child. Put the reassurance where they will see it:

- Accreditation (ACA or the provincial body), stated plainly.
- Supervision ratios, and staff training or certifications.
- Real photos of this camp, not stock images.
- Specific parent quotes, attributed and used with permission, not "Great camp!"
- How many families return each year, if you have the number.
- A refund and cancellation policy a parent can actually find.

This is the same proof that helps search and AI assistants (see camp-seo, camp-aeo), so it does more than one job.

### 5. Answer the objections on the page (Solid setup)

Parents hesitate over the same handful of things. Name them and answer them, in the copy or an FAQ:

- Cost, and any aid (camperships, sibling and early-bird discounts).
- Homesickness, especially for a first overnight camp.
- Safety and supervision.
- Whether their child will fit in.
- Food, allergies, and dietary needs.
- What a day actually looks like.
- Refunds if plans change.

Parents trust a camp more when it answers a hard question instead of dodging it.

### 6. Calls to action that fit a camp (all tiers)

Name the action and what the parent gets from it. Good options depend on the page: "See session dates," "Check availability," "Request the brochure," "Book a tour," "Join the waitlist," "Start your application." Avoid "Submit" and "Learn more." Match the button to where the parent is, since a researching parent is readier to see dates than to enroll on the spot.

### 7. Reduce the friction (Full build)

Good copy still loses a parent if acting is hard:

- Ask only for what you need at this step. A long form loses people.
- Show the price, or a clear range. Hiding it makes a parent leave, and an AI skip you (see camp-aeo).
- Make the next step obvious on every page.
- Write and check it on a phone first, since most parents are on one.

### 8. Write it in the camp's voice, then check it (all tiers)

Draft in camp-voice, then run the self-audit: reread and ask what still sounds like AI or like any camp, and fix it against the avoid-list. The clichés like "memories that last a lifetime" live on camp websites, so this check earns its keep here.

## Deliver the copy

- Lay the copy out by section, ready to paste, with any [placeholders] clearly marked where a real price, date, quote, or photo goes. Never invent those.
- For the headline and the main button, give two or three options with a line on why each works, so the director can choose.
- Hand the page title and meta description to camp-seo.
- Run the draft through camp-voice's avoid-list and self-audit before handing it over.

## What this skill will not do

- Invent facts, prices, quotes, accreditations, or results, or promise a child a good time.
- Use a child's photo, name, or quote without consent.
- Manufacture urgency, like "only two spots left" when it is not true.
- Decide which pages the site needs (see camp-seo) or write paid ad copy (see camp-ads).
- Restate the voice rules, which live in camp-voice.

## Grounded in

Standard conversion-copywriting practice, plus honest-advertising rules. Claims on a camp's site about safety, outcomes, or reviews have to be true and able to be backed up.

- US FTC advertising and marketing guidance: https://www.ftc.gov/business-guidance/advertising-marketing
