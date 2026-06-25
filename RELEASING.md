# Releasing Camp Skills

How the collection is versioned and how people get updates. For how to contribute a change in the first place, see [CONTRIBUTING.md](CONTRIBUTING.md).

## Status: pre-release

Camp Skills has not been versioned yet. Until the first release, everything is the `1.0.0` baseline-in-progress: merge changes the normal way and **do not bump anything**. There is no published version to increment from, so every edit simply folds into the baseline.

Versioning begins the moment `v1.0.0` is tagged. From then on, the rules below apply.

## How versioning works

Two layers, both [SemVer](https://semver.org/):

- **Per-skill version** — a `version` field in each skill's `SKILL.md` frontmatter. Skills evolve independently, so one can move without re-versioning the rest.
- **Collection version** — one number for the whole set, recorded as a git tag and GitHub Release (`v1.2.0`).

[VERSIONS.md](VERSIONS.md) lists every skill with its current version and last-updated date. It exists so an agent (or a person) can compare against an installed copy and tell whether it is behind.

## What counts as a change

These are prose skills, not code, so "breaking" means a break in what the user relies on:

- **Patch** (`1.0.0` → `1.0.1`) — wording, clarity, fixed or better examples. No change to what the skill does.
- **Minor** (`1.0.0` → `1.1.0`) — additive: a new skill, or a substantive new section that gives the agent a capability it did not have, without changing existing behaviour.
- **Major** (`1.0.0` → `2.0.0`) — a contract break: a skill renamed or removed, its trigger or scope narrowed so it stops firing where people relied on it, or a referenced file path moved (for example, where `camp-profile` saves its file).

The collection version takes the highest bump among the skills changed in that release.

## How people get updates

Updates are **pull, not push.** The skills CLI copies skill files into the user's project; there is no live link or auto-update. So:

- A user updates by **re-running the install** — `npx skills add campfront/camp-skills` overwrites the skills with the latest from the repo.
- Installs are additive-overwrite: re-running refreshes shipped skills and adds new ones, but does not clean the folder. A renamed or removed skill leaves an old copy behind until the user deletes it — call those out in the release notes.
- Because updates are opt-in, most users run an older copy until they reinstall. `VERSIONS.md` is the mitigation: an agent can read it and notice it is behind.

### Reinstalling does not touch a camp's own data

A camp's context lives at `.agents/camp-profile.md` (with `.claude/camp-profile.md` as a fallback) — a file at the user's project root, outside any skill folder. Reinstalling refreshes the **shipped skill files** and never writes to that profile, so a user's setup survives every update.

The one thing a reinstall does overwrite: **local edits a user made to a shipped `SKILL.md`.** The place to customise is the profile, not the skill text.

## Cutting a release

1. Branch, make the change, and merge it the normal way (see [CONTRIBUTING.md](CONTRIBUTING.md)).
2. Bump the `version` of each changed skill in its `SKILL.md` frontmatter.
3. Update those skills' rows in [VERSIONS.md](VERSIONS.md) — version and date.
4. Tag the merge commit and cut a GitHub Release, with notes covering what changed and anything users must clean up:
   ```
   gh release create v1.1.0 --notes "..."
   ```
5. Users pick up the change when they re-run `npx skills add campfront/camp-skills`.

## First release (v1.0.0)

The one-time setup, run as a single PR when we are ready to ship:

- Add `version: 1.0.0` to every skill's frontmatter.
- Create `VERSIONS.md` with every skill at `1.0.0`, dated that day.
- Add a one-line note to the README that reinstalling updates the skills but leaves `.agents/camp-profile.md` alone.

Then tag and release `v1.0.0`.

Claude Code plugin manifests (a `.claude-plugin/` folder) are intentionally left out for now; they can be added later to offer a `/plugin` install path alongside the CLI.
