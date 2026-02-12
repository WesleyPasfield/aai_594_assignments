# AAI 594 — Assignment 6 Submission

**Name:**  
**Date:**

> **Setup:** Your submission folder should look like:
>
> ```
> assignment_6/
> ├── AAI_594_Assignment_6_Lab.ipynb   ← executed notebook with all outputs
> ├── SUBMISSION_6.md                  ← this file
> └── screenshots/
>     └── (optional: MLflow traces UI, aligned judge comparison)
> ```

---

## Deliverables

### 1. Executed Notebook

- [ ] **Section 3:** Agent and custom judge recreated. Vector Search endpoint and index working.
- [ ] **Section 4:** 15 traces generated with outputs visible in notebook.
- [ ] **Section 5:** Human feedback logged for all 15 traces. Ratings (True/False) and rationales are specific and honest — not just placeholder text.
- [ ] **Section 6:** `align()` ran successfully. Both original and aligned judge comparison results visible.
- [ ] **Section 7:** All four reflection questions answered thoughtfully.
- [ ] **Section 8:** Cleanup confirmed — endpoint and index deleted.

### 2. Deployment (Optional)

- [ ] **Section 9:** Attempted deployment or reviewed the conceptual walkthrough.

---

## Grading Rubric

### Criterion 1: Trace Generation (20%)

*Did the student generate meaningful traces for human review?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| 15 traces generated with diverse questions (tools, no-tools, edge cases, multi-step). Trace outputs visible in notebook. Student can identify traces in MLflow UI. | 15 traces generated but questions lack diversity. Outputs visible. | Fewer than 15 traces or many errored. | No traces generated. |

### Criterion 2: Feedback Quality and Thoroughness (25%)

*Did the student provide genuine, thoughtful human feedback for all traces?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| All 15 traces have feedback with honest ratings and specific rationales. Student clearly reviewed the actual outputs — rationales reference specific agent behavior (e.g., "called wrong tool", "missed the comparison"). Mix of True/False ratings shows critical evaluation. | All 15 traces have feedback. Rationales are reasonable but may be generic ("looks good"). Mostly True ratings with 1-2 False. | Fewer than 15 traces have feedback. Rationales are copy-paste or single words. | Placeholder feedback not replaced. No actual review performed. |

### Criterion 3: Align Execution and Analysis (25%)

*Did align() run successfully and did the student analyze the results?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| `align()` completed successfully. Student compares original vs. aligned judge prompts and explains the differences. Comparison evaluation shows the aligned judge better matches human feedback. Student understands the SIMBA optimization concept. | `align()` ran. Some comparison analysis but lacks depth. May not fully explain prompt differences. | `align()` attempted but errored, or analysis is minimal. | Not attempted. |

### Criterion 4: Reflection (20%)

*Does the reflection demonstrate deep understanding of human-in-the-loop evaluation?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| All 4 questions answered with specific examples from this assignment. Connects to "Who Validates the Validators" reading. Articulates why automated judges alone are insufficient. Proposes a concrete plan for their final project. | Answers present and reasonable. May lack specific examples or reading connection. Proposal is generic. | Brief or surface-level answers. Missing questions. | Placeholder text only. |

### Criterion 5: Notebook Quality (10%)

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| All cells executed with outputs. Clean code. Cleanup confirmed. Coherent progression from traces to feedback to alignment. | Most cells executed. Minor issues. | Significant cells missing output. | Not executed or missing major sections. |

---

## Notes (optional)

Add any notes, issues you ran into, or things you tried here.
