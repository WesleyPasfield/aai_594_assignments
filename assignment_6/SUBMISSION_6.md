# AAI 594: Assignment 6 Submission

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
- [ ] **Section 4:** 12 traces generated with outputs visible in notebook.
- [ ] **Section 5:** Human feedback logged for all 12 traces. Ratings (True/False) and rationales are specific and honest, not just placeholder text.
- [ ] **Section 6:** SIMBA alignment ran successfully. Both original and aligned judge comparison results visible.
- [ ] **Section 7:** Both reflection questions answered thoughtfully.
- [ ] **Cleanup note:** Reviewed. No additional cleanup was required for this lab.

### 2. Submission Notes

- The optional `optimize_anything` / agent skills section is enrichment only. It is not required for submission and is not part of the grading rubric.

---

## Grading Rubric

### Criterion 1: Trace Generation (20%)

*Did the student generate meaningful traces for human review?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| 12 traces generated with diverse questions (tools, no-tools, edge cases, multi-step). Trace outputs visible in notebook. Student can identify traces in MLflow UI. | 12 traces generated but questions lack diversity. Outputs visible. | Fewer than 12 traces or many errored. | No traces generated. |

### Criterion 2: Judge and Feedback Execution (20%)

*Did the student run the judge and provide usable SME feedback?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Judge scores and SME feedback are present for all 12 traces. Labels and rationales clearly reflect actual review of trace behavior. | Most traces have judge results and SME feedback, but some rationales are shallow. | Feedback is incomplete or mostly generic. | Judge execution or SME feedback is missing. |

### Criterion 3: Align Execution and Analysis (30%)

*Did alignment run successfully, and did the student analyze the resulting judge?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| SIMBA alignment completed successfully. The student compares the original and aligned judge results and prompts, then explains how the aligned judge better matches human feedback. | Alignment ran and some comparison is present, but the analysis lacks depth or concrete examples. | Alignment was attempted but not completed, or analysis is minimal. | Alignment was not attempted. |

### Criterion 4: Reflection (30%)

*Does the reflection demonstrate deep understanding of human-in-the-loop evaluation?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Both reflection questions are answered with specific examples from this assignment. Responses connect alignment back to human-in-the-loop evaluation and explain why automated judges alone are insufficient. | Both answers are present and reasonable, but they lack specific examples or depth. | One reflection answer is missing or both are very surface-level. | Placeholder text only. |

---

## Notes (optional)

Add any notes, issues you ran into, or things you tried here.
