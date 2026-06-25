---
name: camp-aeo
description: When the user wants a summer camp to be recommended, cited, or surfaced by AI assistants and answer engines such as ChatGPT, Perplexity, Google AI Overviews, Gemini, and Copilot. Use for AEO, answer engine optimization, generative engine optimization, GEO, LLM optimization, getting recommended by ChatGPT, showing up in AI search or AI Overviews, getting cited by AI, llms.txt, or when AI keeps suggesting other camps. For classic search engines see camp-seo, and for the page copy itself see camp-website-copy.
summary: Get your camp recommended by AI answer engines.
category: marketing
icon: sparkle
examples:
  - "When parents ask ChatGPT for a camp like ours, why don't we come up?"
  - "Turn our FAQ into answers ChatGPT will quote."
  - "Make sure AI gets our dates, ages, and prices right when parents ask."
order: 3
status: published
version: 1.0.0
---

# camp-aeo

Make yours the camp an AI recommends when a parent asks for one. More parents now open ChatGPT, Gemini, or Perplexity and ask "what's a good overnight camp near us for a shy ten-year-old" instead of scrolling a search page. This skill carries full answer-engine and generative-engine optimization practice, with a camp-specific layer on top.

It is written for you, the agent. Shape the output to the director, but keep the method intact. Answer engines change fast and never guarantee a mention, so give direction rather than promises. Honesty is central here: an assistant recommends camps it can verify, so the goal is to be genuinely accurate, consistent, and reputable, not to trick it.

If the camp-overview skill is available, draw on it for industry context (the directories and advisors parents use, accreditation, how families choose). This skill assumes that grounding but does not require it.

camp-aeo and camp-seo share a foundation: accurate facts, a strong Google Business Profile, genuine reviews, and clean structured data help both. Do not redo that work here; build on it and add the AI-citation layer.

## Ask first

Start from what is known, then ask only for the gaps.

**1. Read the camp's context before asking anything.**
- If a camp profile exists (`.agents/camp-profile.md` or `.claude/camp-profile.md`), read it for the durable facts (name, type, location, programs, ages, accreditation, voice, positioning). Do not re-ask what it answers.
- If no profile exists, offer to capture one with the camp-profile skill, then continue either way.

**2. Ask only the task-specific gaps** for AI visibility:
- The real questions parents ask an assistant, in their words ("best sleepaway camp near [town] for a first-timer," "affordable summer day camps in [city]," "is [camp] any good").
- Current AI presence: have they checked what ChatGPT, Gemini, or Perplexity say when asked for a camp like theirs? Are they mentioned, and what do the engines get wrong?
- Where their facts already live: site, Google Business Profile, camp directories, association listing, review sites, and whether those facts agree with each other.
- What genuinely makes the camp the right fit for particular families. AI recommends by fit, so this is the raw material.

**3. How far to go (the depth dial).** Match it to the director's goal and how much they want to take on. Default to the quick wins, and offer to go deeper.

- **Quick wins (low effort):** make the camp's facts accurate, consistent, and public; shore up reviews; let AI crawlers in; check what AI says about the camp today.
- **Solid setup (medium effort):** answer real parent questions in extractable form, claim the third-party presence AI pulls from, and keep it fresh.
- **Full build (high effort):** structured data, machine-readable files, monitoring across platforms, and full topical coverage.

Read their expertise and adjust how much you explain, not how sound the plan is.

## How AI picks a camp to recommend

A few realities shape everything below, and they are the "why" behind the steps:

- **AI recommends a small fraction of local businesses and filters out the weak ones.** Recent local-visibility research found assistants surface only a small share of businesses for a given query and skew toward higher-rated ones. Accurate facts and genuine, recent, well-rated reviews are what get a camp considered at all.
- **Inconsistent facts cost recommendations.** When a camp's name, location, ages, or dates differ across its site, Google Business Profile, and directories, models lose confidence and recommend a camp they are surer about. Make the core facts identical everywhere.
- **AI cites third parties more than your own site.** A camp is far likelier to be surfaced through an ACA listing, a reputable directory, or review sites than through its own homepage alone.
- **The engines differ.** Gemini and Google AI Overviews lean on Google Maps and your search presence (so the camp-seo work feeds them directly); ChatGPT draws on Bing plus third-party sources and favors fresh content; Perplexity rewards FAQ structure and freshness; Claude prizes factual precision. For the per-platform detail and which to prioritize, see `references/ai-platforms.md`.

## Work in order of leverage

### 1. Make your facts accurate, consistent, and public (Quick wins)

State the facts an assistant needs to describe and recommend you, in plain text on your own pages, and make them match everywhere else:

- The essentials: camp type, location and the area served, ages, programs, session dates, price range, and accreditation.
- The fit: who the camp is right for (first-timers, sporty teens, kids who need quiet, dietary needs met). AI matches a family's need to a camp, so say plainly who thrives here.
- Keep these identical across the site, the Google Business Profile, and every directory. Gemini in particular is grounded in Google Maps, so an accurate, complete Business Profile is a direct line into its answers (this is camp-seo work; lean on it).

### 2. Reviews and reputation (Quick wins)

