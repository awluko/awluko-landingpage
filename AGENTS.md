# awluko-landingpage Agent Rules

Scope: Applies to `/Users/andrewlukosevic/Documents/Programming/awluko-landingpage` and overrides broader workspace rules for this repo.

## Project Context
- Site type: personal landing site + blog.
- Stack: Astro 4, Tailwind CSS 3.
- Deployment: GitHub Pages via GitHub Actions on push to `main`.

## Repository Map
- Pages: `src/pages`
- Blog content: `src/content/blog`
- Content collection config: `src/content/config.ts`
- Shared layout: `src/layouts/Base.astro`
- Global styles: `src/styles/global.css`
- Static assets: `public`

## Tooling and Commands
- Package manager: `npm` (use `package-lock.json`; do not switch package managers).
- Install: `npm install`
- Dev server: `npm run dev` (or `npm run start`)
- Production build: `npm run build`
- Production preview: `npm run preview`
- Astro CLI passthrough: `npm run astro -- <args>`

## Implementation Rules
- Keep changes focused on the user's request; avoid broad visual rewrites unless asked.
- Preserve existing Astro routing/content patterns unless a requested change requires restructuring.
- Prefer editing existing components/layouts over introducing new abstractions for small changes.
- For blog-related edits, keep frontmatter and slug behavior compatible with `src/content/config.ts`.
- Avoid adding dependencies unless clearly needed for the requested outcome.

## Verification
For any code/content change, run:
1. `npm run build`

When behavior or UI changes:
1. Run `npm run dev` or `npm run preview`.
2. Validate the affected route(s) manually.

If verification cannot run, state exactly what was blocked and why.

## Safety
- No destructive commands unless explicitly requested.
- Do not remove existing content/assets unless the user asks.

## Handoff Requirements
- List changed files.
- Summarize user-visible impact.
- Report verification commands and outcomes.
