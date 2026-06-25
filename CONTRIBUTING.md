# Contributing to Camp Skills

Camp Skills is an open collection, and we welcome new skills, improvements, and ideas. This guide covers how to contribute and the bar we hold skills to.

The collection is curated. Anyone can propose a skill, and Campfront reviews every change for quality, voice, and safety before it merges. We may edit a contribution to fit before merging.

## Ways to contribute

- **Request a skill.** Open an issue describing a job a camp needs done. This is the easiest way to help, and it shapes what we build next.
- **Improve a skill.** Spotted a better method, a clearer draft, or a fix? Open a PR. Keep the change focused.
- **Add a skill.** Build a new skill that fills a real gap. Read the bar below first.

## What makes a Camp Skills skill

Every skill follows the same shape. Before building one, read camp-overview, camp-profile, and camp-voice, plus a couple of task skills like camp-seo, so yours matches the rest.

- **Carries the full best practice.** A skill is the method an expert would use for the job, not a thin prompt. Detail that does not fit inline goes in `references/`.
- **Adds a camp layer.** It applies that method to summer camps specifically.
- **Asks first, then drafts.** It asks about the camp before it writes, and hands back an editable draft to adapt, never a template to paste.
- **Reads the foundations.** Task skills rely on camp-overview, camp-profile, and camp-voice rather than repeating them.
- **Sounds like us.** Any copy a skill produces follows the voice rules in [camp-voice/references/avoid-list.md](skills/camp-voice/references/avoid-list.md). This keeps the whole collection cohesive.
- **Respects safety.** Anything touching camper safety, supervision, or local regulation must say so and defer to the people responsible at the camp and their accreditor. We review these closely.

## Skill structure

A skill is a folder under `skills/`:

```
skills/your-skill-name/
  SKILL.md         required
  references/      optional, supporting detail the skill loads on demand
  assets/          optional, templates or data files
  scripts/         optional, executable helpers
```

`SKILL.md` opens with YAML frontmatter:

```yaml
---
name: your-skill-name          # lowercase, hyphens, matches the folder name
description: >                  # when to use this skill, rich with phrases a user would say
  When the user wants ...
summary: One line for the site and README.
category: marketing             # marketing, programs, or hiring
icon: search                    # a short icon keyword
examples:
  - "A thing a director might ask."
  - "Another."
order: 2                        # sort order within its category
status: published
version: 1.0.0                   # bumped per SemVer when the skill changes; see RELEASING.md
---
```

Then the instructions. Keep `SKILL.md` focused and under roughly 500 lines, and move depth into `references/`. Never commit credentials, API keys, or a real camp's private data.

## How to submit

1. Fork the repo and create a branch named for the change type: `feat/your-skill`, `fix/...`, or `docs/...`.
2. Make your change. Test it by installing from your fork: `npx skills add <your-username>/camp-skills --skill your-skill-name`.
3. Open a PR. Title it as a Conventional Commit (`feat(scope): ...`, `fix: ...`, `docs: ...`) — we squash-merge, so the title becomes the commit. In the description, say what the skill does and who it is for.

Campfront reviews against the bar above and may suggest edits, or adjust for voice and consistency, before merging.
