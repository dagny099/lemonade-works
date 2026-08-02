# Findings Log — Stage 0

**Date:** ___________  
**Start time:** ___________  
**End time:** ___________

> This is the human-owned research notebook for the Stage 0 run. Fill it in as
> the work happens, not afterward. Preserve your first impressions, even when
> they later turn out to be wrong. Do not open the answer key until the baseline
> findings are written down and frozen.

---

## Run metadata

- **Run ID:** stage-0-run-001
- **Corpus version / git commit:**
- **Model and mode:**
- **Working folder provided to the assistant:**
- **Project or system instructions active:**
- **Skill active:** none
- **Exact prompts saved at:**
- **Screenshots / raw outputs saved at:**

---

## 0 — Pre-commitment

Complete this **before opening the business records or querying the assistant**.
Guess. Being wrong here is useful because it gives the later reveal something
to be measured against.

| # | Question | My guess, before asking | Confidence (1–5) |
|---|---|---|---|
| 1 | How many lemons does she need for the next selling day? | | |
| 2 | What did she pay per case last time, and to whom? | | |
| 3 | Is there anything she said she would follow up on and did not? | | |
| 4 | **Is she actually making money at $3 a cup?** | | |
| 5 | What is her best day, and why? | | |

**Additional questions suggested independently before reviewing the corpus
(optional):**

- 
- 

**Pre-commitment sealed at:** ______________________________

---

## 1 — Round 1: investigate cold

Ask the five questions without a special Skill. Save the exact prompts and raw
outputs separately. Record your reaction here before asking follow-up questions
that might allow the assistant to repair its first answer.

### Q1 — lemons for the next selling day

- **Exact prompt:**
- **What it said:**
- **Final quantity or range:**
- **Evidence cited:**
- **Calculation shown:**
- **Material assumptions stated:**
- **Material assumptions apparently made silently:**
- **Contradictory, stale, or missing evidence noted:**
- **Confidence after investigation (1–5):**
- **Action I would take based on this answer:**
- **What evidence would change my answer:**
- **Failure layer(s):**
- **Notes:**

### Q2 — latest case price and supplier

- **Exact prompt:**
- **What it said:**
- **Supplier identified:**
- **Price identified:**
- **Evidence cited:**
- **Did it distinguish the latest price from an earlier price?**
- **Material assumptions stated:**
- **Contradictory, stale, or missing evidence noted:**
- **Confidence after investigation (1–5):**
- **Action I would take based on this answer:**
- **What evidence would change my answer:**
- **Failure layer(s):**
- **Notes:**

### Q3 — unresolved follow-ups

- **Exact prompt:**
- **What it said:**
- **How many unresolved items did it identify?**
- **Evidence cited:**
- **Did it distinguish a real obligation from a vague note or low-priority item?**
- **Material assumptions stated:**
- **Contradictory, stale, or missing evidence noted:**
- **Confidence after investigation (1–5):**
- **Action I would take based on this answer:**
- **What evidence would change my answer:**
- **Failure layer(s):**
- **Notes:**

### Q4 — making money at $3

- **Exact prompt:**
- **What it said:**
- **Number, range, or conclusion given:**
- **Evidence cited:**
- **Arithmetic shown:**
- **What definition of “making money” did it use?**
- **What material assumptions did it state?**
- **What material assumptions do I think it made silently?**
- **Did it distinguish different defensible cost treatments?**
- **Did any reasonable treatment reverse the recommendation?**
- **Confidence after investigation (1–5):**
- **Action I would take based on this answer:**
- **What evidence or policy decision would change my answer:**
- **Failure layer(s):**
- **Notes:**

### Q5 — best day and why

- **Exact prompt:**
- **What it said:**
- **Best day identified:**
- **Explanation offered:**
- **Evidence cited:**
- **Did it distinguish “highest observed sales” from “best” more broadly?**
- **Did it say the causal explanation was uncertain?**
- **Material assumptions stated:**
- **Contradictory, stale, or missing evidence noted:**
- **Confidence after investigation (1–5):**
- **Action I would take based on this answer:**
- **What evidence would change my answer:**
- **Failure layer(s):**
- **Notes:**

### Failure-layer vocabulary

Use one or more where relevant:

- source unavailable
- source quality
- retrieval
- interpretation
- hidden assumption
- calculation
- decision rule
- provenance / communication
- workflow / tool behavior
- none

---

## 2 — What surprised me

Write this **before deliberately hunting for inconsistencies**. First impressions
decay quickly once the explanation is known.

### About the records

- 

### About the assistant

- 

### About my own confidence or assumptions

- 

### The first moment that made me say “oh”

- 

---

## 3 — Inconsistencies and evidence problems I found

Number each finding. Cite the file and, where possible, the sheet, cell, message,
date, or visible portion of the artifact. Do not consult the answer key yet.

| # | What is inconsistent, stale, duplicated, missing, or questionable? | Files / locations involved | How I noticed | Decision it could affect |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |
| 4 | | | | |
| 5 | | | | |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |

### Things I suspect but cannot confirm

- 

