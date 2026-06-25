---
name: camp-social
description: When the user wants social media posts or a posting plan for a summer camp, mostly on Instagram and Facebook, to keep families warm and reach new ones. Use for camp social media, Instagram or Facebook posts and captions, a content calendar or posting schedule, Reels or short video for a camp, what to post, or how often to post. It draws on camp-voice for the captions and camp-profile for the camp's voice and facts. For paid promotion see camp-ads, and for the page posts link to see camp-website-copy.
summary: On-brand social posts and a posting rhythm for the season.
category: marketing
icon: bubble
examples:
  - "Write three Instagram captions announcing our open week."
  - "Plan a month of off-season posts to keep families warm over winter."
  - "Turn today's five photos into a post that sounds like us."
order: 5
status: published
version: 1.0.0
---

# camp-social

Turn a camp's real moments into posts that keep its families warm and bring new ones in, mostly on Instagram and Facebook. This carries standard social-media practice with a camp layer on top.

It is written for you, the agent. Use camp-voice for the captions, camp-profile for the camp's voice and facts, and camp-overview for the camp year. One rule overrides everything else here: never post a child's image, name, or words without the family's consent and the camp's media release. More on that in the guardrails below, and it is not negotiable.

## Ask first

Start from what is known, then ask only for the gaps.

**1. Read the camp's context first.**
- If a camp profile exists (`.agents/camp-profile.md` or `.claude/camp-profile.md`), read it for the camp's voice and facts. Do not re-ask what it answers.
- Use camp-voice for the captions and its avoid-list, and camp-overview for the camp year.
- If no profile exists, offer to capture one with the camp-profile skill, then continue.

**2. Ask only the task-specific gaps:**
- Which platforms they use, and whether this is one post, a week, or a season plan.
- The point of it (keep current families warm, reach new ones, fill a session, announce an open house).
- What real content they have right now (photos, video, a camper or staff story), and whether they have consent to post it.
- Where they are in the camp year, and who runs the account and how much time they have.

**3. How far to go (the depth dial).** Match it to the director's goal and how much they want to take on. Default to a few strong posts, and offer to go deeper.

- **Quick wins (low effort):** a handful of strong posts for right now, in the camp's voice, from content they already have.
- **Solid setup (medium effort):** content pillars and a month or season of posts mapped to the camp year.
- **Full build (high effort):** a year-round calendar across Instagram and Facebook, a way to turn one moment into several posts, an engagement routine, and what to measure.

## Run the social

### 1. Pick the platforms and who you are talking to (all tiers)

For most camps the buyer is a parent, and parents are on **Instagram and Facebook**, so start there and do them well. TikTok and YouTube reach teens and can suit a teen program, but they take more time and raise the same child-safety questions, so only add them with a reason and the care below. Consistency on two platforms beats a thin presence on five.

### 2. Build around content pillars (Solid setup)

Decide a handful of recurring post types so you are not inventing each time. A workable camp mix:

- **Camp life:** real photos and short video of a normal day (the strongest content a camp has).
- **People and traditions:** a camper or staff spotlight, a tradition, a throwback.
- **Behind the scenes:** off-season prep, staff training, the site waking up for summer.
- **Reassurance for parents:** a day in the life, how homesickness is handled, what to pack. This doubles as trust and answers real questions (see camp-aeo).
- **Proof:** a real parent quote as a simple graphic, or a family's story, used with permission.
- **Announcements:** enrollment open, early-bird, an open house. Keep these a small share of the mix.

The full calendar and post-type ideas with caption examples are in `references/calendar-and-posts.md`.

### 3. Post to the camp year, not evenly (all tiers, scaled)

Camp interest rises and falls with the season, so move with it (this matches camp-overview and the calendars in camp-seo and camp-ads):

- **In season (summer):** real moments, short daily recaps. (Note: a private daily photo feed for enrolled families, often through the camp's management software, is a separate, operational thing from public marketing posts.)
- **Late summer:** closing highlights, and the first gentle "next summer" notes while the summer is still fresh for families.
- **Fall:** parents start researching, so open up behind-the-scenes and announce that enrollment is open.
- **December to April:** the main research and decision stretch, so this is where the highest-intent content goes (testimonials, day-in-the-life, program highlights, early-bird).
- **Spring:** the run-up, with staff introductions and packing and prep content.

### 4. What to actually post (Solid setup)

- Real photos and short video of this camp, never stock.
- In season, a short daily or few-times-a-week recap of real moments.
- Parent quote cards, and camper or alumni stories, used with permission.
- Reassurance posts that answer a real parent question.
- Write every caption in camp-voice: lead with the moment, keep it short, and add a soft next step only where it fits (an enrollment post has one, a pure camp-life post needs none).

### 5. Short video and Reels (Solid setup)

Short video reaches the most people on Instagram. Keep it 15 to 30 seconds of real camp moments, vertical, captions on (most parents watch with the sound off), with the hook in the first three seconds (a kid landing a kayak roll, the first-night cabin settling in).

### 6. Engage, do not just broadcast (Full build)

Reply to comments and DMs from parents, and repost what families share about the camp, with their consent. Keeping alumni and parent groups warm is some of the most valuable time you spend, because those families refer others (see camp-referrals).

### 7. Measure what matters (Full build)

Watch reach, saves, and shares more than likes, and watch profile visits and link clicks for buying interest. Social mostly builds awareness and trust rather than booking campers directly, so set that expectation: for direct enrollment, pair it with camp-ads and send people to the page from camp-website-copy.

### 8. Child safety and consent (all tiers, non-negotiable)

Posting children in public is the part to get right, every time:

- Get a signed photo and media release before posting any camper's image, name, or words. No consent, no post.
- Let families opt out, and honor it. Keep a list of children who must not appear.
- Do not post identifying details, such as a child's full name together with their cabin, schedule, or anything that shows where a specific child is and when.
- Follow the camp's own media policy and each platform's rules.

This protects the children in the camp's care and the camp itself, so it comes before any engagement goal.

## Deliver the posts

- For each post, give the caption (in camp-voice), a note on what the photo or video should show, and the platform it is for. For a plan, give the pillars and the rhythm scaled to the tier.
- Flag any post that needs photo consent before it can go out, and never assume consent.
- Run every caption through camp-voice's avoid-list and self-audit before handing it over.
- Send direct-enrollment work to camp-ads, and point links at the page from camp-website-copy.

## What this skill will not do

- Post a child's image, name, or words without consent, or reveal identifying details about a camper.
- Invent reviews, results, or testimonials.
- Promise outcomes the camp cannot stand behind.
- Buy reach (see camp-ads) or write direct messages to enrolled families (see camp-emails).
- Restate the voice rules, which live in camp-voice.

## Grounded in

Standard social-media practice, child-safety and consent norms, and honest-marketing rules. Get consent and follow the camp's media release before sharing any child, and make only claims the camp can back.

- US FTC guidance on endorsements and testimonials: https://www.ftc.gov/business-guidance/advertising-marketing
- American Camp Association: https://www.acacamps.org
