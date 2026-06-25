# Answer content patterns for camps

Load this when writing the content that gets a camp cited by AI. Assistants extract self-contained passages, so each block below is built to be lifted out and quoted cleanly. Write for parents first; these structures just make the good answer easy to extract. Writing the final voice is camp-website-copy's job; this defines what each block must contain.

Two rules run through all of them:

- **Lead with the answer.** Put the direct answer in the first sentence (about 40 to 60 words), then add detail. Do not bury it.
- **Be specific and honest.** Real numbers, dates, and named facts get cited; vague claims ("the best summer of their life") do not, and overclaiming erodes the trust models are checking for.

## Answer block (for a single parent question)

Use as the standalone answer to one question.

```markdown
### How much does a two-week session cost?

A two-week overnight session at Camp Wildwood is $2,400 for summer 2026, which covers lodging, all meals, activities, and equipment. Sibling and early-bird discounts are available, and camperships (financial aid) cover part of tuition for families who need it. Transport from Denver is an optional $90 add-on.
```

## FAQ block (several questions on one page)

The home for the questions parents actually ask an assistant. Pair it with FAQPage schema (see camp-seo's schema reference). Phrase each heading the way a parent would type or speak it.

```markdown
## Common questions from parents

### Is the camp good for a first-time camper?
Yes. About a third of our campers each summer are first-timers, and cabins pair new campers with returning ones. Counselors are trained in homesickness support, and first-night routines are built to settle nervous kids.

### What are the ages and group sizes?
We serve ages 8 to 15, grouped in cabins of 8 to 10 by age, with two counselors per cabin (a 1 to 5 staff ratio).

### What if my child has dietary needs or allergies?
Our kitchen handles common allergies and dietary needs, including nut-free, gluten-free, and vegetarian. Families share details on the health form, and the health center manages any medications.
```

Tips: use natural question words (what, how, when, is, does); match the "People also ask" phrasing from search; keep each answer roughly 50 to 100 words.

## Fit block (who this camp is right for)

Unusually powerful for AI, because assistants match a family's need to a camp. State who thrives here, and honestly who might not.

```markdown
## Who Camp Wildwood is right for

Camp Wildwood suits kids who love the outdoors and want a traditional, screen-free overnight experience with a strong cabin community. It is a good first sleepaway camp: sessions start at one week, and staff are trained to support homesickness.

It is less of a fit for a child looking for a single-sport intensive or a specialty academic program, where a focused specialty camp would serve them better.
```

## Comparison block (for "best camp for X" or "A vs B")

A clear table or short, honest list beats prose for these queries. Stay fair; models discount obviously biased comparisons.

```markdown
## Day camp or overnight camp: which fits your child?

| Consider | Day camp | Overnight camp |
|----------|----------|----------------|
| Nights away | Home each night | On site for the session |
| Best for | Younger or first-time campers, working-parent childcare | Building independence, deeper friendships |
| Typical length | A week at a time, repeatable | One to several weeks |
| Cost | Lower per week | Higher, includes lodging and meals |

Bottom line: a younger or anxious child often starts with day camp or a short overnight session, then moves to longer sessions as they are ready.
```

## Authority tactics (what makes a passage citable)

Layer these into the blocks above. Each raises the chance an assistant quotes you:

- **Cite real sources.** Attribute safety or developmental claims to a named body ("the American Camp Association recommends...") rather than asserting them.
- **Use specific numbers with context.** "A 1 to 5 counselor-to-camper ratio," "92% of families returned in 2025," not "great staff" or "most families come back." Only real figures; never invent them.
- **Name your credentials.** Accreditation, staff certifications (lifeguard, Wilderness First Aid), and years running. These are the trust signals models weigh.
- **Show the date.** A visible "last updated" and current-year dates and prices signal freshness, which several engines weight heavily.

## What to avoid

- Marketing fluff with no facts ("an unforgettable summer"). It does not get cited.
- Writing a separate "for AI" version of a page. Write one good page for parents; these structures serve both. Fragmenting content to bait AI can trip spam policies.
- Hiding the answer below scene-setting. The first sentence should answer the heading.
