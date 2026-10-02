# AGENTS.md

"AI Agents for Beginners": lessons `00-` to `15-`, each a README plus runnable samples for beginners.

**Outcome:** every change leaves the course accurate, runnable by a beginner, and consistent with neighbouring lessons.

**Hard boundaries**
- Never edit `translations/` or `translated_images/`. CI regenerates them from the English root files on push to `main`.
- Never commit `.env`, `venv/`, `__pycache__/` or `*-backup.ipynb`. Never print or hard-code secrets.
- Never say a sample works unless you ran it. Samples need live model credentials you usually lack, so state what you did check (JSON validity, syntax, imports) and what you couldn't.

Sample conventions: `course-samples` skill. Setup: `00-course-setup/README.md`. PR titles start with `[Lesson-XX]`, `[Fix]`, `[Update]` or `[Docs]`.
