# Workflow Specification: write-portfolio

**Module:** bd
**Status:** Placeholder — To be created via create-workflow workflow
**Created:** 2026-03-01

---

## Workflow Overview

**Goal:** Write a polished portfolio case study with image suggestions, ready to publish on Upwork, LinkedIn, or ad platforms.

**Description:** User briefs BDO on a completed project. BDO structures a professional case study, writes the copy, and produces a specific image brief (not vague advice — actual suggestions for screenshots, workflow diagrams, before/after results, or ad creatives). Output is a ready-to-publish portfolio piece paired with a clear visual brief.

**Workflow Type:** Feature — specialized output workflow

---

## Workflow Structure

### Entry Point

```yaml
---
name: write-portfolio
description: Write a polished portfolio case study and image suggestions
web_bundle: true
installed_path: '{project-root}/_bmad/bd/workflows/write-portfolio'
---
```

### Mode

- [x] Create-only (steps-c/)
- [ ] Tri-modal (steps-c/, steps-e/, steps-v/)

---

## Planned Steps

| Step | Name | Goal |
|------|------|------|
| 01 | Gather Project Info | Collect: client type, what was built, outcome, measurable results |
| 02 | Choose Platform | Select target platform (Upwork / LinkedIn / Ad creative / General) |
| 03 | Structure Case Study | Organise into: Problem → Approach → Solution → Results |
| 04 | Write Copy | Professional, achievement-focused prose tailored to the platform |
| 05 | Generate Image Brief | Suggest specific images: screenshots, diagrams, before/after, ad creatives |
| 06 | Deliver | Output the portfolio piece + image brief together |

---

## Workflow Inputs

### Required Inputs

- Project description (client type, what was built, key deliverables)
- Outcomes and results (quantified if possible — e.g., "30% increase in CTR")

### Optional Inputs

- Target platform (defaults to Upwork if not specified)
- Tone preference (e.g., "more technical", "results-focused", "storytelling style")
- Existing images available (so BDO can refine suggestions to what's achievable)

---

## Workflow Outputs

### Output Format

- [x] Document-producing
- [ ] Non-document

### Output Files

- Portfolio case study (structured prose, platform-appropriate length and tone)
- Image brief (specific suggestions for visuals to pair with the piece)

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
- Workflow name: write-portfolio
- Step structure: 6 steps (gather → platform → structure → write → images → deliver)
- Key differentiator: image suggestions must be specific (not "add a screenshot" but "screenshot of the checkout flow showing the custom Shopify fields you built")
- Platform awareness: Upwork portfolio format differs from LinkedIn articles or ad creatives — step 02 matters
- Sidecar option: after creating a portfolio piece, offer to store the project in the sidecar for future proposal use

---

_Spec created on 2026-03-01 via BMAD Module workflow_
