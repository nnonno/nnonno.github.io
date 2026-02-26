# CLAUDE.md

## Project Overview
Personal academic webpage for Yifu Wu, built with Hugo and Hugo Blox Builder (academic-cv starter). Deployed via GitHub Actions to GitHub Pages.

## Tech Stack
- **Static site generator**: Hugo (v0.145.0)
- **Theme**: Hugo Blox Builder (`blox-tailwind` v0.3.1)
- **Deployment**: GitHub Actions -> GitHub Pages
- **URL**: https://nnonno.github.io/yifu_wu/

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

## Important Notes
- `public/` and `resources/` are gitignored build artifacts - do NOT commit them
- `baseURL` in `config/_default/hugo.yaml` must match the GitHub Pages URL
- Hugo modules are managed via `go.mod` / `go.sum`