Assistants skew toward higher-rated places and read review text for fit. So genuine, recent, well-rated reviews on Google and the main directories matter as much for AI as for search. Earn them steadily and reply to them (see camp-seo for the how). Never buy or fake them; beyond the FTC and platform rules, models cross-check and inconsistency hurts.

### 3. Let AI in (Quick wins)

A camp can be invisible to AI by accident:

- Check `robots.txt` does not block the AI crawlers. To be citable, allow GPTBot and ChatGPT-User (ChatGPT), PerplexityBot, ClaudeBot and anthropic-ai (Claude), Google-Extended (Gemini and AI Overviews), and Bingbot (Copilot). The full block is in `references/ai-platforms.md`.
- Make sure the key facts render in plain HTML, not only after heavy JavaScript. If the page is blank until scripts finish, assistants and agents may see nothing.

### 4. Answer real parent questions (Solid setup)

This is where camps win citations, and where the FAQ content that no longer earns Google rich results still pays off. Take the actual questions parents ask an assistant and answer each one directly, in their words:

- Lead each answer with the answer, in about 40 to 60 words, then add detail. Assistants extract self-contained passages, not whole pages.
- Use headings phrased the way a parent asks ("How much does a two-week session cost?", "Is the camp good for a first-time camper?").
- Add a fit section: who this camp is right for, and honestly who it is not. Fit content is unusually powerful for AI recommendation.
- For "[Camp A] vs [Camp B]" or "best camps for X" questions, a clear comparison table or a short, honest list beats prose.

Copy-paste block patterns with camp examples (answer block, FAQ, fit, comparison) are in `references/answer-content.md`.

### 5. Be where AI looks (Solid setup)

Build the third-party presence assistants actually cite for camps:

- Your ACA (or provincial association) accreditation and its public listing or "find a camp" directory.
- Reputable camp directories and advisor or referral services parents use.
- Genuine reviews on Google and those directories.
- Local press, and authentic presence where parents discuss camps (community forums, local parent groups). Participate honestly; never astroturf.

### 6. Structure and freshness (Solid setup)

- Keep answer passages self-contained, so they make sense lifted out of the page.
- Show a visible "last updated" date and refresh dates, prices, and sessions each year. Several engines weight freshness heavily, and a current page beats a stale one even if the stale one once ranked.
- Cover the whole topic, not one phrase. Assistants fan a question out into related ones, so a page (or site) that answers the surrounding parent questions gets pulled in more often.

### 7. Structured data and machine-readable facts (Full build)

- Add schema so engines can parse you: `LocalBusiness`, `Course` for programs, `Event` for sessions, and `FAQPage` for your question-and-answer content. (FAQ markup no longer earns Google rich results, but it still helps non-Google engines, especially Perplexity.) Reuse the camp JSON-LD in camp-seo's `references/schema-examples.md` and add FAQPage there.
- Make pricing legible. Camps that hide all pricing get skipped on cost questions; a clear public price range, or a simple machine-readable facts page, lets assistants include you.
- Optional and advanced: an `llms.txt` summarizing the camp and linking key pages. Treat newer agent formats (such as OKF) as register-early experiments, not priorities for most camps.

### 8. Check what AI says now, then watch it (all tiers)

You cannot improve what you have not looked at:

- Run the camp's main parent queries through ChatGPT, Gemini, Perplexity, and Google. Note whether the camp appears, who does instead, and what the engines get wrong about it.
- Watch how the camp is described, not only whether it appears. An assistant that names you but gives the wrong ages or price, or describes the camp faintly, costs enrollments as surely as leaving you out. Wrong or weak framing usually traces back to stale or inconsistent facts (steps 1 and 3) or to what third-party sources and reviews say (step 5).
- Fixing the wrong facts is often the fastest win.
- Re-check every month or two; AI answers shift, and so does who is cited.

## Deliver a prioritized plan

Scale the plan to the chosen tier and split it by effort:

- **This week (quick wins):** correct and align the core facts across site, Business Profile, and directories; shore up reviews; confirm AI crawlers are allowed; run the "what does AI say about us" check.
- **This season (the build):** answer the real parent questions in extractable form, claim the directory, association, and review presence, and keep it fresh.
- **Full build (if chosen):** schema, machine-readable facts, and monthly monitoring.

For each item, say what to do, why it matters, and the rough effort. Then hand off: camp-seo for the search and Business Profile foundation, camp-website-copy to write the fit and FAQ content this calls for, and camp-referrals for earning the genuine reviews this depends on.

## What this skill will not do

- Promise that an AI will mention or recommend the camp. No one can.
- Invent facts, accreditations, reviews, or rankings to game a model. This is a child-safety field; accuracy is non-negotiable.
- Use hidden, manipulative, or inauthentic tactics (fake community posts, scaled doorway content) that platforms penalize.
- Replace the search work (see camp-seo) or write the page copy (see camp-website-copy).

## Grounded in

This is an emerging area, so the durable principle is simple: be accurate, consistent, and genuinely reputable, because models recommend camps they can verify. Specifics change fast, so check current platform behavior before relying on it.

- Google's guidance on AI features and your site: https://developers.google.com/search/docs/fundamentals/ai-optimization-guide
- Google Search Essentials: https://developers.google.com/search/docs/essentials
- American Camp Association: https://www.acacamps.org
- US FTC guidance on reviews and endorsements: https://www.ftc.gov/business-guidance/advertising-marketing
