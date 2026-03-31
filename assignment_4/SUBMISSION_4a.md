# AAI 510 — Assignment 4a Submission

**Name:**
**Date:**

> **Setup:** Your submission folder should look like:
>
> ```
> assignment_4/
> ├── AAI_510_Assignment_4a_lab.ipynb   ← executed notebook with all outputs
> ├── SUBMISSION_4a.md                  ← this file (with your analysis written in)
> ├── PROPOSAL_4b.md                    ← project proposal
> └── screenshots/
>     └── ai_playground.png             ← AI Playground with UC tools + MCP (required)
> ```

---

## Required

### Notebook execution

Run the evaluation cell so that all 5 test queries execute against all 3 LLMs in `LLMS_TO_COMPARE`. The notebook output should show 15 total traces (5 queries × 3 models) with responses visible.

**Test queries:**

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

- [ ] Evaluation cell executed with all outputs visible in the notebook.
- [ ] 15 traces present (5 queries × 3 models) in the notebook output or Experiments UI.

### AI Playground Screenshot (Required)

Paste a screenshot of the AI Playground showing your agent with UC tools and MCP attached and a successful tool-calling conversation.

![AI Playground with UC tools + MCP server](screenshots/ai_playground.png)

### Project Proposal (Required)

- [ ] `PROPOSAL_4b.md` completed and included in the submission folder.

---

## Optional but Strongly Encouraged

### Prompt Optimization with GEPA

Run the optional GEPA cell in the notebook to automatically improve your agent's system prompt. The code is experimental — run it if you want to explore prompt optimization, but it is not required.

- [ ] GEPA optimization cell run with output visible.

---

## Short-answer Questions

**Do not use AI for these answers.** Review the traces in the notebook output or MLflow Experiments UI and answer in your own words. Each answer should be 2–3 sentences unless the question doesn't warrant more (e.g. if no hallucinations occurred, say so briefly).

### Tool selection

**Q1.** For each of the 5 queries, did all three models call the correct tool? Were there any queries where a model chose the wrong tool, skipped a tool entirely, or called an unnecessary one?

*Write your answer below:*

**[Your answer here]**

**Q2.** Did any model call multiple tools in sequence when one would have sufficed, or vice versa? What does that suggest about how differently these models reason about tool use?

*Write your answer below:*

**[Your answer here]**

### Response quality

**Q3.** For query 3 (sources comparison) and query 5 (vicuna vs llama comparison), which model's answer was most accurate and specific? Which was vaguest? What was different about how the responses were constructed?

*Write your answer below:*

**[Your answer here]**

**Q4.** For the web search query (query 4), did all three models successfully invoke the MCP tool and incorporate the results into their answer? If one failed or hallucinated, describe what happened.

*Write your answer below:*

**[Your answer here]**

### Style and behavior

**Q5.** How did the length and tone of responses differ between models? Was verbosity helpful or did it obscure the answer?

*Write your answer below:*

**[Your answer here]**

**Q6.** When the agent retrieved a tool result, did any model add unsolicited commentary, caveats, or hallucinated detail beyond what the tool returned? Give a specific example if so.

*Write your answer below:*

**[Your answer here]**

### Judgment

**Q7.** Based on what you observed, which model would you choose to back this agent if you were deploying it for real users? Why? What trade-offs are you accepting with that choice?

*Write your answer below:*

**[Your answer here]**

---

## Grading Rubric

### Criterion 1: Execution (40%)

*Did the student run all 5 test queries against all 3 models?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|------------------|------------|-------|------------|
| All 15 traces visible in notebook output or Experiments UI. All 5 queries and all 3 models present. AI Playground screenshot included. | 10–14 traces present; one model or query missing. Screenshot included. | Fewer than 10 traces or only 1–2 models tested. | Evaluation cell not run or no outputs visible. |

### Criterion 2: Analysis — NO AI Usage (60%)

*Did the student meaningfully assess the differences between models in their own words?*

| Meets or Exceeds | Approaches | Below | Inadequate |
|------------------|------------|-------|------------|
| Answers address tool selection, response quality, and a judgment call with specific examples drawn from the traces. Observations are concrete (e.g. "Model X called `compare_models` twice for query 5 before answering"). Clearly written in the student's own words — not AI-generated prose. | Most questions answered with some specificity. May lack concrete examples or skip one category entirely. | Answers are generic or surface-level (e.g. "Model A was better overall"). Little reference to specific traces. | Analysis not written, or clearly AI-generated with no original observation. |

---

## Notes (optional)

Add any notes, issues you ran into, or things you tried here.
