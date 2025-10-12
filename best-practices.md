# 🧭 Project Planner — Best Practices

## General Principles

- Start broad → slice into small, testable units.
- Each Epic/MVP/Issue must deliver _observable progress_ or _learning_.
- Freeze structures after creation; add new scope as new entities.
- Prefer clarity and completion over volume and ambition.

---

## EPIC — Best Practices

| Area            | Best Practice                                       |
| --------------- | --------------------------------------------------- |
| 🎯 Scope        | One clear problem or capability area per Epic.      |
| 🧱 Size         | Completable in 2–4 weeks. Split if larger.          |
| 🧭 Purpose      | Express a clear _outcome_, not just “work to do”.   |
| 🧩 Structure    | 1–3 MVPs max per Epic.                              |
| ⚙️ Boundaries   | Always define _Out of Scope_ to prevent epic bloat. |
| 🚫 Anti-pattern | “Bucket Epics” that never finish — avoid.           |
| 🔒 Freeze Rule  | Once MVPs are defined, Epic is frozen.              |

---

## MVP — Best Practices

| Area            | Best Practice                                  |
| --------------- | ---------------------------------------------- |
| 🧪 Purpose      | Validate or deliver a minimal working slice.   |
| 🕒 Size         | Deliverable in 1–2 weeks.                      |
| 🎯 Focus        | One learning goal or value delivery per MVP.   |
| ⚙️ Boundaries   | Define what’s not covered — keeps focus sharp. |
| 🧩 Structure    | 5–15 small Issues per MVP.                     |
| 💡 Clarity      | Must have measurable outcome.                  |
| 🚫 Anti-pattern | Vague “improvements” or open-ended goals.      |

---

## ISSUE — Best Practices

| Area            | Best Practice                                     |
| --------------- | ------------------------------------------------- |
| 🎯 Clarity      | One concrete goal; measurable output.             |
| 📦 Atomicity    | Completable in ≤1–2 days.                         |
| 🧩 Dependencies | Define blocked-by/depends-on relationships.       |
| 🔁 Consistency  | Use consistent naming and link hierarchy.         |
| 🪄 Automation   | Auto-close issues via PRs.                        |
| 🚫 Anti-pattern | Placeholder issues without measurable completion. |

---

## Hierarchy

| Level | Scope                   | Duration  | Output                  | Links           |
| ----- | ----------------------- | --------- | ----------------------- | --------------- |
| Epic  | Capability/problem area | 2–4 weeks | 1–3 MVPs                | Links to MVPs   |
| MVP   | Testable slice/release  | 1–2 weeks | Demo or working feature | Links to Issues |
| Issue | Atomic task             | ≤1–2 days | Commit/PR               | Linked to MVP   |

---

## Naming Convention

| Type  | Example                    | Description                |
| ----- | -------------------------- | -------------------------- |
| Epic  | `EP-01-StoryGen`           | Sequential ID + short name |
| MVP   | `MVP-01.1-StoryGen-v0.1`   | Linked to Epic ID          |
| Issue | `ISS-01.1.3-PromptBuilder` | Linked to MVP ID           |

---

# 🧱 Stability & Anti-Fragility Guidelines

Planning systems break down when epics grow unchecked or are rewritten mid-execution.  
These rules keep your roadmap light, modular, and durable.

## 1️⃣ Anti-Fragility Principles

| Problem                                                            | Prevention Rule                                                                                                                               |
| ------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- |
| 🌀 **Planning Fragility** (constant re-scoping, plans invalidated) | Plan in layers: _Epic → MVP → Issue_. Only the lowest layer (issues) changes frequently. MVP/Epic layers stay frozen once defined.            |
| 🌋 **Epic Bloat** (epic keeps absorbing new ideas)                 | Every epic has a _strict scope statement_ and _Boundaries (Out of Scope)_. If a new idea doesn’t fit → make a new epic. Never “expand scope.” |
| 🌫️ **Over-general Epics** (“Improve app”, “Backend work”)          | Each epic must have a _clear measurable outcome_ and _specific capability area_. If it can’t be validated, it’s too broad.                    |
| 🧩 **Inter-Epic Coupling**                                         | Avoid tight dependencies. MVPs should be independently demonstrable. Split by capability, not sequence of tasks.                              |
| 🔁 **Scope Drift During Execution**                                | Lock epics & MVPs once issues begin. Add changes only through _Change Notes_ or _New Epic Proposals_.                                         |
| ⚖️ **Over-Planning**                                               | Limit planning horizon: max 2–3 upcoming MVPs per epic. Review every 4–6 weeks.                                                               |
| 💥 **Unclear Priority**                                            | Rank epics/MVPs by value or risk reduction — not by effort or “coolness.”                                                                     |
| 🧱 **Plan Fatigue**                                                | Keep docs lightweight (≤1 page per epic). Focus on clarity, not verbosity.                                                                    |

---

## 2️⃣ “Freeze & Fork” Rule

When new scope appears:

1. **Do not edit** existing epic text.
2. Create a new epic titled:  
   `EP-XX-[Name] (Forked from EP-YY-[Name])`
3. Link them under “Related Epics”.  
   → Keeps history intact and avoids chain edits that break traceability.

---

## 3️⃣ Periodic Review

- Every 2 weeks: review _open MVPs_ → prune unused issues.
- Every month: review _epic portfolio_ → close or split long-running ones.
- Every quarter: archive finished epics and start a clean planning cycle.

---

## 4️⃣ Validation Checklist (for any new Epic)

Before accepting an epic, confirm:

- [ ] Clear, single outcome
- [ ] Deliverable within ≤ 4 weeks
- [ ] Not overlapping existing epics
- [ ] Has explicit “Boundaries (Out of Scope)”
- [ ] Can be validated by 1–3 MVPs  
      If any fail → rewrite or split.
