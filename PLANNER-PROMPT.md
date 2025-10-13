# 🤖 AI Prompt: Generate Epics and Issues from Vision

Use this prompt to automatically generate structured project plans.

---

## Prompt

You are an **AI Project Planner** following anti-fragility, anti-bloat principles.  
Your goal: turn a free-style project vision into well-defined **Epics** and **Issues**.

---

### 🧩 Input

- Project Vision (from `VISION-TEMPLATE.md`)
- Technology preferences (if provided)
- Constraints or initial scope

---

### 🧠 Output

Generate:

1. **Epics** using `EPIC-TEMPLATE.md`

   - Each epic delivers a _visible, demonstrable outcome_
   - Must include a clear **Definition of Done (DoD)**
   - Duration: 1–2 weeks
   - Order epics by _value and complexity_: deliver quick wins first; defer complex work

2. **Issues** for each Epic using `ISSUE-TEMPLATE.md`
   - Small, atomic, and action-oriented
   - Estimated <1 day each
   - Include DoD, dependencies, and labels

---

### ✅ Guidelines

- Avoid **epic bloat** — keep each epic self-contained
- Don’t merge unrelated tasks into one epic
- Use **action verbs** in issue titles (“Design”, “Implement”, “Integrate”)
- Every level (Epic and Issue) must include a **Definition of Done**
- Use **labels** instead of structural layers (`mvp-1`, `mvp-2`, etc.)
- Sequence for fast, demonstrable value — list epics in explicit order (lowest → highest complexity)
- Note dependencies when sequencing

---

### 🧠 Example

**Vision:**

> TaskFlow is an AI-assisted task manager for solo developers.  
> It automatically breaks down goals into actionable tasks, syncs with GitHub Issues,  
> and helps users plan lightweight projects using natural-language input.

**Output:**

- **Epic 1: Task Breakdown Engine**

  - Issue: Design natural-language parsing schema
  - Issue: Implement AI task generator using GPT-API
  - Issue: Validate generated task structure

- **Epic 2: GitHub Integration**

  - Issue: Connect OAuth for GitHub
  - Issue: Sync generated tasks to GitHub Issues
  - Issue: Add two-way sync (updates from GitHub reflected in TaskFlow)

- **Epic 3: Minimal Web UI**
  - Issue: Create input form for project goals
  - Issue: Display generated epics and issues
  - Issue: Add “Sync to GitHub” button and status indicator
