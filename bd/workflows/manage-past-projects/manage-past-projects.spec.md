# Workflow Specification: manage-past-projects

**Module:** bd
**Status:** Placeholder — To be created via create-workflow workflow
**Created:** 2026-03-01

---

## Workflow Overview

**Goal:** Maintain BDO's past project knowledge base — the memory that powers every personalised proposal.

**Description:** Allows the user to add new past projects, view existing entries, update project details, or remove outdated ones. Each entry is stored in BDO's sidecar so future proposals can reference real, specific work history. Well-structured entries = better proposals.

**Workflow Type:** Core — powers the write-proposal workflow's personalisation

---

## Workflow Structure

### Entry Point

```yaml
---
name: manage-past-projects
description: Add, view, or update past project references in BDO's knowledge base
web_bundle: true
installed_path: '{project-root}/_bmad/bd/workflows/manage-past-projects'
---
```

### Mode

- [ ] Create-only (steps-c/)
- [x] Tri-modal (steps-c/, steps-e/, steps-v/) — supports Add, Edit, and View operations

---

## Planned Steps

| Step | Name | Goal |
|------|------|------|
| 01 | Show Action Menu | Present options: Add / View All / Update / Remove |
| 02 | Execute Action | Route to the appropriate sub-flow based on user choice |
| 03 | Collect Project Details | Gather: client type, what was built, outcome, results, skills demonstrated |
| 04 | Save to Sidecar | Write structured entry to BDO's sidecar |
| 05 | Confirm | Report success and show the stored entry |

---

## Workflow Inputs

### Required Inputs

- Action selection (Add / View / Update / Remove)
- For Add/Update: project details (client type, deliverable, outcome, results, relevant skills)

### Optional Inputs

- Project name or label (for easy reference in future)
- Tags (e.g., "Shopify", "email marketing", "landing page") for matching to jobs

---

## Workflow Outputs

### Output Format

- [ ] Document-producing
- [x] Non-document

### Output Files

- Updated BDO sidecar (past projects knowledge base)
- Confirmation summary of the stored/updated/removed entry

---

## Agent Integration

### Primary Agent

BDO (Business Development Officer) — owns and maintains the sidecar

### Other Agents

None (single-agent module)

---

## Implementation Notes

**Use the create-workflow workflow to build this workflow.**

Inputs needed:
- Workflow name: manage-past-projects
- Mode: Tri-modal (add = create, update = edit, view = validate/read)
- Sidecar structure: define a consistent schema for past project entries (client_type, deliverable, outcome, results, skills, tags)
- Key UX: viewing entries should be clean and scannable; adding should feel quick, not like filling out a form

---

_Spec created on 2026-03-01 via BMAD Module workflow_
