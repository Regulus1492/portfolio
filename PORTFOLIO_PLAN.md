# Portfolio Improvement Plan

## 1. Project Goal
The goal of this project is to transform the current GitHub Pages site into a high-impact Upwork portfolio. We will focus on highlighting results-driven experience, technical expertise, and client-centric communication to attract and convert potential hires.

## 2. Context Files
- `_config.yml`: Jekyll configuration for the GitHub Pages site.
- `README.md`: The primary content and layout for the portfolio.
- `my_cv.txt`: Detailed professional history used to enrich and update the portfolio.

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

*   **Git Strategy**: Decided to exclude `my_cv.txt`, `prompts.txt`, and `PORTFOLIO_PLAN.md` from the public GitHub repository using `.gitignore` to keep the repo focused only on the live site files and protect internal context.

## 6. Reusable Templates Placeholder

*   **Project Card Template**: (TBD in Step 4b)
*   **Sync Convention**: Tag-Based Markdown Sync using `<!-- START:SECTION -->` markers and a Python injection script.


