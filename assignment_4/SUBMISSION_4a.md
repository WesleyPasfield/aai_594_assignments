# AAI 594 — Assignment 4a Submission

**Name:**  
**Date:**

> **Setup:** Your submission folder should look like:
>
> ```
> assignment_4/
> ├── AAI_594_Assignment_4a_Lab.ipynb   ← executed notebook with all outputs
> ├── SUBMISSION_4a.md                  ← this file
> ├── PROPOSAL_4b.md                    ← project proposal
> └── screenshots/
>     └── ai_playground.png             ← Section 4 (required)
> ```

---

## Deliverables

### 1. Executed Notebook

- [ ] **Section 3:** Vector Search endpoint and index recreated successfully.
- [ ] **Section 4:** Prototyped agent in AI Playground with tools attached.
- [ ] **Section 5:** Agent code runs in notebook. Test queries produce tool-calling outputs.
- [ ] **Section 6:** UC functions listed via `SHOW USER FUNCTIONS`.
- [ ] **Section 7:** Prompt registered in UC Prompt Registry with two versions and "production" alias.
- [ ] **Section 8:** Same 3 queries run against 2 different LLMs with outputs visible.
- [ ] **Section 8:** Written comparison analysis of the two models.
- [ ] **Section 9:** Cleanup confirmed — endpoint and index deleted.

### 2. AI Playground Screenshot (Required)

![AI Playground with tools and a tool-calling conversation](screenshots/ai_playground.png)

### 3. Project Proposal (Required)

- [ ] `PROPOSAL_4b.md` completed and included in submission folder.

### 4. Prompt Optimization Reflection (Optional)

- [ ] **Section 10:** Written reflection on prompt optimization concepts.

---

## Grading Rubric

### Criterion 1: Agent Implementation (30%)

*Did the student build a working agent with tool calling?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Agent runs in notebook and correctly calls UC functions in response to test queries. Code is well-organized with clear comments. Evidence of AI Playground prototyping (screenshot). Agent handles queries that don't need tools appropriately. | Agent runs and calls at least one tool correctly. Some test queries work. Screenshot provided but may show limited testing. | Agent code is present but fails on most queries or doesn't call tools. Limited evidence of Playground use. | No working agent code. No Playground screenshot. |

### Criterion 2: Prompt Registration (20%)

*Did the student register and version prompts correctly?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Prompt registered with two versions and a "production" alias. Student demonstrates loading by alias. Commit messages are descriptive. Student understands the purpose of versioning. | Prompt registered with at least one version. Alias may be missing or commit messages are generic. | Prompt registration attempted but incomplete or errors in output. | No prompt registration attempted. |

### Criterion 3: LLM Comparison (25%)

*Did the student meaningfully compare two LLMs?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Same 3 queries run against 2 models with all outputs visible. Written analysis covers tool usage, quality, verbosity, and error handling with specific examples from the outputs. Connects observations to agentic AI concepts. | Queries run against 2 models. Analysis covers some dimensions but may lack specific examples or depth. | Only one model tested, or analysis is superficial (e.g., "Model A was better"). | No comparison attempted. |

### Criterion 4: Notebook Quality (15%)

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| All cells executed with outputs. Clean code with comments. Cleanup confirmed. Coherent narrative from Playground to comparison. | Most cells executed. Minor issues with organization. | Significant cells missing output. Disorganized. | Notebook not executed or missing major sections. |

### Criterion 5: Prompt Optimization Reflection (10%)

| Meets or Exceeds | Approaches | Below | Inadequate |
|---|---|---|---|
| Thoughtful answers to all 3 reflection questions. Connects readings to the agent built in this assignment. Proposes a concrete metric for DSPy optimization. | Answers present but surface-level. May not connect to readings. | Brief or generic answers. | Section not attempted. |

---

## Notes (optional)

Add any notes, issues you ran into, or things you tried here.
