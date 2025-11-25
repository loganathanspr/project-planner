# Prompt: Generate EPIC_N.md using SSOT workflow

You are my planning assistant.  
Your job is to generate the refined EPIC_N.md file following my Single Source of Truth (SSOT) project structure.

---

## 1. Files you MUST read

Load and understand these files from the project root:

- docs/2-epics/EPICS.md
- docs/2-epics/EPIC_1.md
- docs/2-epics/EPIC_2.md

SSOT design documents under docs/1-architecture/ :

- docs/1-architecture/ARCHITECTURE.md
- docs/1-architecture/API_SPEC.md
- docs/1-architecture/DATA_MODEL.md
- docs/1-architecture/SYSTEM_OVERVIEW.md
- docs/1-architecture/NON_FUNCTIONAL.md

Other optional context:

- docs/0-vision/VISION.md
- docs/0-vision/FEATURES.md
- docs/6-history/ADRS/* (architecture decisions)

Determine:
- What EPIC_N corresponds to in EPICS.md
- Which subsystems it affects
- Which SSOT sections need stubs or updates

---

## 2. Update SSOT MINIMALLY before generating the epic

Before writing the EPIC_N.md file, create minimal stubs in:

- docs/1-architecture/ARCHITECTURE.md  
- docs/1-architecture/API_SPEC.md  
- docs/1-architecture/DATA_MODEL.md  

Only add:
- New section headers  
- 1–3 bullet summaries  
- Enough structure so EPIC_N issues can reference the correct section headings  

Examples of allowed stubs (DO NOT copy literally; generate relevant ones):

Example architecture stub:
## <Subsystem Name> (EPIC N)
- One-line purpose  
- Data flow summary  
- Dependencies  

Example API stub:
## API — <Module> (EPIC N)
- Endpoint names + their purposes  

Example data model stub:
## Model — <Entity> (EPIC N)
- Key conceptual fields  

DO NOT add detailed schemas or long explanations.  
DO NOT overplan.

Return these SSOT updates in a section titled:

### SSOT Updates

---

## 3. Generate EPIC_N.md using the exact required structure

Use this template:

# EPIC N — <Epic Name>
<!-- Status: not_started -->

## Linked Design Docs
- System Overview: ../1-architecture/SYSTEM_OVERVIEW.md
- Architecture: ../1-architecture/ARCHITECTURE.md
- Data Model: ../1-architecture/DATA_MODEL.md
- API Spec: ../1-architecture/API_SPEC.md
- Non-Functional: ../1-architecture/NON_FUNCTIONAL.md
- ADRs: ../6-history/ADRS/

## Design Scope (Epic-level DoR)
Authoritative Sections:
- ARCHITECTURE.md#<section>
- DATA_MODEL.md#<section>
- API_SPEC.md#<section>

Definition of Ready for all issues:
- SSOT impact identified  
- API contract reviewed (if API involved)  
- DB changes documented (if schema touched)  

## Goal
<1–3 sentences>

## In Scope
- <bullets>

## Out of Scope
- <bullets>

## Issues

### Issue EPN-01 — <title>
<!-- Status: not_started -->
Type: feature/chore/bug  
Priority: high/medium/low  

Description:  
<one paragraph>

Design Ties:
- ARCHITECTURE.md#<section>
- DATA_MODEL.md#<section>
- API_SPEC.md#<section>

Definition of Ready Check:
- [ ] SSOT impact identified  
- [ ] API contract reviewed  
- [ ] DB changes documented (if any)

Acceptance Criteria:
- [ ] Functional tests  
- [ ] Integration tests  
- [ ] QA checklist passed  
- [ ] Implementation matches design  
- [ ] SSOT updated (if required)

Notes:  
<implementation hints>

## SSOT Update Requirements (Epic-level verification)
At completion of this epic:
- Confirm all issue-level SSOT updates were made  
- Ensure no undocumented design changes exist  
- Create ADR if architecture changed significantly  

---

## 4. Required Output Format

Your final response must contain exactly two sections:

### SSOT Updates
<updated stubs for ARCHITECTURE.md, API_SPEC.md, DATA_MODEL.md>

### EPIC_N.md
<the fully generated epic>

Nothing else.

---

## 5. Rules

- Do NOT overdefine anything.  
- Keep SSOT stubs very short.  
- Keep issues high-level but actionable.  
- Follow EPIC_1.md and EPIC_2.md conventions.  
- Use 4–8 issues maximum.  
- Use exact header names.  
- Do NOT invent future epics.  

---

## 6. Start

After reading all referenced files, generate:

1. "SSOT Updates"  
2. "EPIC_N.md"

Only these two sections.

