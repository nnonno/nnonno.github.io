# CLAUDE.md

## Project Overview
Personal academic webpage for Yifu Wu, built with Hugo and Hugo Blox Builder (academic-cv starter). Deployed via GitHub Actions to GitHub Pages.

## Tech Stack
- **Static site generator**: Hugo (v0.145.0)
- **Theme**: Hugo Blox Builder (`blox-tailwind` v0.3.1)
- **Deployment**: GitHub Actions -> GitHub Pages
- **URL**: https://nnonno.github.io/

## Key Directories
- `config/_default/` - Hugo configuration (hugo.yaml, params.yaml, menus.yaml, module.yaml, languages.yaml)
- `content/` - Site content (Markdown files)
- `content/authors/admin/_index.md` - Main bio/profile
- `content/_index.md` - Homepage sections
- `content/experience.md` - Experience page
- `assets/` - Theme assets (media, CSS overrides)
- `layouts/` - Template overrides
- `.github/workflows/publish.yaml` - CI/CD deployment workflow

## Build & Development
- Local dev: `hugo server` (requires Hugo v0.145.0 extended)
- Production build handled by GitHub Actions on push to `main`
- Hugo version must stay in sync across: `hugoblox.yaml`, `.github/workflows/publish.yaml`, `netlify.toml`

## Content Sources
- CV data lives in `/Users/wuyifu/workspaces/personal/Awesome-CV/examples/`
  - `cv_comprehensive/` - Full academic CV (summary, experience, education, publications, patents, projects, skills, honors, teaching)
  - `resume_nlp/` - NLP-focused industry resume

## Current Work Experience (on webpage)
1. **AWS GenAI** (Mar 2025 – Present) — B2B AI Application, multi-media text/image/video understanding
2. **Amazon Alexa Science** (Apr 2024 – Mar 2025) — LLM inference optimization, responsible AI guardrails
3. Earlier roles: CU Anschutz, AI Newsletter Startup, Purdue RA, Iowa State RA, U of Akron RA, Tsinghua Instructor, Haite SE

## Resume PDF
- `static/uploads/resume.pdf` — sourced from `cv_comprehensive.pdf` (full academic CV)
- Linked via the "Download CV" button on the homepage

## Important Notes
- `public/` and `resources/` are gitignored build artifacts - do NOT commit them
- `baseURL` in `config/_default/hugo.yaml` must match the GitHub Pages URL
- Hugo modules are managed via `go.mod` / `go.sum`
- Repo was renamed from `yifu_wu` to `nnonno.github.io` — remote and baseURL updated accordingly
- Education consolidated to 3 entries: PhD (Purdue), ME (Limerick), BS (HIT). Iowa State and U of Akron are listed as work/RA positions, not separate degree entries.
