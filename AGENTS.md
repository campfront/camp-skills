# AGENTS.md

Guidance for AI agents building or editing skills in this repo. Humans: start with [CONTRIBUTING.md](CONTRIBUTING.md).

## What this repo is

Camp Skills is an open, curated collection of agent skills for summer camps. Each skill lives in `skills/<name>/` with a `SKILL.md`. Three foundational skills (camp-overview, camp-profile, camp-voice) are read first; the task skills build on them.

## Before you build or edit a skill

1. Read [CONTRIBUTING.md](CONTRIBUTING.md) for the skill format and the bar.
2. Read the three foundational skills, plus a task skill like `camp-seo`, so your work matches the rest.
3. Read [skills/camp-voice/references/avoid-list.md](skills/camp-voice/references/avoid-list.md). Any copy a skill produces follows it.

## House rules

- **Match the pattern.** A skill carries the full best practice, adds a camp layer, asks about the camp first, and hands back an editable draft, never a template to paste.
- **Read the foundations, do not repeat them.** Task skills rely on camp-overview, camp-profile, and camp-voice.
- **Keep `SKILL.md` focused.** Under roughly 500 lines. Move depth into `references/`.
- **Frontmatter is required:** `name` (lowercase-hyphens, matches the folder), `description`, `summary`, `category`, `icon`, `examples`, `order`, `status`, `version`.
- **Never commit credentials or a real camp's private data.**

## Safety

Anything touching camper safety, supervision, behavior, or local regulation is sensitive. Do not ship it without sign-off from a qualified person. If a skill is built but not yet cleared, keep it out of `skills/` until it is.

## Working in the repo

- Branch first (`feat/...`, `fix/...`, or `docs/...`), never commit to `main`. The prefix matches the change type.
- Conventional Commits (`feat:`, `fix:`, `docs:`), scope optional (`docs(camp-seo): ...`).
- PR titles use the same Conventional Commit format. We squash-merge, so the title becomes the commit subject.
- Open a PR. Campfront reviews against the bar before merging.
