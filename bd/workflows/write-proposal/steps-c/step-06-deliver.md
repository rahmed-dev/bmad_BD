---
name: 'step-06-deliver'
description: 'Deliver the final proposal with BDO confidence signal and save to output file'
outputFile: '{bd_artifacts}/proposals/proposal-{date}.md'
proposalTemplate: '../templates/proposal-template.md'
---

# Step 6: Deliver

## STEP GOAL:

Output the final, checked proposal with BDO's honest confidence signal, and save it to the output file.

## MANDATORY EXECUTION RULES (READ FIRST):

### Universal Rules:

- 📖 CRITICAL: Read the complete step file before taking any action
- ✅ YOU MUST ALWAYS SPEAK OUTPUT In your Agent communication style with the config `{communication_language}`

### Role Reinforcement:

- ✅ You are BDO — delivering the finished product with an honest signal
- ✅ The confidence signal is never performative — it reflects the actual quality of the match
- ✅ This is the moment of delivery; keep it clean and useful

### Step-Specific Rules:

- 🎯 Output the proposal exactly as it passed the quality check in step 05
- 🚫 FORBIDDEN to rewrite or modify the proposal at this stage
- 💬 Confidence signal must reflect genuine assessment — not always positive
- 💾 Save the proposal to {outputFile}

## EXECUTION PROTOCOLS:

- 🎯 Present the final proposal clearly
- 💾 Save to {outputFile} using {proposalTemplate} structure
- 📖 Provide honest confidence signal based on job-to-project match quality

## CONTEXT BOUNDARIES:

- Available: final checked proposal from step 05, analysis from step 02, selected project from step 03
- Focus: delivery and save
- Dependencies: steps 01–05 complete

---

## MANDATORY SEQUENCE

**CRITICAL:** Follow this sequence exactly. Do not skip, reorder, or improvise unless user explicitly requests a change.

### 1. Deliver the Proposal

Present the final proposal cleanly:

"**Your proposal:**

---
[final proposal text from step 05]

---"

### 2. Assess and Signal

Assess the proposal honestly against these criteria:
- How well does the past project actually match this job?
- Is the tone right for this client?
- Is the job post clear enough to have written a strong proposal?

Select the honest confidence signal:

| Signal | When to use |
|--------|-------------|
| *"This one's strong. Send it."* | Tight match, clear formula, right tone |
| *"Solid. The project reference lands well."* | Good match, clean execution |
| *"Client sounds formal — you may want to tighten the tone before sending."* | Casual draft for a formal-sounding client |
| *"Not much to work with here — I've made assumptions. Review before sending."* | Vague job post, limited detail |
| *"No close match in past projects — this one's weaker for it. Consider adding a relevant project."* | No strong sidecar match found |

Deliver the signal on a new line after the proposal.

"**BDO:** [confidence signal]"

### 3. Save to Output File

Save the proposal to {outputFile} using the structure from {proposalTemplate}:

- `date`: today's date
- `job_title`: the job title or a short descriptor from the JD
- `confidence`: the confidence signal text
- Proposal body: the final proposal text

### 4. Optional Next Step

Offer two quick options:

"Want to:
- **[A]** Add this project to your past projects knowledge base for future proposals
- **[D]** Done — that's everything"

#### Menu Handling Logic:

- IF A: Launch `{project-root}/_bmad/bd/workflows/manage-past-projects/workflow.md` to add to sidecar
- IF D or any other: Close out cleanly — "**Good luck with the bid.**"
- IF Any other question or comment: answer, then redisplay the two options

---

## 🚨 SYSTEM SUCCESS/FAILURE METRICS:

### ✅ SUCCESS:

- Final proposal delivered clearly
- Honest confidence signal provided
- Proposal saved to output file
- User offered the option to update their knowledge base

### ❌ SYSTEM FAILURE:

- Rewriting the proposal at delivery
- Generic or always-positive confidence signal
- Not saving to output file

**Master Rule:** Skipping steps is FORBIDDEN.
