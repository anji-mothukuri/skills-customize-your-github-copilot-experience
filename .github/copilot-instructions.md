# Copilot Coding Agent Onboarding Instructions

## High-Level Repository Overview

- **Purpose:** This repository is an educational portal for Mergington High School's Computer Science course. It provides web-based assignment management, Python starter code, and exercises for students to learn programming fundamentals, data analysis, and game development.
- **Project Type:** Mixed web and Python educational project.
- **Languages:** JavaScript (frontend logic), HTML/CSS (web UI), Python (assignment starter code), JSON (configuration).
- **Frameworks/Tools:** No backend framework; uses vanilla JS, HTML, CSS. Python scripts are standalone. No package manager or build system is required.
- **Repo Size:** Small to medium; <100 files, mostly educational content and scripts.

## Build, Run, and Validation Instructions

- **Web Portal:**
  - Open `index.html` in a browser to view the portal. No build step is required.
  - All assets are in `assets/` (JS, CSS, images).
  - Assignments are loaded from `config.json`.
  - Always ensure `config.json` is valid JSON after edits.
- **Python Assignments:**
  - Each assignment folder under `assignments/` contains a `starter-code.py` and a `README.md`.
  - Run Python scripts directly (e.g., `python starter-code.py`).
  - No dependencies except for `data-analysis`, which may require `pandas` and `matplotlib`. Install with `pip install pandas matplotlib` if needed.
  - Always validate code changes by running the script in the assignment directory.
- **Validation:**
  - No formal test or lint pipeline. Manual validation: run scripts and check for errors.
  - For web changes, reload the browser and check assignment rendering.
  - For Python, check for runtime errors and correct output.
- **GitHub Actions:**
  - `.github/workflows/` contains step-based YAML workflows for exercise validation. These check for file existence, directory creation, and config updates.
  - No CI build or test pipeline; workflows are for exercise progression and file checks.

## Project Layout and Key Files

- **Root Files:**
  - `index.html`: Main portal page.
  - `config.json`: Assignment/course configuration.
  - `README.md`: Course overview.
  - `LICENSE`: MIT license.
- **Assets:**
  - `assets/js/script.js`: Portal logic.
  - `assets/js/assignment.js`: Assignment detail logic.
  - `assets/css/styles.css`: Styles.
  - `assets/pages/assignment.html`: Assignment detail page.
- **Assignments:**
  - `assignments/`: Contains subfolders for each assignment.
    - Each has `starter-code.py` and `README.md`.
    - `data-analysis/` includes `data.csv`.
- **Templates:**
  - `templates/assignment-template.md`: Assignment markdown template.
- **GitHub Workflows:**
  - `.github/workflows/`: Step-based YAML files for exercise validation.

## Key Validation Steps

- After any change, always:
  - Validate `config.json` syntax.
  - Run Python scripts in assignment folders.
  - Reload web portal and check assignment display.
- For `data-analysis` assignment, install required Python packages before running.
- Trust these instructions unless you find errors or missing information. Only search for additional details if instructions are incomplete or do not work as described.

## Error Handling and Workarounds

- If web portal fails to load assignments, check for JSON syntax errors in `config.json`.
- If Python scripts fail, check for missing dependencies and install as needed.
- If assignment files are missing, check workflow logs for file existence checks.

## Summary of Root and Key Directory Contents

- **Root:** `index.html`, `config.json`, `README.md`, `LICENSE`
- **assets/js/**: `script.js`, `assignment.js`
- **assets/css/**: `styles.css`
- **assets/pages/**: `assignment.html`
- **assignments/**: `python-basics/`, `games-in-python/`, `python-classes/`, `data-analysis/` (each with `starter-code.py`, `README.md`)
- **templates/**: `assignment-template.md`
- **.github/workflows/**: `0-start-exercise.yml`, `1-step.yml`, `2-step.yml`, `3-step.yml`, `4-last-step.yml`

---

**Follow these instructions for efficient onboarding and task completion. Only perform additional searches if information here is incomplete or incorrect.**
