---
name: camp-seo
description: When the user wants a summer camp to be found in search, including local SEO, Google Business Profile, program or landing pages built to rank, technical SEO, structured data, or fixing low search visibility. Use for "SEO," "rank for summer camps near me," "Google Business," "get found on Google," "our site doesn't show up," "local search," "schema," or "keywords for our camp." For the copy on those pages see camp-website-copy; for being recommended by AI assistants see camp-aeo; for paid placement see camp-ads.
summary: Get found by local parents searching for a camp.
category: marketing
icon: search
examples:
  - "Help us rank for 'summer camp near me' in local search."
  - "Which program pages should we build to rank for what parents search?"
  - "Get our Google Business Profile ready before enrollment opens."
order: 2
status: published
version: 1.0.0
---

# camp-seo

Help local parents find your camp in search, and build pages that can rank. Camp search is local and seasonal: a parent looking for a camp in their area, usually months before summer. The job is to be the clear right choice in that area, before demand peaks, on a site search engines can crawl and trust.

This skill carries full SEO best practice with a camp-specific layer on top. It is written for you, the agent. Shape the output to the director in front of you, but do not water down the underlying method. Rankings depend on factors no page controls, so give direction, never a guaranteed position or date.

If the camp-overview skill is available, draw on it for industry context (the camp year, the enrollment journey, jurisdiction). This skill assumes that grounding but does not require it.

## Ask first

Start from what is already known, then ask only for the gaps. Three things shape the plan: the camp, the task specifics, and how far they want to go.

**1. Read the camp's context before asking anything.** A director should not have to re-explain their camp to every skill.

- If a camp profile exists (`.agents/camp-profile.md` or `.claude/camp-profile.md`), read it. It holds the durable facts: name, type, location and jurisdiction, programs and ages, voice, accreditation, website, and what makes the camp different. Use it, and do not re-ask what it already answers.
- Draw on the camp-overview skill for how camps work in general.
- If no profile exists, offer to capture one with the camp-profile skill (a few minutes, reused by every skill), then continue either way.

**2. Ask only the task-specific gaps** that a profile would not hold and SEO needs:

- The towns or areas to target in search, which can be narrower than where families currently come from.
- Which programs and ages to prioritize ranking for this season.
- Whether the Google Business Profile is claimed and verified. Fixing one differs from building one.
- Reviews: how many, how recent, and where. This is the biggest local lever, so it sets the first priority.
- The plain words parents would type. Usually "summer camp + town," or "[sport or art] camp for [age]." Use their words, not industry terms.

**3. How far to go (the depth dial).** Match it to the director's goal and how much they want to take on. Default to the quick wins, and offer to go deeper.

- **Quick wins (low effort):** the few highest-impact actions, mostly free, no site rebuild. For a busy director who wants progress this week.
- **Solid setup (medium effort):** the seasonal foundation, the program pages, and the habits that compound. For a camp investing a season into being found.
- **Full build (high effort):** everything, including technical SEO, structured data, and trust signals. For a camp or its web developer that wants to compete hard.

Read their expertise too. A beginner wants plain steps and done-with-you help; someone with a developer wants a spec to hand over. Adjust how much you explain, not how sound the plan is. Each step below is tagged with the lowest tier it belongs to.

## Work in order of leverage

For a local camp, effort pays off in roughly this order. Do the early steps first; they move results faster than anything on the website.

### 1. Google Business Profile (Quick wins)

For local searches and Google Maps, the profile often outweighs the website. An unverified profile cannot appear in the local results at all, so verification comes first.

- **Claim and verify** the profile before anything else.
- **Primary category** is the single strongest relevance signal. Choose the most specific accurate one ("Summer camp" or "Day camp"), then add secondary categories for what you genuinely offer ("Sports school," "Art school").
- **Business name** must match real-world signage. Do not append keywords like "Camp Wildwood Summer Camp Austin." Google now suspends profiles for this.
- **Fill every field**: hours including seasonal hours, service area, phone, website, and the services and attributes lists. Each attribute you complete is another search you can match.
- **Description**: a natural paragraph with one or two place words worked in. Readability first; forced keywords backfire.
- **Photos**: add real ones regularly (camp in action, facilities, staff). Photo activity is a trust and ranking signal, and strong photos earn more clicks and calls.
- **Posts**: post roughly weekly through the active season (open house, early-bird deadline, sessions filling). Posts expire after seven days, so a steady cadence keeps the profile active, which itself helps ranking.

### 2. Reviews (Quick wins)

Reviews are the largest prominence signal, and recency is weighted heavily: forty reviews from this year and last usually outrank two hundred from five years ago. So aim for a steady flow of reviews rather than one big push.

