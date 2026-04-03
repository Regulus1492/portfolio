# Portfolio Improvement Plan

## 1. Project Goal
The goal of this project is to transform the current GitHub Pages site into a high-impact Upwork portfolio. We will focus on highlighting results-driven experience, technical expertise, and client-centric communication to attract and convert potential hires.

## 2. Context Files
- `_config.yml`: Jekyll configuration for the GitHub Pages site.
- `README.md`: Technical documentation for the repository (setup, tech stack, usage). (Pending to modify)
- `my_cv.txt`: Raw professional history used to enrich and update the portfolio.


## Step 1a: Professional Repository Alignment & Infrastructure

This phase focuses on aligning the repository with industry best practices for Software Development and Data Science. The goal is to separate the "Technical Manual" (for developers/recruiters) from the "Website Content" (for the end-user).

### Tasks:
- [x] **Environment Reproducibility**:
    - Run `pip freeze > requirements.txt` to capture the current environment state.
    - Ensure `.venv/` remains in `.gitignore` while `requirements.txt` is tracked.
- [x] **Documentation vs. Content Separation**:
    - **Migrate Content**: Move the professional bio, experience, and certifications from `README.md` to a new `index.md`.
    - **Add Front Matter**: Include a YAML block at the top of `index.md` for Jekyll (layout, title, etc.).
    - **Draft Technical README**: Rewrite `README.md` to include:
        - High-level project summary.
        - Setup instructions (`pip install -r requirements.txt`).
        - Tech stack overview (Python, Jekyll, GitHub Actions).
        - A clear "Live Link" to the portfolio.
- [x] **Asset Management**:
    - Create a structured directory: `assets/img/`.
    - Relocate root images (like `photoLinkedin.jpg`) into `assets/img/`.
    - Update `_config.yml` to reflect the new path for the `logo`.
- [x] **Architecture Validation**:
    - Confirm that GitHub Pages/Jekyll correctly picks up `index.md` as the home page and ignores the technical `README.md` for site generation.


## 3. The Full Step-by-Step Plan
- **Step 1: Audit the current page**
  - *Action*: Analyze structure, content, and design against the CV.
  - *Deliverable*: Audit report identifying gaps and improvement areas.
  - *Approval*: Required before Step 2.
- **Step 2: Apply fixes and enrich content**
  - *Action*: Fix structural issues and integrate recent achievements from `my_cv.txt`. Propose a CV sync system.
  - *Deliverable*: Updated `README.md` and a sync strategy.
  - *Approval*: Required before Step 3.
- **Step 3: Simplify the job experience section**
  - *Action*: Refactor roles to emphasize impact and results using client-friendly language.
  - *Deliverable*: Concise and persuasive Experience section.
  - *Approval*: Required before Step 4.
- **Step 4: Add a Projects section**
  - **4a: Write Project README**
    - *Action*: Draft a comprehensive README for a selected GitHub project.
    - *Deliverable*: Markdown file for the repository.
    - *Approval*: Required before 4b.
  - **4b: Create Project Card**
    - *Action*: Design a reusable project card template and add the project to the portfolio.
    - *Deliverable*: Portfolio project card.
    - *Approval*: Required before Step 5.
- **Step 5: Final review**
  - *Action*: Perform a hireability audit from a non-technical client's perspective.
  - *Deliverable*: Final checklist/feedback report.

## 4. Progress Tracker
- [x] Step 1 — Audit
- [x] Step 2 — Apply fixes
- [ ] Step 3 — Simplify experience
- [ ] Step 4a — Write README
- [ ] Step 4b — Project card
- [ ] Step 5 — Final review

## 5. Decisions & Notes Log

*   **Git Strategy**: Decided to exclude `my_cv.txt` and `prompts.txt` from the public GitHub repository using `.gitignore` to keep the repo focused only on the live site files and protect internal context. `PORTFOLIO_PLAN.md` is now tracked for project management.
*   **README vs. index.md Separation**: Moved all professional/website content from `README.md` into `index.md` (Jekyll homepage). `README.md` now serves as a technical guide for developers. GitHub Pages natively prioritizes `index.md` over `README.md` — no `_config.yml` changes required.

## 6. Reusable Templates Placeholder

*   **Project Card Template**: (TBD in Step 4b)
*   **Sync Convention**: Tag-Based Markdown Sync using `<!-- START:SECTION -->` markers and a Python injection script.


