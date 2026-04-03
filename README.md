# Portfolio — Juan Carlos Serrano

Personal portfolio site hosted on GitHub Pages.

**Live site:** https://regulus1492.github.io/portfolio/

---

## Tech Stack

| Layer | Technology |
|---|---|
| Static site generator | Jekyll |
| Theme | jekyll-theme-minimal |
| Hosting | GitHub Pages |
| Content format | Markdown |

---

## Key Files

| File | Purpose |
|---|---|
| `index.md` | Website content (homepage rendered by GitHub Pages) |
| `_config.yml` | Jekyll site metadata: title, logo, description, theme |
| `assets/img/` | Static images (profile photo, etc.) |
| `PORTFOLIO_PLAN.md` | Strategic roadmap and progress tracker |
| `CLAUDE.md` | Guidance for Claude Code in this repository |
| `requirements.txt` | Python environment snapshot |

> `README.md` (this file) is **not** rendered as the homepage. GitHub Pages prioritizes `index.md` over `README.md`.

---

## Local Preview

Jekyll must be installed:

```bash
gem install jekyll bundler
```

Then serve locally:

```bash
jekyll serve
# Site available at http://localhost:4000
```

---

## Deployment

Pushing to `main` triggers an automatic GitHub Pages build. No CI configuration is required — GitHub Pages runs Jekyll natively.
