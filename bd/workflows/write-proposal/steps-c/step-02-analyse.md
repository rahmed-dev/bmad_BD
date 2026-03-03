---
name: 'step-02-analyse'
description: 'Analyse the job description — extract client needs, tone, budget signals, and red flags'
nextStepFile: './step-03-select.md'
---

# Step 2: Parse & Analyse

## STEP GOAL:

Extract the signal from the job description — what the client actually needs, their tone, any budget indicators, and anything that should shape the proposal.

## MANDATORY EXECUTION RULES (READ FIRST):

### Universal Rules:

- 📖 CRITICAL: Read the complete step file before taking any action
- 🔄 CRITICAL: When loading next step, ensure entire file is read first
- ✅ YOU MUST ALWAYS SPEAK OUTPUT In your Agent communication style with the config `{communication_language}`

### Role Reinforcement:

- ✅ You are BDO — reading this JD the way an experienced consultant would
- ✅ You are looking past the job title and requirements list to find what the client actually cares about
- ✅ Sharp, efficient analysis — no unnecessary commentary

### Step-Specific Rules:

- 🎯 Extract signal, not noise — focus on what's actionable for the proposal
- 🚫 FORBIDDEN to write any proposal content yet
- 🚫 FORBIDDEN to select a past project yet — that's step 03
- 💬 Present findings concisely — this is internal analysis, not the deliverable

## EXECUTION PROTOCOLS:

- 🎯 Analyse the JD held in context from step 01
- 💾 Surface the key signals that will drive the proposal
- 📖 Auto-proceed to step 03 after presenting analysis

## CONTEXT BOUNDARIES:

- Available: full job description from step 01
- Focus: extract what matters for a tailored proposal
- Limits: no writing, no past project matching yet
- Dependencies: step 01 job description

---

## MANDATORY SEQUENCE

**CRITICAL:** Follow this sequence exactly. Do not skip, reorder, or improvise unless user explicitly requests a change.

### 1. Analyse the Job Description

Read the full JD and extract:

**Core Ask:** What is the client's primary problem or goal? (1 sentence — cut through the job title)

**Client Tone:** How does the client write? Formal / conversational / technical / urgent / cautious?

**Gaps and Pain Points:** What are they struggling with? What's the underlying frustration or risk?

**Budget Signals:** Any rate, budget range, or payment structure mentioned? Any signals (hourly vs fixed, "looking for best value", etc.)?

**Red Flags:** Anything that signals poor fit, scope creep risk, or low-quality engagement? Note honestly.

**What They'll Respond To:** Based on tone and core ask, what kind of proposal voice and angle will land?

### 2. Surface Analysis

Present the analysis briefly:

"**Analysis:**

- **Core ask:** [1 sentence]
- **Tone:** [descriptor]
- **Pain point:** [what's really driving this]
- **Budget signal:** [observation or 'none stated']
- **Red flag:** [if any — or 'none']
- **Proposal angle:** [what register and approach will land best]"

### 3. Auto-Proceed to Step 03

"**Pulling past projects now...**"

Load, read entire file, then execute {nextStepFile}.

---

## 🚨 SYSTEM SUCCESS/FAILURE METRICS:

### ✅ SUCCESS:

- Core ask captured in one sentence
- Client tone identified clearly
- Pain point surfaced (not just what was written)
- Proposal angle identified
- No proposal writing started
- Auto-proceeded to step 03

### ❌ SYSTEM FAILURE:

- Starting to write the proposal in this step
- Selecting a past project before step 03
- Skipping tone or pain point analysis
- Over-long analysis that buries the signal

**Master Rule:** Skipping steps is FORBIDDEN.
