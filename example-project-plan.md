# Example Project Plan: Team Knowledge Base Launch

---

## Epic: Team Knowledge Base Launch

| Field                     | Value                                                                |
| ------------------------- | -------------------------------------------------------------------- |
| Goal                      | Launch a centralized knowledge base for all team documentation.      |
| Why                       | Reduce onboarding time and prevent knowledge loss as the team grows. |
| Boundaries (Out of Scope) | Personal notes, external vendor docs, non-English content.           |
| Deliverables              | MVP-01.1 Knowledge Base MVP, onboarding guide, demo video.           |
| Definition of Done (DoD)  | MVP accepted, onboarding guide published, demo delivered.            |
| Dependencies              | SSO integration epic, design system update.                          |
| Labels                    | epic, docs, web-app                                                  |

---

## MVP: Knowledge Base MVP

| Field              | Value                                                                |
| ------------------ | -------------------------------------------------------------------- |
| Linked Epic        | EP-01 Team Knowledge Base Launch                                     |
| Goal               | Deliver a searchable, taggable knowledge base with markdown support. |
| Features Covered   | Search, tagging, markdown editor, permissions, onboarding flow.      |
| Boundaries         | No export to PDF, no mobile app, no external API integration.        |
| Definition of Done | Users can create, search, and tag docs; onboarding flow complete.    |
| Time Horizon       | 2 weeks                                                              |
| Acceptance Tests   | Docs can be created, searched, tagged; onboarding flow works.        |
| Labels             | mvp, docs, v0.1                                                      |

---

### Issues

| Title                      | Type    | Goal                                       | Steps                                                                         | Acceptance Criteria                              | Dependencies         | Labels            | Estimate |
| -------------------------- | ------- | ------------------------------------------ | ----------------------------------------------------------------------------- | ------------------------------------------------ | -------------------- | ----------------- | -------- |
| Build knowledge base shell | feature | Scaffold main UI and navigation            | 1. Implement layout<br>2. Add navigation<br>3. Set up permissions             | UI loads, navigation works, permissions enforced | Design system update | frontend, feature | M        |
| Implement search & tagging | feature | Enable search and tagging of docs          | 1. Build search bar<br>2. Add tag system<br>3. Integrate with doc list        | Search returns results, tags filter docs         | Knowledge base shell | frontend, feature | M        |
| Add markdown editor        | feature | Allow users to write docs in markdown      | 1. Integrate markdown editor<br>2. Save docs<br>3. Preview mode               | Docs save and preview correctly                  | Knowledge base shell | frontend, feature | S        |
| Create onboarding flow     | feature | Guide new users through first doc creation | 1. Build onboarding modal<br>2. Add step-by-step guide<br>3. Track completion | Onboarding modal appears, guide completes        | Knowledge base shell | frontend, feature | S        |
| Write onboarding guide     | doc     | Document onboarding steps for new users    | 1. Draft guide<br>2. Review with team<br>3. Publish to knowledge base         | Guide published, reviewed by team                | Onboarding flow      | docs, high        | XS       |
| Record demo video          | doc     | Create a demo video for internal training  | 1. Script video<br>2. Record walkthrough<br>3. Share with team                | Video shared, feedback collected                 | Onboarding guide     | docs, medium      | XS       |

---

## Review & Next Steps

| Action                                       |
| -------------------------------------------- |
| Schedule team demo and feedback session      |
| Prepare change notes for future improvements |
| Plan mobile MVP as a separate epic           |
