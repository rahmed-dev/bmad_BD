---
name: 'step-05-check'
description: 'Run quality checks on the proposal draft before delivery'
nextStepFile: './step-06-deliver.md'
---

# Step 5: Quality Check

## STEP GOAL:

Verify the proposal passes all structural, tonal, and human-quality standards before delivery.

## MANDATORY EXECUTION RULES (READ FIRST):

### Universal Rules:

- 📖 CRITICAL: Read the complete step file before taking any action
- 🔄 CRITICAL: When loading next step, ensure entire file is read first
- ✅ YOU MUST ALWAYS SPEAK OUTPUT In your Agent communication style with the config `{communication_language}`

### Role Reinforcement:

- ✅ You are BDO running a pre-send quality gate — honest and precise
- ✅ Flag real issues; don't rubber-stamp the draft
- ✅ If the proposal needs a fix, fix it before proceeding

### Step-Specific Rules:

- 🎯 Run ALL checks — do not skip any
- 🚫 FORBIDDEN to pass a failing proposal without fixing it first
- 💬 Be direct about failures — this is a quality gate, not a formality
- ⚙️ Fix the proposal in this step if any check fails; deliver the fixed version

## EXECUTION PROTOCOLS:

- 🎯 Run each check against the draft from step 04
- 💾 Note any failures and apply fixes
- 📖 Auto-proceed to delivery once all checks pass

## CONTEXT BOUNDARIES:

- Available: proposal draft from step 04
- Focus: quality assurance only — no new content decisions
- Dependencies: step 04 proposal draft

---

## MANDATORY SEQUENCE

**CRITICAL:** Follow this sequence exactly. Do not skip, reorder, or improvise unless user explicitly requests a change.

### 1. Run Structural Checks

**Check 1 — Word count:**
Count the words. Is it under 120?
- PASS: under 120 words
- FAIL: over 120 words → trim ruthlessly; remove any sentence that doesn't directly serve the formula

**Check 2 — Ends with a question:**
Does the final sentence end with a question mark?
- PASS: yes, and it's a specific, relevant question
- FAIL: no, or it's a generic call to action → rewrite the closing line

**Check 3 — No skill lists or tool lists:**
Scan for any list of skills, tools, or technologies.
- PASS: none present
- FAIL: lists found → replace with the past project reference that demonstrates those skills in action

**Check 4 — Past project referenced:**
Is there a specific reference to a past project — client type, deliverable, outcome?
- PASS: yes, specific and concrete
- FAIL: vague or missing → strengthen with the selected project from step 03

### 2. Run Human-Quality Checks

**Check 5 — No AI-pattern openers:**
Does the proposal start with "Certainly", "Great", "I'd be happy to", "As an experienced", "I noticed", "I came across", or similar?
- PASS: none present
- FAIL: replace the opener with a direct observation from the JD

**Check 6 — No ` - ` as sentence connector:**
Scan for ` - ` used between clauses or sentences.
- PASS: none present
- FAIL: rewrite the affected sentences using proper punctuation (full stop, comma, or rephrase)

**Check 7 — No hedging language:**
Scan for "I believe", "I think", "potentially", "perhaps", "it seems", "might be able to", or similar hedges.
- PASS: none present
- FAIL: replace with direct, confident phrasing

**Check 8 — No bullet points or lists in the body:**
Is the proposal written in flowing prose?
- PASS: yes, prose only
- FAIL: rewrite as prose

**Check 9 — Tone match:**
Does the proposal's register match the client tone identified in step 02?
- PASS: tone is consistent
- FAIL: adjust register to match (formal client → tighten formality; casual client → loosen slightly)

**Check 10 — Sounds human:**
Read the proposal as a whole. Does it sound like a confident professional wrote it, or does it read like a template?
- PASS: natural, specific, confident
- FAIL: identify the AI-sounding phrases and rewrite them with direct, specific language

### 3. Apply Fixes

For any failed check, apply the fix directly to the proposal. Do not leave failures unfixed.

After all fixes: re-read the full proposal once more to confirm it flows naturally as a whole.

### 4. Auto-Proceed to Delivery

"**All checks passed. Delivering...**"

Load, read entire file, then execute {nextStepFile}.

---

## 🚨 SYSTEM SUCCESS/FAILURE METRICS:

### ✅ SUCCESS:

- All 10 checks run
- Any failures fixed before proceeding
- Final proposal is under 120 words, ends with question, sounds human
- No AI patterns, no dashes as connectors, no lists
- Auto-proceeded to step 06

### ❌ SYSTEM FAILURE:

- Skipping any check
- Passing a failing proposal without fixing it
- Delivering a proposal that fails one or more checks

**Master Rule:** Skipping steps is FORBIDDEN.
