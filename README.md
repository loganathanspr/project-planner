# Project Planner

A minimal, anti-fragility Markdown system to go from **Vision → Epics → Issues** with clear, verifiable outcomes.

---

## 📦 What's Inside

- `BEST-PRACTICES.md` — Principles and checklists for resilient planning
- `PLANNER-PROMPT.md` — AI prompt to convert a free-style vision into structured Epics and Issues
- `templates/` — Ready-to-use templates:
  - `VISION-TEMPLATE.md`
  - `EPIC-TEMPLATE.md`
  - `ISSUE-TEMPLATE.md`
- `examples/` — Example plans such as `LinguaNotes-PLAN.md`

---

## 🚀 Quickstart

### 1. Draft Your Vision

Copy `templates/VISION-TEMPLATE.md` and write a short free-style vision (5–10 lines):

> Purpose, Value, Scope, Outcomes, and Constraints.

### 2. Generate Epics & Issues with AI

Open `PLANNER-PROMPT.md`, paste your vision, and ask your AI to produce:

- **Epics** (1–2 weeks each, clear DoD)
- **Issues** (<1 day each, atomic and action-oriented)

### 3. Sequence for Fast Value

- Order epics by **value and complexity** — ship low-hanging fruit first, defer the complex ones.
- Note dependencies that affect order, keeping each epic self-contained where possible.

### 4. Capture Epics

Use `templates/EPIC-TEMPLATE.md` for each epic.  
Ensure clear **Definition of Done (DoD)**, concise description, and ~1–2 week scope.

### 5. Break Down into Issues

Use `templates/ISSUE-TEMPLATE.md` for small, verifiable tasks (<1 day).  
Include DoD, dependencies, and labels.

### 6. Label Instead of Layers

Use simple labels like `mvp-1`, `mvp-2` to indicate phases instead of creating additional plan layers.

---

## 🧠 Key Principles

See `BEST-PRACTICES.md` for detailed guidance. Highlights:

- Every level must have a **clear Definition of Done**.
- Keep epics **short-lived** (1–2 weeks) and issues **atomic** (<1 day).
- Avoid epic bloat — create new epics for new ideas.
- **Sequence by value and complexity** to deliver demonstrable value early.
- Prefer **labels** over structural hierarchies.

---

## 🧩 Example

Check `examples/LinguaNotes-PLAN.md` for a real project plan showing Vision → Epics → Issues.

---

## 💡 Why This Approach Works

This framework keeps plans **lightweight, adaptable, and verifiable**.  
By shipping quick wins first, you build momentum, gather feedback early, and minimize planning fragility.