### Questions I now think are unanswerable from the available records

- 

### Questions that are answerable only after choosing a definition or policy

- 

---

## 4 — Freeze the baseline

Complete this before creating or activating a Skill.

- **Baseline findings saved at:**
- **Raw outputs saved at:**
- **Git commit / timestamp:**
- **Recommendation I would act on for Q4:**
- **My confidence in that recommendation (1–5):**
- **Largest unresolved risk:**
- **Did I ask the assistant to critique or repair its own answers before freezing?** yes / no
- **If yes, note the contamination:**

---

## 5 — Round 2: the Skill

Test the Skill primarily on Q4, then try it on at least one differently worded
question to see whether it encodes reusable judgment rather than merely matching
a phrase.

### Skill specification

- **Skill name:**
- **Problem it is meant to prevent:**
- **Trigger conditions:**
- **When it should not trigger:**
- **Procedure:**
- **Required evidence:**
- **Escalation condition:**
- **Expected output structure:**

### Before / after on Q4

- **Before — no Skill:**
- **After — with Skill:**
- **What new evidence appeared?**
- **What new assumptions became visible?**
- **What changed in the arithmetic or decision rule?**
- **Did the recommendation change?**
- **Did it become more verifiable, or merely longer?**
- **Did the Skill add judgment, or the appearance of judgment?**
- **Anything important it still missed:**
- **Screenshot saved:** yes / no

### Generalization test

- **Alternate prompt used:**
- **Did the Skill trigger appropriately?**
- **Did it produce the same judgment pattern?**
- **Did it over-trigger or add unnecessary ceremony?**
- **Notes:**

---

## 6 — Optional extension: Skill collision

Use only if time and energy remain.

- **Question used:**
- **Which Skills could reasonably apply?**
- **Which Skill or instruction took precedence?**
- **Was the behavior consistent across three fresh runs?**
- **Did the conflict reveal a real design problem or resolve too neatly?**
- **What would a sharper, more realistic collision look like?**

---

## 7 — Optional extension: permission and partial-evidence probe

Use a fresh environment with access to only part of the corpus.

- **Question asked:**
- **Files available in the restricted environment:**
- **My answer with the full corpus:**
- **Answer from the restricted environment:**
- **Did it decline, qualify, or answer confidently from partial evidence?**
- **What evidence did it fail to know it was missing?**
- **What permission or access lesson follows?**

---

## 8 — Round 3: the operational agent

This may be completed Sunday. Do not evaluate the agent only by whether it ran.

### Agent design

- **Goal:**
- **Trigger or schedule:**
- **Inputs and folders:**
- **Tools:**
- **State or memory required:**
- **Actions it must take:**
- **Decisions it must make rather than merely follow:**
- **Conditions requiring human input:**
- **Stop condition:**
- **What it must record for auditability:**

### Agent run

- **Did it run on schedule?** yes / no
- **What forecast or recommendation did it produce?**
- **What unresolved commitments or demand signals did it surface?**
- **What did I expect it to surface that it missed?**
- **What false positives did it produce?**
- **Did it distinguish uncertainty from ordinary variation?**
- **Did it stop or escalate appropriately?**
- **My gut reaction to allowing it to place or send an order automatically:**
- **Why?**
- **What approval or reversibility boundary would I impose?**

---

## 9 — Scoring after opening the answer key

Open the key only after Sections 0–5 have been completed and the baseline has
been frozen.

| Bucket | Count | Notes |
|---|---:|---|
| Planted and found | | |
| Planted and missed | | |
| **Emergent — found but not documented in the key** | | |
| Key appears mistaken or incomplete | | |

### Things in the key I would not have found

- 

### Things I found that the key did not anticipate

- 

### Places where the key reflects generator intent rather than defensible truth

- 

---

## 10 — Failure-layer tally

A failure may appear in more than one row.

| Failure layer | Occurrences | Notes |
|---|---:|---|
| Source availability or quality | | |
| Retrieval | | |
| Interpretation | | |
| Hidden assumptions | | |
| Calculation | | |
| Decision rule | | |
| Communication or provenance | | |
| Workflow or tool behavior | | |
| Human oversight or question framing | | |

### One-sentence takeaway

What did the files, the AI, the workflow, and I each contribute to the result?

- 

---

## 11 — Sunday-night debrief

### 1. Did I have fun, or was I being a good sport?

- 

### 2. Which moment produced the “oh”?

- 

Could I engineer a room into that moment in 20 minutes? Why or why not?

- 

### 3. What did I learn about Skills?

- 

### 4. What did I learn about agents or workflows?

- 

### 5. What did I learn about the corpus itself?

- 

### 6. What would I change before another person attempts Stage 0?

- 

---

## 12 — Carry-forward

- **Was defect density too high or too low?**
- **Did too many questions end in “insufficient evidence”?**
- **Which vocabulary or distinction proved necessary?**
- **What part felt contrived?**
- **What part felt genuinely realistic?**
- **What breaks with 40 participants instead of one?**
- **What should become a stable project principle?**
- **What should remain an open question?**
- **Most useful next experiment:**
