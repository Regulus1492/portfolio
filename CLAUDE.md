# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A GitHub Pages portfolio site built with Jekyll, targeting Upwork clients and technical recruiters. The goal is a high-impact, results-driven professional profile for an Economist/Data Scientist.

## Local Development

No Gemfile is present — GitHub Pages builds Jekyll automatically on push. To preview locally, install Jekyll manually:

```bash
gem install jekyll bundler
jekyll serve   # serves at http://localhost:4000
jekyll build   # outputs to _site/
```

There are no automated tests. Validate changes by running `jekyll serve` and checking the rendered site in a browser before pushing.

## Architecture

- **`_config.yml`**: Jekyll site metadata (title, logo path, theme). Uses `jekyll-theme-minimal`.
- **`index.md`**: Website homepage content (rendered by GitHub Pages). Contains the full professional profile (bio, experience, certifications, etc.). Jekyll prioritizes `index.md` over `README.md`.
- **`README.md`**: Technical guide for developers (stack, setup, file map). Not rendered as the live site homepage.
- **`PORTFOLIO_PLAN.md`**: Strategic roadmap — read this before making any content changes to understand intended direction and what's already been decided.
- **`my_cv.txt`**: Gitignored source-of-truth for the full professional history. Use this to cross-reference and enrich content in `index.md`. It contains more detail and exact dates than the live site.
- **`assets/img/`**: Profile photo and other static images.

## Content Sync Convention

When content is later split into sections, the planned convention is **tag-based Markdown sync** using `<!-- START:SECTION_NAME -->` / `<!-- END:SECTION_NAME -->` markers with a Python injection script. Don't introduce ad-hoc sync patterns — keep this convention in mind.

## Active Roadmap (PORTFOLIO_PLAN.md)

Steps 1, 2, and 1a (infrastructure) are complete. **Next step: Step 3.**

- **Step 3** ← resume here: Refactor the Experience section in `index.md` — concise, impact-first, client-friendly language. Cross-reference `my_cv.txt` for detail.
- **Step 4a**: Draft a project README for a selected GitHub project.
- **Step 4b**: Design a reusable project card template and add it to the portfolio.
- **Step 5**: Hireability audit from a non-technical client's perspective.

Each step requires user approval before proceeding to the next.
