# 🌱 Project Plan — LinguaNotes

_A sample project using Vision → Epics → Issues format_

---

## 🌟 Vision

### 🎯 Purpose

LinguaNotes is a lightweight web app where users create short bilingual notes for daily learning.  
Each note automatically generates a translation, pronunciation, and key grammar hints.

### 💎 Value

- Users can capture real-life phrases and instantly see translations.
- Encourages micro-learning through quick, meaningful notes.
- Makes language practice more natural and contextual.

### 🧩 Scope

**In Scope:**

- AI translation + explanation module
- Simple note-taking interface (web)
- Data storage (local or cloud)
- Pronunciation audio generation

**Out of Scope:**

- Full social features or chat
- Gamification (points, levels)
- Mobile native app (for later MVP)

### 🚀 Outcomes

- MVP: Create bilingual notes (text + translation + audio) through a minimal web UI.
- Output stored locally or in lightweight cloud backend.

### ⚙️ Technology Preferences

- Next.js + TypeScript frontend
- FastAPI backend
- OpenAI or compatible model for translation and explanations
- SQLite / Supabase for storage

---

## 🧩 Epics

---

### 🧩 Epic 1: AI Translation and Explanation Engine

**Goal:**  
Build an API module that takes input text and returns translation, pronunciation, and grammar explanation.

**Labels:**  
`mvp-1`, `ai`, `backend`

#### 🎯 Description

This epic provides the core AI engine of the app — a service that transforms a user’s note into a bilingual learning snippet.

#### ✅ Definition of Done (DoD)

- [ ] Translation endpoint working
- [ ] Grammar and pronunciation included in response
- [ ] Output follows structured JSON format

#### 🧩 Issues

- [ ] `#1` Define API schema for translation response
- [ ] `#2` Implement translation function using OpenAI API
- [ ] `#3` Add pronunciation + grammar explanation logic
- [ ] `#4` Write unit tests for translation module

#### ⏱️ Estimation

~1 week

---

### 🧩 Epic 2: Note Creation UI

**Goal:**  
Design a simple, modern interface to create and view bilingual notes.

**Labels:**  
`mvp-1`, `frontend`, `ui`

#### 🎯 Description

Develop a minimal web interface where users can type a note, view its translation instantly, and save it for future reference.

#### ✅ Definition of Done (DoD)

- [ ] UI allows text entry and displays AI results
- [ ] Notes can be saved locally or via API
- [ ] Responsive layout works on desktop + mobile

#### 🧩 Issues

- [ ] `#5` Create note input component
- [ ] `#6` Display translation + explanation in card format
- [ ] `#7` Add “Save Note” button (local storage)
- [ ] `#8` Add minimal Tailwind styling and layout

#### ⏱️ Estimation

~1 week

---

### 🧩 Epic 3: Data Storage and Retrieval

**Goal:**  
Persist user notes and enable browsing, searching, and deleting.

**Labels:**  
`mvp-2`, `backend`, `infra`

#### 🎯 Description

Implement lightweight data layer for storing bilingual notes with metadata (date, language, tags).

#### ✅ Definition of Done (DoD)

- [ ] Database schema defined and implemented
- [ ] CRUD API endpoints working
- [ ] Search/filter by language or keyword

#### 🧩 Issues

- [ ] `#9` Define database schema for notes
- [ ] `#10` Create CRUD endpoints in FastAPI
- [ ] `#11` Integrate with frontend note list
- [ ] `#12` Add search and delete functionality

#### ⏱️ Estimation

~1–1.5 weeks

---

### 🧩 Epic 4: Audio Pronunciation Generator

**Goal:**  
Add pronunciation playback for each bilingual note using text-to-speech.

**Labels:**  
`mvp-2`, `ai`, `media`

#### 🎯 Description

Use a TTS engine (OpenAI TTS or local alternative) to generate short audio clips for each note’s text and translation.

#### ✅ Definition of Done (DoD)

- [ ] Audio generated on note creation
- [ ] Playback available in UI
- [ ] Audio files cached efficiently

#### 🧩 Issues

- [ ] `#13` Integrate TTS API
- [ ] `#14` Add playback button to note card
- [ ] `#15` Cache audio locally for reuse
- [ ] `#16` Test performance with 10+ notes

#### ⏱️ Estimation

~1 week

---

### 🧩 Epic 5: MVP Integration and Testing

**Goal:**  
Combine all modules into a working MVP with basic CI/CD.

**Labels:**  
`mvp-final`, `integration`, `infra`

#### 🎯 Description

Connect frontend, backend, and AI services into one functioning deployment with automated build pipeline.

#### ✅ Definition of Done (DoD)

- [ ] MVP deployed on Vercel or Fly.io
- [ ] Backend API hosted and connected
- [ ] CI/CD workflow tested
- [ ] Basic smoke test passed

#### 🧩 Issues

- [ ] `#17` Set up Vercel deployment (frontend)
- [ ] `#18` Deploy backend API (Fly.io / Render)
- [ ] `#19` Connect env vars (API keys, DB URL)
- [ ] `#20` Write end-to-end test for MVP flow

#### ⏱️ Estimation

~1–2 weeks

---

## 🧠 Summary of Plan

| Epic | Focus                        | Est. Duration | MVP Label |
| ---- | ---------------------------- | ------------- | --------- |
| 1    | AI Translation + Explanation | 1 week        | mvp-1     |
| 2    | Note Creation UI             | 1 week        | mvp-1     |
| 3    | Storage & Retrieval          | 1.5 weeks     | mvp-2     |
| 4    | Audio Pronunciation          | 1 week        | mvp-2     |
| 5    | MVP Integration & Testing    | 1–2 weeks     | mvp-final |

---

## 🔍 Notes

- Avoid expanding existing epics; add new epics for new ideas.
- All issues estimated to be ≤1 day tasks.
- Labels group issues by MVP phases.
- Vision can evolve, but epics should stay atomic and deliverable.
