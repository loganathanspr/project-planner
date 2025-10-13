# 🧭 Best Practices for AI Project Planning

_A minimal, anti-fragility approach from Vision → Epics → Issues._

---

## 🪶 Philosophy

- **Start simple:** Vision → Epics → Issues.
- **Prevent fragility:** Plans should evolve, not explode.
- **Avoid bloat:** Close epics; new ideas belong in new epics.
- **Plan by intent:** Describe outcomes, not technical details.
- **Stay verifiable:** Every Epic and Issue has a clear **Definition of Done (DoD)**.

---

## 🌱 Free-Style Vision Guidelines

A “free-style vision” is an open narrative that defines your project’s intent and direction.

Include:

1. **Purpose** — Why the project exists.
2. **Value** — What user or business value it creates.
3. **Scope** — What’s included and excluded.
4. **Outcomes** — What success looks like (e.g., working MVP, public release).
5. **Constraints / Preferences** — Tech stack, speed, or quality constraints.

Keep it short — 5–10 lines maximum.

---

## 🧱 Best Practices for Epics

| Principle                           | Description                                                                      |
| ----------------------------------- | -------------------------------------------------------------------------------- |
| 🎯 **Clear Outcome**                | Defines a functional or visible deliverable.                                     |
| 🕓 **Short-Lived**                  | Should be done within 1–2 weeks.                                                 |
| 🧩 **Self-Contained**               | Minimize dependencies between epics.                                             |
| ✅ **Definition of Done (DoD)**     | Observable and verifiable outcome.                                               |
| 🚫 **No Endless Scope**             | Once done → close; new ideas → new epic.                                         |
| 🏷️ **Use Labels for MVPs**          | Replace “MVP” layers with simple labels (`mvp-1`, `mvp-2`).                      |
| 🔢 **Sequence by Value/Complexity** | Prioritize quick wins first; defer complex epics until after demonstrable value. |

---

## 🔹 Best Practices for Issues

| Principle                   | Description                                                      |
| --------------------------- | ---------------------------------------------------------------- |
| ⚡ **Atomic**               | Achievable in <1 day.                                            |
| ✍️ **Action-Oriented**      | Use verbs (“Implement”, “Design”, “Fix”, “Write”).               |
| 🎯 **Goal-Focused**         | Express intent, not implementation.                              |
| ✅ **DoD-Driven**           | Measurable completion criteria required.                         |
| ⛓️ **Dependencies Visible** | Reference related issues or epics (`#12`).                       |
| 🧠 **AI-Friendly Context**  | Include short notes for Copilot/AI.                              |
| 🔀 **Respect Epic Order**   | Plan sprints using lower-complexity epics first, unless blocked. |

---

## 🧭 Anti-Fragility Principles

- Plan in **small, testable increments**.
- Never expand existing epics indefinitely.
- Let **new ideas become new epics**.
- Keep the **vision stable**, but let execution evolve.
- Always **define “done” before starting**.
- **Deliver quick wins first** — record reasons if order changes.
