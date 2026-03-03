# Workflows Reference

The BD module includes 3 workflows:

---

## write-proposal

**Type:** Core workflow
**Agent:** BDO
**Trigger:** `[WP]` from BDO's menu

**Purpose:**
Write a tailored, ready-to-send Upwork proposal from a job posting. Applies the 3-line formula (What I Saw → How I'll Help → Next Step) grounded in real past project references.

**When to Use:**
You've found a job posting worth bidding on and want a personalised, human-sounding proposal in seconds.

**Key Steps:**
1. Paste the job description
2. BDO parses the job and identifies client needs, tone, and gaps
3. BDO selects the most relevant past project from the sidecar
4. BDO applies the 3-line formula
5. Quality check: under 120 words, no skill lists, ends with a question
6. Delivers the proposal + confidence signal

**Output:** ~90-word proposal ready to copy-paste + BDO's confidence signal

---

## manage-past-projects

**Type:** Core workflow (powers write-proposal personalisation)
**Agent:** BDO
**Trigger:** `[PP]` from BDO's menu

**Purpose:**
Maintain BDO's past project knowledge base — the memory that makes every proposal specific and personal rather than generic.

**When to Use:**
- After finishing a project (add it so BDO can reference it)
- Before a big bidding session (review what BDO knows)
- When a past project entry needs updating

**Key Operations:**
- **Add** — Enter project details (client type, deliverable, outcome, results, skills)
- **View** — Browse all stored past projects
- **Update** — Edit an existing entry
- **Remove** — Delete an outdated entry

**Output:** Updated sidecar knowledge base (non-document — data persisted for future proposals)

---

## write-portfolio

**Type:** Feature workflow
**Agent:** BDO
**Trigger:** `[PF]` from BDO's menu

**Purpose:**
Write a polished, professional portfolio case study with a specific image brief. Ready to publish on Upwork, LinkedIn, or use in ad creatives.

**When to Use:**
You've completed a significant project and want to showcase it professionally — without spending hours writing it yourself.

**Key Steps:**
1. Brief BDO on the project (client type, what was built, outcome, results)
2. Select target platform (Upwork / LinkedIn / Ad creative / General)
3. BDO structures the case study: Problem → Approach → Solution → Results
4. BDO writes professional, achievement-focused copy for the platform
5. BDO generates specific image suggestions (not vague — actual descriptions of what to capture)
6. Delivers the portfolio piece + image brief together

**Output:** Ready-to-publish case study + specific image brief

---
