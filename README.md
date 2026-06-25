```
 █▀▀ █▀█ █▄█ █▀█   █▀▀ █ █ ▀█▀ █   █   █▀▀
 █   █▀█ █ █ █▀▀   ▀▀█ █▀▄  █  █   █   ▀▀█
 ▀▀▀ ▀ ▀ ▀ ▀ ▀     ▀▀▀ ▀ ▀ ▀▀▀ ▀▀▀ ▀▀▀ ▀▀▀
```

# Camp Skills

Agent skills for running a summer camp. A starting set for directors and staff, for use in Claude, ChatGPT, or any AI assistant.

## Using a skill

Install the whole set into your coding assistant (Claude Code, Cursor, Codex, Copilot, Gemini):

```
npx skills add campfront/camp-skills
```

Or add a single skill:

```
npx skills add campfront/camp-skills --skill camp-seo
```

See the [skills CLI docs](https://www.skills.sh/docs) for how the installer maps into each assistant.

Not using a coding tool? Every skill also works in the Claude or ChatGPT apps: open one on [camp-skills.com](https://camp-skills.com), copy its Markdown, and paste it into a chat. To add it as a reusable skill, follow your assistant's guide: [Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude) or [ChatGPT](https://help.openai.com/en/articles/20001066-skills-in-chatgpt).

## Updating

Re-run the install to get the latest:

```
npx skills add campfront/camp-skills
```

This refreshes the shipped skill files and adds any new ones. It never touches your camp's own details in `.agents/camp-profile.md`, so your setup survives every update. See [VERSIONS.md](VERSIONS.md) for current versions, and [RELEASING.md](RELEASING.md) for how versioning works.

## How they work

Three foundational skills give the agent its bearings. The task skills read those first, so you set your camp up once and everything else builds on it.

- **camp-overview**: industry context for how camps run, so the agent reasons like someone who knows the field.
- **camp-profile**: your camp's own details, so suggestions fit your camp rather than a generic one.
- **camp-voice**: how your camp sounds in writing, so anything for families reads like you.

The rest cover marketing, programs, and hiring.

### Marketing

- **camp-website-copy**: Landing, enrollment, and program-page copy that converts.
- **camp-seo**: Get found by local parents searching for a camp.
- **camp-aeo**: Get your camp recommended by AI answer engines.
- **camp-ads**: Paid social and search ads that fill your sessions.
- **camp-social**: On-brand social posts and a posting rhythm for the season.
- **camp-referrals**: Turn happy families into referrals and reviews.
- **camp-emails**: Enrollment, re-enrollment, newsletters, and reminders, in your voice.

### Programs

- **session-scheduler**: Daily and weekly schedules and themed program weeks.
- **activity-planner**: Games and activities by age, group size, weather, and energy.
- **evening-program**: Campfire and all-camp evening programs kids remember.

### Hiring

- **staff-job-post**: Counselor and specialist job posts that fill your roles.

## Using them well

Treat each skill as a starting point and adapt it to your camp. The agent supplies the method and a first draft. What makes the result good is your judgment about your campers, your families, and your season. Anything that touches camper safety, supervision, or local regulation should be reviewed by the people responsible for it at your camp, and by your accreditor where you have one.

## Repository structure

Skills live in `skills/`, one folder each. The three foundational skills load first; the task skills build on them.

```
skills/
  camp-overview/      foundational
  camp-profile/       foundational
  camp-voice/         foundational
  camp-seo/           task skill
  session-scheduler/  task skill
  staff-job-post/     task skill
  ...
```

Each folder holds a `SKILL.md` (instructions plus frontmatter) and optional `references/`, `assets/`, and `scripts/`. See [CONTRIBUTING.md](CONTRIBUTING.md) for the format.

## Contributing

Camp Skills is an open collection. Request a skill, improve one, or add your own. See [CONTRIBUTING.md](CONTRIBUTING.md) for the skill format and the bar we hold skills to, and open an issue if you have a question or an idea.

## License

MIT. See [LICENSE](LICENSE).

---

Brought to you by [Campfront](https://campfront.com).
