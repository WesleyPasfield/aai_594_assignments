# AAI 594 — Assignment 4a Submission

**Name:**
**Date:**

> **Setup:** Your submission folder should look like:
>
> ```
> assignment_4/
> ├── driver.ipynb                      ← executed notebook with all outputs
> ├── SUBMISSION_4a.md                  ← this file (with your analysis written in)
> ├── PROPOSAL_4b.md                    ← project proposal
> └── screenshots/
>     └── ai_playground.png             ← AI Playground with UC tools + MCP (required)
> ```

---

## Criterion 1: Executed 5 test traces across 3 models

Run the evaluation cell in driver.ipynb so that all 5 test queries execute against all 3 LLMs in `LLMS_TO_COMPARE`. The notebook output should show 15 total traces (5 queries × 3 models) with responses visible.

**Test queries run:**

| # | Query | Purpose |
|---|-------|---------|
| 1 | "What models are involved in testing?" | UC function — list/enumerate tool |
| 2 | "Analyze the complexity of: What is 2+2?" | UC function — simple instruction analysis |
| 3 | "What sources are available in the dataset and how do they compare in size?" | UC function — multi-part lookup |
| 4 | "Search the web for the latest news about Llama models from Meta." | MCP tool — web search |
| 5 | "How has vicuna-33b performed against llama-2-70b-chat?" | UC function — model comparison |

**Models compared:**
- `databricks-gpt-oss-120b`
- `databricks-gpt-oss-20b`
- `databricks-llama-4-maverick`

**Checklist:**

- [ ] Evaluation cell executed with all outputs visible in the notebook.
- [ ] 15 traces present (5 queries × 3 models) in the notebook output or Experiments UI.
- [ ] AI Playground screenshot included at `screenshots/ai_playground.png`.

---

## Criterion 2: Written model comparison

**Write your analysis below. Do not use AI to write this — review the traces yourself and answer in your own words.**

Look at the notebook output and the MLflow Experiments UI (trace view) to answer the questions below. You don't need to answer every sub-question exhaustively — pick the observations that stood out most to you.

---

### Tool selection

1. For each of the 5 queries, did all three models call the correct tool? Were there any queries where a model chose the wrong tool, skipped a tool entirely, or called an unnecessary one?

2. Did any model call multiple tools in sequence when one would have sufficed, or vice versa? What does that suggest about how differently these models reason about tool use?

**Your answer:**

---

### Response quality

3. For query 3 (sources comparison) and query 5 (vicuna vs llama comparison), which model's answer was most accurate and specific? Which was vaguest? What was different about how the responses were constructed?

4. For the web search query (query 4), did all three models successfully invoke the MCP tool and incorporate the results into their answer? If one failed or hallucinated, describe what happened.

**Your answer:**

---

### Style and behavior

5. How did the length and tone of responses differ between models? Was verbosity helpful or did it obscure the answer?

6. When the agent retrieved a tool result, did any model add unsolicited commentary, caveats, or hallucinated detail beyond what the tool returned? Give a specific example if so.

**Your answer:**

---

### Judgment

7. Based on what you observed, which model would you choose to back this agent if you were deploying it for real users? Why? What trade-offs are you accepting with that choice?

**Your answer:**

---

## Grading Rubric

### Criterion 1: Execution (40%)

*Did the student run all 5 test queries against all 3 models?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|------------------|------------|-------|------------|
| All 15 traces visible in notebook output or Experiments UI. All 5 queries and all 3 models present. AI Playground screenshot included. | 10–14 traces present; one model or query missing. Screenshot included. | Fewer than 10 traces or only 1–2 models tested. | Evaluation cell not run or no outputs visible. |

### Criterion 2: Analysis (60%)

*Did the student meaningfully assess the differences between models in their own words?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|------------------|------------|-------|------------|
| Answers address tool selection, response quality, and a judgment call with specific examples drawn from the traces. Observations are concrete (e.g. "Model X called `compare_models` twice for query 5 before answering"). Clearly written in the student's own words — not AI-generated prose. | Most questions answered with some specificity. May lack concrete examples or skip one category entirely. | Answers are generic or surface-level (e.g. "Model A was better overall"). Little reference to specific traces. | Analysis not written, or clearly AI-generated with no original observation. |

---

## Notes (optional)

Add any notes, issues you ran into, or things you tried here.
