# Workflow Specification: write-proposal

**Module:** bd
**Status:** Placeholder — To be created via create-workflow workflow
**Created:** 2026-03-01

---

## Workflow Overview

**Goal:** Write a tailored, ready-to-send Upwork proposal from a job posting in seconds.

**Description:** User pastes a job description. BDO reads it, identifies client needs and tone, pulls the most relevant past project from the sidecar, and applies the 3-line formula (What I Saw → How I'll Help → Next Step) to produce a clean ~90-word proposal. Ends with a quality check and confidence signal.

**Workflow Type:** Core — primary value delivery workflow

---

## Workflow Structure

### Entry Point

```yaml
---
name: write-proposal
description: Write a tailored Upwork proposal from a job posting
web_bundle: true
installed_path: '{project-root}/_bmad/bd/workflows/write-proposal'
---
```

### Mode

- [x] Create-only (steps-c/)
- [ ] Tri-modal (steps-c/, steps-e/, steps-v/)

---

## Planned Steps

| Step | Name | Goal |
|------|------|------|
| 01 | Gather Job Post | User pastes the job description; BDO confirms receipt |
| 02 | Parse & Analyse | Identify client needs, gaps, tone, budget signals |
| 03 | Select Past Project | Pull the most relevant past project from the sidecar |
| 04 | Write Proposal | Apply 3-line formula: What I Saw → How I'll Help → Next Step |
| 05 | Quality Check | Verify: under 120 words, no skill lists, ends with a question |
| 06 | Deliver | Output the proposal + confidence signal |

---

## Workflow Inputs

### Required Inputs

- Job description (pasted by user — full text of the Upwork posting)

### Optional Inputs

- Tone preference override (e.g., "go more formal" or "keep it casual")
- Specific past project to reference (if user wants to choose instead of BDO)

---

## Workflow Outputs

### Output Format

- [x] Document-producing
- [ ] Non-document

### Output Files

- Ready-to-send proposal (~90 words, 3-line formula structure)
- Confidence signal from BDO (e.g., *"This one's strong. Send it."*)
- Optional: note if assumptions were made due to a weak job post

---

## Agent Integration

### Primary Agent

BDO (Business Development Officer) — owns this workflow end-to-end

### Other Agents

None (single-agent module)

---

## Implementation Notes

**Use the create-workflow workflow to build this workflow.**

Inputs needed:
- Workflow name: write-proposal
- Step structure: 6 steps (gather → parse → select → write → check → deliver)
- Key logic: 3-line formula enforcement, sidecar lookup for past projects, quality checklist
- Sidecar integration: BDO reads past projects from sidecar to select the best match
- Quality rules: <120 words, no skill lists, ends with a question, human-sounding tone

---

_Spec created on 2026-03-01 via BMAD Module workflow_