- Ask every happy family at the moment of peak goodwill (end of session, the proud-parent pickup), with a direct link to the review form.
- Keep a consistent flow into each new season rather than one burst.
- Reply to every review, positive and negative. Calm public responses to criticism reassure the next parent reading.
- Never buy, incentivize, or fake reviews. It violates Google's policy and the FTC's reviews rule, and risks the whole profile.

### 3. Fix the pages you already have (Quick wins)

Before building anything, correct the basics on existing pages, because they are fast and they matter:

- One clear **title tag** per page, 50 to 60 characters, primary keyword near the front, brand at the end: `Soccer Day Camp in Denver, Ages 6-12 | Camp Wildwood`.
- One **H1** per page that names the program and place.
- A **meta description**, 150 to 160 characters, written to earn the click (benefit, place, season, a call to action).
- The primary keyword in the **first 100 words** of the page, used naturally, never stuffed.
- Consistent **name, address, and phone (NAP)** everywhere it appears, matching the Google Business Profile exactly. Mismatches confuse the local algorithm.

### 4. Map searches to pages (Solid setup)

The core mistake is one page trying to rank for everything. Give each real search its own page. A parent searching "soccer camp for 8 year olds in Denver" should land on a page about exactly that, not a generic homepage.

To find the phrases, use what is free before reaching for tools: Google autocomplete, the "People also ask" box, and the "Related searches" at the foot of a results page all show real phrasing. If Search Console or an SEO tool (Ahrefs, Semrush) is connected, pull actual query and ranking data instead of guessing. Match the parent's own word, not the industry term: they search "sleepaway camp," not "overnight residential," say "day camp," and add "near me" to almost everything, so a page in their words matches more of what they type. Sort phrases by intent, because intent decides the channel: early-research terms ("summer camps 2026," "things to do this summer") reward content and patience, while ready-to-enroll terms ("soccer camp denver july," "[camp] registration") are where SEO and camp-ads compete hardest.

Then build one focused page per program-and-place, and per distinct age band where it matters. This is the local version of the proven "[service] in [location]" page pattern, with one rule that keeps it safe: every page must carry genuine, unique value (real dates, schedule, location, price, photos), never the same text with the town name swapped. Thin, near-duplicate pages get filtered or penalized, so build a few real pages rather than many empty ones.

Page templates, with a worked example for a soccer day camp in Denver:

- **URL**: short, readable, hyphenated, lowercase, in a subfolder: `/programs/soccer-day-camp-denver/`
- **Title tag**: `Soccer Day Camp in Denver, Ages 6-12 | Camp Wildwood`
- **H1**: `Soccer Day Camp in Denver`
- **Meta description**: `A week of skills, games, and fun for ages 6-12 in central Denver. Summer 2026 sessions filling now. See dates and enroll.`
- **Body**: answer the real questions (ages, dates, daily schedule, location and parking, price, what to bring, safety and ratios), in the camp's own voice.

Writing that body copy is camp-website-copy's job. This skill decides which pages exist and what each must target. Work the season and place into the words too ("summer 2026," the town, the nearby towns you serve).

### 5. Site structure and internal links (Solid setup)

How pages connect tells search engines what matters and helps parents navigate:

- **Hub and spoke**: a single "Programs" or "Camps" hub page links to every program page, and each program page links back. This concentrates authority and makes the set easy to crawl.
- **Three-click rule**: any important page should be reachable within three clicks of the homepage.
- **Descriptive internal links**: "our soccer day camp," not "click here." No orphan pages (every page needs at least one internal link to it).
- **Breadcrumbs** (Home > Programs > Soccer Day Camp) that mirror the URL, giving free internal links and clearer structure.
- **One page per search**: do not let two pages chase the same term, which splits their strength (keyword cannibalization).
- If you serve several towns, a genuine page for each, never thin doorway copies.

### 6. Technical foundations (Full build)

Search engines must be able to crawl, index, and load the site, or nothing above ranks. The essentials: a crawlable site with a clean XML sitemap and sane robots.txt; correct canonical tags so duplicates do not compete; fast, mobile-first pages (most parents search on a phone); and HTTPS everywhere. Core Web Vitals targets are LCP under 2.5s, INP under 200ms, CLS under 0.1.

For the full checklist (crawlability, indexation, canonicalization, Core Web Vitals, mobile, HTTPS, URL hygiene), and the common traps, read `references/technical-seo.md`.

One caveat worth stating up front: a raw page fetch or `curl` cannot see structured data injected by JavaScript (many site builders do this), so never report "no schema" from a fetch alone. Verify with Google's Rich Results Test, which renders the page.

### 7. Structured data, or schema (Full build)

