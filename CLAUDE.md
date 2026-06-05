# CLAUDE.md

Guidance for Claude Code when working in this repository.

## What this repo is

This is Harry's **GitHub profile repository** (`HarryXin0919/HarryXin0919`). Because
the repo name matches the username, its `README.md` is rendered at the top of the
GitHub profile page at https://github.com/HarryXin0919.

It is **not** an application — there is no build, test, or runtime. The deliverable
is the rendered Markdown and the image assets it references.

## Layout

- `README.md` — the profile page. Hand-written HTML + Markdown (centered headers,
  shields.io badges, a 2×2 table of project cards).
- `assets/cards/` — PNG "cards" for featured projects, linked from the README:
  - `finditem.png`, `pantrypath.png`, `viralens.png`, `findit-website.png`

## Featured projects (linked from the README)

- **FindItem** — decentralized parts locator; search a part and the right storage bin
  lights up and beeps (ESP32-C3 · MQTT · FastAPI / Spring Boot)
- **pantrypath** — cheapest ingredient-substitution chain as a shortest-hyperpath
  problem (Python)
- **viralens** — hypothesis-driven analytics for Bilibili / YouTube creators
- **findit-website** — open-source landing page for FindItem

## Conventions

- **Badges** use shields.io with `style=for-the-badge`. Keep that style consistent
  when adding new ones, and group them in the same `<p align="center">` blocks by
  category (languages, hardware/frameworks, tooling).
- **Project cards** live in the 2×2 `<table>`. To add a project: add its PNG to
  `assets/cards/`, add a `<td>` linking to the repo, and add a matching bullet in the
  "Featured projects" list.
- Keep the tone concise and maker-focused, matching the existing voice.
- The README mixes raw HTML with Markdown — preserve the centered, badge-driven layout.

## Working in this repo

- No tests or CI to run; verify changes by checking that Markdown/HTML renders and that
  every referenced asset path exists.
- When changing an image, keep the filename stable so README links don't break, or
  update both the file and the reference together.
