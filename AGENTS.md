# AGENTS.md

GitHub **profile** repository (`yosoyignicion/yosoyignicion`). It is not a software project:
there is no build, test, lint, typecheck, or CI. `README.md` is rendered on the public GitHub
profile page, so edits here are user-facing.

## Editing rules
- `README.md` is **bilingual**: Spanish first, English second. Keep both halves in sync — any
  fact change (project stats, contact, availability, skills) must be applied twice.
- The language switch uses anchors `#-español` / `#-english`, generated from the headings
  `## 🇪🇸 Español` / `## 🇬🇧 English`. The explicit `<a id="...">` tags also depend on them.
  **Do not rename or re-emoji those headings** or the toggle links break.
- `assets/banner.svg` hardcodes the name, tagline, availability text and handle that also live
  in the README. Update the SVG when those change, not just the Markdown.
- Project facts (test counts, CI status, release tags, stack) are duplicated in `README.md` and
  `yosoyignicion.md`; update both when a linked project changes.
- `CV_Ignacio_Badenes_Tecnico.pdf` is linked as `./CV_Ignacio_Badenes_Tecnico.pdf` — keep the
  filename/path stable.

## Sources
- `README.md` — canonical public profile (ES/EN).
- `yosoyignicion.md` — long-form profile, currently untracked; treat as source material.
- `assets/*.svg` — hand-written SVGs, referenced by relative path; no generator.

## Verification
No automated checks exist. Preview the rendered Markdown (e.g. `grip`/GitHub preview) and
confirm SVG links, anchor links, and ES/EN parity before committing.

## Conventions
- Conventional Commits (existing history: `docs: ...`).
- `.engram/` is local agent state and is gitignored — never stage or commit it.
- Write in UTF-8; keep the formal, no-hype tone of the existing copy.
