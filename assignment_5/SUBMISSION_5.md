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
>     └── eval_results.png              ← required: MLflow Evaluation Runs screenshot (see notebook Section 9)
> ```

---

## Deliverables

### 1. Executed Notebook

- [ ] **Section 3:** Embeddings table verified.
- [ ] **Section 4:** Agent loaded and verified with a test query.
- [ ] **Section 5:** Evaluation dataset created (8+ provided, 5 your own questions with expected_facts where applicable). UC-backed `eval_dataset` created and passed to `mlflow.genai.evaluate()`.
- [ ] **Section 6:** Predict function and built-in judge (`RelevanceToQuery`) defined.
- [ ] **Section 7:** Guidelines judges (`tool_citation`, `data_grounding`) defined.
- [ ] **Section 8:** Custom judge (example and/or your own) defined.
- [ ] **Section 9:** Combined evaluation ran with all judges (built-in, both guidelines, your custom). All analysis questions (9a–9c and any others) answered.
- [ ] **Evaluation screenshot:** Screenshot of MLflow Evaluation Runs (Experiments → run → Evaluation Runs; "Group by Session" off) showing at least 12 traces and all assessment columns. File: `screenshots/eval_results.png` (or similar).
- [ ] **Clean up:** Confirmed no Vector Search cleanup needed (embeddings persist in Delta table).

---

## Grading Rubric

### Criterion 1: Evaluation Dataset Quality (20%)

*Did the student create a diverse, well-designed evaluation dataset?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Dataset includes 12+ questions (7 provided, 5 your own) covering all tool types (lookup, analyze, no-tool, edge cases). UC-backed `eval_dataset` used in evaluate. Student's 5 custom questions test meaningfully different scenarios, including their custom functions. | Dataset includes 10+ questions. UC-backed dataset created and passed to evaluate. Student's custom questions are present but may overlap with provided ones. | Fewer than 10 questions or student questions are trivial/duplicate. | Eval dataset not created or only contains the provided questions with no additions. |

### Criterion 4: Custom Judge Design (30%)

*Did the student create and run a meaningful custom judge?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Custom judge ran with a well-crafted prompt template. The judge evaluates something distinct from the built-in and guidelines judges. Results are meaningful. | Custom judge ran. Prompt is reasonable but may overlap with guidelines judges. | Custom judge attempted but errored or prompt is trivial. | Not attempted. |

### Criterion 4: Evaluation Job and Results (20%)

*Did the student execute the evaluation job and provide a screenshot of the evaluation run output?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Evaluation job ran successfully. Screenshot from MLflow Experiments UI shows Evaluation Runs with "Group by Session" off, at least 12 traces (7 provided + 5 student questions), and all assessment columns (e.g. Relevance, data_grounding, tool_citation, custom judge) visible. Screenshot included in submission (e.g. `screenshots/eval_results.png`). | Evaluation ran. Screenshot provided but may show grouped view or fewer than 12 traces. | Evaluation ran but screenshot missing, unclear, or shows only grouped session view. | Evaluation not run or no screenshot provided. |

### Criterion 5: Analysis and Reflection (30%)

*Did the student provide a thoughtful comparative analysis?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| All analysis questions (e.g. 9a–9c) answered with specific examples from evaluation results. Student identifies judge disagreements and explains why. Connects to at least one Week 5 reading. Proposes concrete agent improvements based on findings. | Answers present but lack specific examples or reading connection. | Answers are brief or generic. May skip questions. | Analysis section empty or placeholder text only. |

---

## Notes (optional)

Add any notes, issues you ran into, or things you tried here.
