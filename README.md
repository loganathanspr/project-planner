# Project Planner

A minimal, anti-fragility Markdown system to go from Vision → Epics → Issues with clear, verifiable outcomes.

## What's inside

- `BEST-PRACTICES.md` — Principles and checklists for resilient planning.
- `PLANNER-PROMPT.md` — AI prompt to convert a free-style vision into Epics and Issues.
- `templates/` — Ready-to-use templates:
  - `VISION-TEMPLATE.md`
  - `EPIC-TEMPLATE.md`
  - `ISSUE-TEMPLATE.md`
- `examples/` — Sample plans, e.g. `LinguaNotes-PLAN.md`.

## Quickstart

1. Draft your Vision

- Copy `templates/VISION-TEMPLATE.md` and write a short free-style vision (5–10 lines: Purpose, Value, Scope, Outcomes, Constraints).

2. Generate Epics and Issues with AI

- Open `PLANNER-PROMPT.md` and paste your vision.
- Ask your AI to produce Epics (1–2 weeks each, clear DoD) and Issues (<1 day each, atomic, action-oriented).

3. Sequence for fast value

- Order epics by value and complexity: ship low-hanging fruit first and defer extremely complex epics.
- Note any dependencies that influence the order and keep epics self-contained where possible.

4. Capture Epics

- Use `templates/EPIC-TEMPLATE.md` per epic. Ensure a clear Definition of Done (DoD), short description, and rough duration (~1–2 weeks).

5. Break down into Issues

- Use `templates/ISSUE-TEMPLATE.md` for small, verifiable tasks (<1 day). Include DoD, dependencies, and labels.

6. Label instead of layers

- Use labels like `mvp-1`, `mvp-2` to indicate phases rather than creating new plan layers.

## Key principles (read this before you plan)

See `BEST-PRACTICES.md` for full details. Highlights:

- Clear outcomes with a Definition of Done at every level.
- Short-lived epics (1–2 weeks) and atomic issues (<1 day).
- Self-contained epics; avoid epic bloat and endless scope.
- Sequence by value/complexity — deliver demonstrable value early by shipping quick wins first.
- Use labels (e.g., `mvp-1`) instead of extra structural layers.

## Example

Check `examples/LinguaNotes-PLAN.md` for a concrete plan showing vision → epics → issues.

## Why this approach

It keeps plans lightweight, adaptable, and verifiable. By sequencing low-complexity, high-value epics first, you get early demos, reduce risk, and gather feedback sooner.
