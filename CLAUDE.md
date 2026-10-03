# CLAUDE.md

This repository is public on GitHub, and so is this file. Keep everything here public-safe.

## Project Overview
Personal academic webpage for Yifu Wu, built with Hugo and Hugo Blox Builder (academic-cv starter). Deployed via GitHub Actions to GitHub Pages.

## Tech Stack
- **Static site generator**: Hugo (v0.145.0)
- **Theme**: Hugo Blox Builder (`blox-tailwind` v0.3.1)
- **Deployment**: GitHub Actions -> GitHub Pages (`hugo --minify`, then a Pagefind search index)
- **URL**: https://nnonno.github.io/

## Key Directories
- `config/_default/` - Hugo configuration (hugo.yaml, params.yaml, menus.yaml, module.yaml, languages.yaml)
- `content/` - Site content (Markdown files)
- `content/authors/admin/_index.md` - Main bio/profile (role, organization, education, work history, skills, About Me)
- `content/_index.md` - Homepage sections (biography + "My Research")
- `content/experience.md` - Experience page (renders work, education, skills and languages from the admin profile)
- `assets/` - Theme assets (media, CSS overrides)
- `layouts/` - Template overrides
- `.github/workflows/publish.yaml` - CI/CD deployment workflow

## Build & Development
- Local dev: `hugo server` (requires Hugo v0.145.0 extended). Hugo is not currently installed on the dev machine, so there is no local build.
- Without a local build: check that edited front matter and config files still parse as YAML (for example with Python's `yaml.safe_load`), then check the GitHub Actions run after pushing.
- Production build handled by GitHub Actions on push to `main`. It does not pass `--buildDrafts`, so pages with `draft: true` are not published.
- Hugo version must stay in sync across: `hugoblox.yaml`, `.github/workflows/publish.yaml`, `netlify.toml`

## Content Sources
- CV data lives in `/Users/wuyifu/workspaces/personal/cv-resume/` (Awesome-CV LaTeX, built with `make`)
  - `cv_comprehensive/` - Full academic CV (summary, experience, education, publications, patents, projects, skills, honors, teaching)
  - `resume_*/` - Role-specific industry resumes
- The CV repo is the source of truth for dates, titles and publication venues. Update it first, then mirror the change here, applying the public-content rules below.

## Current Work Experience (on webpage)
1. **AWS Generative AI Innovation Center**, Applied Scientist (Apr 2026 – Present). Keep the description generic: agent infrastructure, prompt caching, model routing, LLM inference efficiency.
2. **Amazon Alexa**, Applied Scientist (Apr 2025 – Apr 2026; the transfer to AWS took effect 2026-04-06). Multilingual content-safety classifiers and guardrail models.
3. **University of Colorado Anschutz Medical Campus**, NLP Data Scientist (Aug 2024 – Mar 2025). Clinical NLP; LogosKG (ACL 2026); coauthor of a Findings of EMNLP 2025 paper.
4. Earlier roles: AI Newsletter Startup ML Engineer Intern (Jun – Aug 2024), Purdue RA (Dec 2019 – May 2024), Iowa State RA (Aug – Dec 2017), U of Akron RA (Aug 2015 – Jul 2019; the CV splits this into Aug 2015 – Aug 2017 and Jan 2018 – Jul 2019 around the Iowa State semester), Tsinghua IT Training School Instructor (Jan – Jun 2015), Haite Software Engineer (Sep 2011 – Dec 2012)

The experience page shows dates as "Month Year", so only the month of `date_start` / `date_end` is visible.

## Education (on webpage)
- Ph.D. in Computer and Information Technology, Purdue University (2019 – 2024)
- M.E. in VLSI Systems, University of Limerick (2013 – 2015)
- B.Eng. in Automation, Harbin Institute of Technology (2007 – 2011)
- Education is consolidated to these 3 entries. Iowa State and U of Akron are listed as work/RA positions, not separate degree entries.

## Public-content rules
- No customer names, internal metrics or numbers from internal work, internal project names, or unpublished / under-review papers. Describe the current AWS work only in the generic terms above.
- Do not state a years-of-experience count.
- State publication counts as peer-reviewed only (13 as of 2026-10-02; preprints are not counted).
- List only published papers, with the exact venue (for example "Findings of EMNLP 2025", not "EMNLP 2025").

## Hidden template placeholders
- The Hugo Blox example pages under `content/publication/`, `content/project/`, `content/post/`, `content/event/` and `content/teaching/`, plus `content/projects.md`, are set to `draft: true`.
- Do not un-draft them as they are. Replace the example content with real material first, then un-draft the section `_index.md` together with its pages (in recent Hugo versions a draft section `_index.md` can also hide the pages inside it).
- Never draft `content/authors/`. The biography and experience blocks load `/authors/admin`, and the build fails without it.

## Menu
- `config/_default/menus.yaml`: only Bio and Experience are active. Papers, Talks, News, Projects and Teaching are commented out. Re-enable an item only after its section has real content.

## Resume PDF
- No CV PDF is currently published. The "Download CV" button in `content/_index.md` is commented out.
- The old `static/uploads/resume.pdf` (a Feb 2026 `cv_comprehensive` build) was removed because it was out of date. Do not restore it as is; it remains in git history (commit `4f3a816`) for reference.
- To publish a CV again: build a corrected PDF from the CV repo, place it at `static/uploads/resume.pdf`, and uncomment the button.

## Important Notes
- `public/` and `resources/` are gitignored build artifacts - do NOT commit them
- `baseURL` in `config/_default/hugo.yaml` must match the GitHub Pages URL
- Hugo modules are managed via `go.mod` / `go.sum`
- Repo was renamed from `yifu_wu` to `nnonno.github.io` — remote and baseURL updated accordingly
