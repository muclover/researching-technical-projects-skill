# Researching Technical Projects Skill

This repository stores a reusable Codex skill for technical project research reports, plus the cuda-oxide research report produced with that skill.

## Structure

```text
skills/
  researching-technical-projects/
    SKILL.md

.agent/
  skills/
    researching-technical-projects -> ../../skills/researching-technical-projects

reports/
  cuda-oxide-research-report.md
```

## Skill Usage

`skills/researching-technical-projects/SKILL.md` is the source copy of the skill.

`.agent/skills/researching-technical-projects` is a relative symlink to the source skill directory. This keeps the project-local agent skill path usable without duplicating files. Edit the skill under `skills/`; the `.agent/skills/` path will see the same content automatically.

Use this skill when asking for a research report, feasibility study, architecture investigation, industry value analysis, competitive technology comparison, or due diligence on a technical project or technology.

## Report

The cuda-oxide research report is stored at:

```text
reports/cuda-oxide-research-report.md
```

The report covers CUDA programming context, Rust's value in GPU programming, cuda-oxide architecture and core implementation, technical feasibility, competitor comparison, Rust language ecosystem implications, NPU/accelerator ecosystem opportunities, and decision recommendations.
