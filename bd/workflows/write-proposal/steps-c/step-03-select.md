---
name: 'step-03-select'
description: 'Read the sidecar and select the most relevant past project for this proposal'
nextStepFile: './step-04-write.md'
sidecarMemories: '{project-root}/_bmad/_memory/bdo-sidecar/memories.md'
---

# Step 3: Select Past Project

## STEP GOAL:

Read BDO's past project knowledge base and select the single most relevant project to reference in the proposal.

## MANDATORY EXECUTION RULES (READ FIRST):

### Universal Rules:

- 📖 CRITICAL: Read the complete step file before taking any action
- 🔄 CRITICAL: When loading next step with 'C', ensure entire file is read first
- ✅ YOU MUST ALWAYS SPEAK OUTPUT In your Agent communication style with the config `{communication_language}`

### Role Reinforcement:

- ✅ You are BDO — drawing on real work history, not inventing examples
- ✅ Relevance > recency. Pick the project that best matches the client's core ask
- ✅ If no strong match exists, say so honestly

### Step-Specific Rules:

- 🎯 Read the COMPLETE {sidecarMemories} file — do not skim
- 🚫 FORBIDDEN to invent or fabricate a past project if none matches
- 🚫 FORBIDDEN to select multiple projects — one reference only
- 💬 If the user specified a past project in step 01, use that instead
- ⚙️ TOOL/SUBPROCESS FALLBACK: If file I/O is unavailable, ask the user to paste the contents of their memories.md file

## EXECUTION PROTOCOLS:

- 🎯 Load {sidecarMemories} and read it completely
- 💾 Select the single best-matching past project
- 📖 Present selection with reasoning; allow user to override

## CONTEXT BOUNDARIES:

- Available: JD from step 01, analysis from step 02, past projects from sidecar
- Focus: match past project to client's core ask
- Limits: one project only; no fabrication
- Dependencies: step 02 analysis (core ask + client tone)

---

## MANDATORY SEQUENCE

**CRITICAL:** Follow this sequence exactly. Do not skip, reorder, or improvise unless user explicitly requests a change.

### 1. Load Past Projects

Load and read the COMPLETE file at {sidecarMemories}.

If the file is empty or does not exist:

"**No past projects found in the knowledge base.** The proposal can still be written, but it won't reference a specific project — which weakens it significantly. Want to add a project now via the manage-past-projects workflow, or continue without a reference?"

- If user wants to add: Exit and launch manage-past-projects workflow
- If user wants to continue: Note 'no past project available' and proceed to step 04

### 2. Match to Core Ask

Using the core ask and pain point from step 02, scan all past projects for the best fit:

- Closest match on deliverable type
- Closest match on client type or industry
- Strongest outcome/result that maps to what this client needs
- Avoid surface-level matches (same tool used) — look for same problem solved

### 3. Present Selection

Show the selected project and reasoning:

"**Selected past project:**

- **Project:** [project name or label]
- **Why:** [1 sentence — what makes this the right match for this JD]
- **Key reference:** [the specific outcome or result that will land in the proposal]"

If no strong match exists, be honest:

"**No close match found.** I'll reference [closest available project] with a note that the fit is partial. Consider adding a stronger match to your past projects after this."

### 4. Present MENU OPTIONS

Display: **Select:** [O] Override — choose a different project [C] Continue

#### EXECUTION RULES:

- ALWAYS halt and wait for user input
- ONLY proceed to writing when user selects 'C' or confirms override

#### Menu Handling Logic:

- IF O: Ask user to name the project they'd like to use; confirm selection; redisplay menu
- IF C: Load, read entire file, then execute {nextStepFile}
- IF Any other: help user, then redisplay menu

---

## 🚨 SYSTEM SUCCESS/FAILURE METRICS:

### ✅ SUCCESS:

- sidecarMemories file read completely
- Single best-matching project identified
- Selection presented with clear reasoning
- Empty sidecar handled gracefully with user decision
- User confirmed selection before proceeding

### ❌ SYSTEM FAILURE:

- Not reading the full sidecar file
- Fabricating a past project that doesn't exist
- Selecting multiple projects
- Proceeding without user confirmation

**Master Rule:** Skipping steps is FORBIDDEN.