Structured data is JSON-LD in the page that tells search engines what it is, which can earn richer results. Implement it completely and accurately (mark up only what is really on the page); partial or false markup produces no benefit and risks trust. Match the type to the page:

- **LocalBusiness** on the homepage or contact page: name, address, phone, hours, geo coordinates.
- **Course** on program pages: the offering, provider, what it teaches.
- **Event** on dated sessions and open houses: `startDate` and `endDate` in ISO-8601 with time zone, `location`, registration `offers`, and `eventStatus`.
- **BreadcrumbList** on any page with breadcrumbs.

Combine types on one page with `@graph`. Validate every block in the Rich Results Test before shipping. Note: FAQ rich results no longer show in Google Search (since May 2026), so do not add FAQ schema for ranking; FAQ content can still help with AI assistants (see camp-aeo).

Copy-paste JSON-LD for a camp (LocalBusiness, Course, Event, BreadcrumbList, and a combined `@graph`) is in `references/schema-examples.md`.

### 8. Trust signals (Quick wins to Full build)

Search rewards sites that show real-world credibility (often summarized as experience, expertise, authoritativeness, trustworthiness), and for a camp the same signals are exactly what convinces a parent. So this work pays twice:

- Accreditation (ACA in the US, or your national body) shown clearly.
- Named staff with relevant credentials and certifications (lifeguard, first aid, coaching).
- Safety information, ratios, and policies that a parent can find.
- Real photos and recent reviews, not stock imagery.
- Clear contact details, address, and a privacy policy.

These help ranking and conversion at once, and they feed directly into being recommended by AI assistants (see camp-aeo).

### Seasonal timing (all tiers)

Camp search is sharply seasonal, and a new page needs two to three months (longer for competitive terms) to reach its ranking potential, so publishing late is the most common wasted effort. The catch: the search peak depends on the camp type, and the bigger the commitment, the earlier parents search. Aim for a page to be ranking before its type's peak, which means publishing well ahead of it:

- **Overnight or sleepaway** searches peak in October; it is the considered, research-driven decision, made early. Have those pages live by mid-summer.
- **Teen and high-school programs** peak in January. Have those pages live by October. (January is also when registration interest spikes across the board, so it is the moment to be visible and current.)
- **Day camp and generic "camps near me"** peak in late spring, close to the season. Have those pages live by late winter, though earlier always helps.

Whichever applies, run the calendar backward from your own peak, not a single date. Through the run-up, keep posting, gathering reviews, and refreshing pages (dates, prices) to hold freshness without losing accumulated ranking. Off-season, keep the profile active rather than going dark; steady activity compounds.

SEO is a slow channel: expect little in the first sixty days, with the payoff building over months. For fast, peak-season reach, pair it with camp-ads.

## Deliver a prioritized plan

Do not hand back a lecture. End with a plan scaled to the tier the director chose, split by effort, since their time is the real constraint:

- **This week (quick wins):** claim or verify the Google Business Profile, set the primary category, fix titles and missing meta descriptions, ask recent happy families for reviews.
- **This season (the build):** one page per program-and-place, internal-link structure, the posting and review habit, the calendar working back from January.
- **Full build (if chosen):** technical foundations, structured data, trust signals.

For each item, say what to do, why it matters, and the rough effort, so they can choose. Then hand off: camp-website-copy to write the pages this plan calls for, camp-ads to buy reach during the January-to-spring peak, and camp-aeo to be recommended by AI assistants as well as ranked.

## Measure

Watch a few signals so the work is directed, not guessed:

- **Google Search Console**: which queries show your pages, impressions and clicks, indexing problems.
- **Google Business Profile insights**: searches, calls, direction requests, website clicks.
- **Reviews**: count and recency trend.

Each month, check whether you actually appear in the local results for your main "[program] + town" searches, and fix the weakest step first.

## What this skill will not do

- Promise rankings, traffic, or timelines. Search is never guaranteed.
- Use tactics that risk penalties or suspension: keyword-stuffed business names, fake or incentivized reviews, doorway pages, hidden text, false schema.
- Write the page copy itself (see camp-website-copy) or buy placement (see camp-ads).

## Grounded in

Standard local-search practice and Google's own guidance, plus honest-review rules. The aim is to be genuinely findable and accurate, never to trick the algorithm. Specifics change often, so verify current rules before relying on them.

- Google Business Profile: https://www.google.com/business/
- Google Search Essentials: https://developers.google.com/search/docs/essentials
- Structured data and rich results: https://developers.google.com/search/docs/appearance/structured-data
- US FTC guidance on reviews and endorsements: https://www.ftc.gov/business-guidance/advertising-marketing
