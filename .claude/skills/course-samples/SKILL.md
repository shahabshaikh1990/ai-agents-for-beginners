---
name: course-samples
description: Use when adding, editing or reviewing a lesson sample, notebook or README in this repo.
---

Outcome: the sample teaches one concept, matches its siblings, and a beginner can run it from the lesson README.

Facts
- Lessons are `<NN>-<name>/` with `README.md`, `images/`, and samples in `code_samples/` (lesson 14: `code-samples/`).
- Notebooks: `<NN>-<framework>.ipynb`, framework one of `semantic-kernel`, `autogen`, `python-agent-framework`, `azureaiagent`. Not every lesson has every variant.
- .NET samples are `<NN>-dotnet-agent-framework.md` plus a `.cs` single-file app, not notebooks.
- Free path: GitHub Models with `GITHUB_TOKEN`. Azure paths use the keys in `.env.example`. Notebooks are authored on Python 3.12; deps live in `requirements.txt`.

Good looks like
- README and sample agree, links resolve, every framework variant teaches the same concept.
- A new sample mirrors its nearest sibling and adds any new dependency to `requirements.txt`.
- Keep outputs that illustrate the lesson. Drop noise (tokens, local paths, stack traces).
