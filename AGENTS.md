# AGENTS.md — shared instructions for Codex and Cursor Agent

> **先读 / Read first:** /home/box/dev/TEAM_CONTEXT.md（规矩、目录、密钥位置、API 用法）；做审计、运营或市场的活时再读 /home/box/dev/TEAM_STATUS.md（分工、各 app 现状、文案规矩）。

Both Codex (CLI) and Cursor Agent (CLI) read this file. They take turns on this same local folder on the shared box, so keep it the single source of truth for how to work here.

## Project

- Project: Shenbee legal and policy pages, a static GitHub Pages site.
- Repo: `maliangone/legal` (private). Local checkout: `/home/box/dev/projects/legal`
- Non-repo artifacts (briefs, reviews, screenshots, assets, release files, logs): `/home/box/dev/work/legal/`
- Site source: root-level HTML files, `.nojekyll`, and `app-ads.txt`.

## Hard rules

- Solo developer: work directly on `main`. `git pull --rebase origin main` before starting, small commits, `git push origin main`. Never create branches or PRs.
- One agent writes at a time. Before you start, check `git status`; if there are uncommitted changes that are not yours, stop and report instead of overwriting. Commit (or clearly hand off) before you finish.
- Never print, paste or commit new secrets. Credentials live outside the repository; reference paths/env names only.
- Do not claim a page is correct without inspecting the rendered HTML or another concrete verification result.
- Do not change a live listing or publish a release unless the task explicitly asks for it.

## Site notes

- This checkout contains static privacy, terms, support, and data-deletion pages for several Shenbee apps, plus a root index page.
- There is no `pubspec.yaml`, `package.json`, or other build manifest in the repository; no application build or test command is defined here.
- Keep links, app names, contact details, and policy text consistent with the corresponding app pages and the shared team context.
- Local artifacts for this project belong under `/home/box/dev/work/legal/`, not in the site repository unless they are published page assets.
