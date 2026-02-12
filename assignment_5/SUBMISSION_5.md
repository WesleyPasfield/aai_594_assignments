# AAI 594 — Assignment 5 Submission

**Name:**  
**Date:**

> **Setup:** Your submission folder should look like:
>
> ```
> assignment_5/
> ├── AAI_594_Assignment_5_Lab.ipynb   ← executed notebook with all outputs
> ├── SUBMISSION_5.md                  ← this file
> └── screenshots/
>     └── (optional: MLflow UI screenshots)
> ```

---

## Deliverables

### 1. Executed Notebook

- [ ] **Section 3:** Agent recreated and verified with a test query.
- [ ] **Section 4:** Evaluation dataset includes 8+ provided questions and 5 student-written questions with expected_facts.
- [ ] **Section 5:** Built-in judge (`RelevanceToQuery`) ran successfully with visible outputs.
- [ ] **Section 6:** Guidelines judges (`tool_citation`, `data_grounding`) ran successfully with visible outputs.
- [ ] **Section 7:** Custom judge (`tool_usage_quality`) ran successfully with visible outputs.
- [ ] **Section 8:** Combined evaluation ran with all 4 judges. All analysis questions answered.
- [ ] **Section 9:** Cleanup confirmed.

---

## Grading Rubric

### Criterion 1: Evaluation Dataset Quality (20%)

*Did the student create a diverse, well-designed evaluation dataset?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Dataset includes 13+ questions covering all tool types (lookup, analyze, no-tool, edge cases). Student's 5 custom questions test meaningfully different scenarios. Expected facts are specific and verifiable. | Dataset includes 10+ questions. Student's custom questions are present but may overlap with provided ones. Expected facts are reasonable. | Fewer than 10 questions or student questions are trivial/duplicate. Expected facts are vague. | Eval dataset not created or only contains the provided questions with no additions. |

### Criterion 2: Built-in Judge (15%)

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| RelevanceToQuery evaluation ran successfully. Student inspected results and understands what the scorer measures. | Evaluation ran but student didn't inspect results closely. | Evaluation attempted but errored or produced no results. | Not attempted. |

### Criterion 3: Guidelines Judge Design (20%)

*Did the student effectively use guidelines judges with meaningful rules?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Both guidelines judges ran successfully. Guidelines are specific and relevant to the UltraFeedback Expert agent. Results show meaningful differentiation (not all pass or all fail). | Guidelines judges ran. Rules are present but generic. | One judge ran; the other errored. Rules are vague. | Not attempted. |

### Criterion 4: Custom Judge Design (20%)

*Did the student create and run a meaningful custom judge?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Custom judge ran with a well-crafted prompt template. The judge evaluates something distinct from the built-in and guidelines judges. Results are meaningful. | Custom judge ran. Prompt is reasonable but may overlap with guidelines judges. | Custom judge attempted but errored or prompt is trivial. | Not attempted. |

### Criterion 5: Analysis and Reflection (15%)

*Did the student provide a thoughtful comparative analysis?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| All 4 analysis questions answered with specific examples from evaluation results. Student identifies judge disagreements and explains why. Connects to at least one Week 5 reading. Proposes concrete agent improvements based on findings. | Answers present but lack specific examples or reading connection. | Answers are brief or generic. May skip questions. | Analysis section empty or placeholder text only. |

### Criterion 6: Notebook Quality (10%)

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| All cells executed with outputs. Clean code. Cleanup confirmed. Coherent narrative. | Most cells executed. Minor issues. | Significant cells missing output. | Not executed or missing major sections. |

---

## Notes (optional)

Add any notes, issues you ran into, or things you tried here.
