# 🧭 Best Practices for AI Project Planning

_A minimal, anti-fragility approach for Vision → Epics → Issues._

---

## 🪶 Philosophy

- **Start simple**: Free-style vision → Epics → Issues.
- **Prevent fragility**: Plans evolve, not explode. Small, self-contained units adapt easily.
- **Avoid bloat**: Epics and issues must close; new ideas go into new epics.
- **Plan by intent**: Describe outcomes, not technical details.
- **Stay verifiable**: Every Epic/Issue must have a clear “Definition of Done” (DoD).

---

## 🎯 Free-Style Vision Guidelines

A “free-style vision” is an open narrative describing your project’s intent and direction.

Include:

1. **Purpose** – Why the project exists.
2. **Value** – What user or business value it creates.
3. **Scope** – Rough boundaries (what’s in, what’s out).
4. **Outcomes** – What success looks like (e.g., working prototype, public release).
5. **Constraints / Preferences** – Technologies, speed, quality, etc.

Keep it short (5–10 lines max).

---

## 🧱 Best Practices for Epics

| Principle                       | Description                                                |
| ------------------------------- | ---------------------------------------------------------- |
| 🎯 **Clear Outcome**            | Defines a functional or visible deliverable.               |
| 🕓 **Short-Lived**              | Done within 1–2 weeks.                                     |
| 🧩 **Self-Contained**           | Independent from other epics as much as possible.          |
| ✅ **Definition of Done (DoD)** | Observable and verifiable outcome.                         |
| 🚫 **No Endless Scope**         | Once done → closed; new ideas → new epic.                  |
| 🏷️ **Use Labels for MVPs**      | Replace “MVP” layer with simple labels (`mvp-1`, `mvp-2`). |

---

## 🔹 Best Practices for Issues

| Principle                   | Description                                          |
| --------------------------- | ---------------------------------------------------- |
| ⚡ **Atomic**               | Achievable in <1 day or a few hours.                 |
| ✍️ **Action-Oriented**      | Use verbs (“Implement”, “Design”, “Fix”, “Write”).   |
| 🎯 **Goal-Focused**         | Express intent, not implementation.                  |
| ✅ **DoD-Driven**           | Each issue must have measurable completion criteria. |
| ⛓️ **Dependencies Visible** | Reference related issues (`#12`) or epics.           |
| 🧠 **AI-Friendly Context**  | Include short notes for Copilot/AI assistance.       |

---

## 🧭 Anti-Fragility Principles

- Plan in **small, testable increments**.
- Never expand existing epics indefinitely.
- Let **new ideas become new epics**.
- Keep the **vision stable**, allow **epics/issues to evolve**.
- Always **define done before starting**.
