# AAI 594 — Agentic AI

**University of San Diego | Masters in Applied Artificial Intelligence**

An 8-week graduate course on building, evaluating, and improving agentic AI systems. Students build the **UltraFeedback Expert** — a tool-calling agent on Databricks — progressing from environment setup to human-aligned evaluation.

## Platform

All assignments run on **Databricks Free Edition** with serverless compute. Key technologies:

- **Unity Catalog** for data governance, functions, and prompt management
- **MLflow 3** for tracing, evaluation, and human feedback
- **Foundation Model APIs** (Llama, Claude, etc.) for LLM access
- **Vector Search** for semantic retrieval
- **Cursor IDE** with Databricks Connect for local development

## Dataset

[UltraFeedback](https://www.kaggle.com/datasets/thedrcat/llm-human-preference-data-ultrafeedback) — an LLM human preference dataset used throughout the course.

## Assignments

### Assignment 1 — Environment Setup (Week 1: What Are Agents)

`assignment_1/`

Set up the Databricks workspace, configure Unity Catalog, load the UltraFeedback dataset from Kaggle, write it as a Delta table, and make your first LLM call via the Foundation Model API. Install the Databricks CLI and optionally configure Cursor IDE with Databricks Connect.

**Deliverables:** Executed notebook, submission template

---

### Assignment 2 — Exploratory Data Analysis (Week 2: Models + Platforms)

`assignment_2/`

Perform EDA on the UltraFeedback dataset. Query the data, assess what's available, identify what's useful for an LLM, and determine what transformations might be needed for downstream agent use.

**Deliverables:** Executed notebook, submission template

---

### Assignment 3 — Agent Tools (Week 3: Agent Tooling)

`assignment_3/`

Build the tools your agent will use:
- **Unity Catalog SQL function** (`lookup_source_info`) — deterministic data lookups
- **Unity Catalog Python function** (`analyze_instruction`) — instruction complexity analysis
- **Your own custom function** — student-designed tool
- **Vector Search** — semantic search over 1,000 UltraFeedback instructions (Delta Sync Index with managed embeddings)
- **External MCP server** — configure You.com web search in Cursor
- **Bonus:** Create an Agent Skill (`SKILL.md`)

**Deliverables:** Executed notebook, MCP screenshot, submission template

---

### Assignment 4a — From Tools to a Working Agent (Week 4: Frameworks + Prompt Optimization)

`assignment_4/`

Wire your tools into a working agent:
1. **Prototype in AI Playground** — select a tools-enabled LLM, attach UC functions and Vector Search, test tool-calling conversations
2. **Export the code** — use "Get code > Create agent notebook" to generate a starting point
3. **Register a prompt** — version your system prompt in the Unity Catalog Prompt Registry with aliases
4. **Swap LLMs and compare** — run the same queries against two Foundation Models and analyze differences in tool usage, quality, and verbosity
5. **Optional:** Reflect on prompt optimization concepts (DSPy) from the readings

**Deliverables:** Executed notebook, AI Playground screenshot, submission template

### Assignment 4b — Project Proposal

`assignment_4/PROPOSAL_4b.md`

Submit a final project proposal: problem statement, agent design, data sources, evaluation plan, and timeline.

**Deliverables:** Completed proposal template (pass/fail)

---

### Assignment 5 — Evaluation (Week 5: Observability + Evals)

`assignment_5/`

Evaluate your agent with three types of LLM judges:
1. **Built-in judge** — `RelevanceToQuery` scorer for baseline quality
2. **Guidelines judges** — custom rules for tool citation and data grounding
3. **Custom judge** — `make_judge()` with a template prompt evaluating tool usage appropriateness
4. **Combined evaluation** — run all judges together, compare pass/fail rates, and analyze where they agree and disagree

Create an evaluation dataset with 8+ provided questions and 5 of your own.

**Deliverables:** Executed notebook, submission template

---

### Assignment 6 — Human Feedback + Judge Alignment (Week 6: Human-in-the-Loop)

`assignment_6/`

Close the loop with human feedback:
1. **Generate 15 traces** — run the agent with MLflow tracing enabled
2. **Review and rate** — role-play as a domain expert, review each trace, and log feedback programmatically via `mlflow.log_feedback()`
3. **Run `align()`** — use MLflow's SIMBA optimizer to improve the custom judge based on your expert feedback
4. **Compare** — evaluate original vs. aligned judge and reflect on what changed
5. **Bonus:** Attempt deploying the agent to a serving endpoint

**Deliverables:** Executed notebook, submission template

---

### Weeks 7–8 — Final Project

No new assignments. Students work on and present their final projects.

## Repository Structure

```
assignment_1/
├── AAI_594_Assignment_1_Lab.ipynb
└── SUBMISSION_1.md

assignment_2/
├── AAI_594_Assignment_2_Lab.ipynb
└── SUBMISSION_2.md

assignment_3/
├── AAI_594_Assignment_3_Lab.ipynb
└── SUBMISSION_3.md

assignment_4/
├── AAI_594_Assignment_4a_Lab.ipynb
├── SUBMISSION_4a.md
└── PROPOSAL_4b.md

assignment_5/
├── AAI_594_Assignment_5_Lab.ipynb
└── SUBMISSION_5.md

assignment_6/
├── AAI_594_Assignment_6_Lab.ipynb
└── SUBMISSION_6.md
```

## Reading List

| Week | Readings |
|------|----------|
| 1 | [Building Effective Agents](https://www.anthropic.com/engineering/building-effective-agents) -- [Emergent Hierarchical Reasoning](https://arxiv.org/pdf/2509.03646) |
| 2 | [DeepSeek R1](https://arxiv.org/abs/2501.12948) -- [Why Reasoning Models Will Generalize](https://www.interconnects.ai/p/why-reasoning-models-will-generalize) |
| 3 | [Practical Guide for Agentic AI Workflows](https://arxiv.org/pdf/2512.08769) -- [MCP Architecture](https://modelcontextprotocol.io/docs/learn/architecture) |
| 4 | [GEPA DSPy Optimization](https://arxiv.org/pdf/2507.19457) -- [Everything is Context](https://www.arxiv.org/pdf/2512.05470) |
| 5 | [Product Evals in Three Steps](https://eugeneyan.com/writing/product-evals/) -- [Survey on Evaluation of LLM-based Agents](https://arxiv.org/pdf/2503.16416) -- [LLM Evals FAQ](https://hamel.dev/blog/posts/evals-faq/) |
| 6 | [Who Validates the Validators](https://arxiv.org/abs/2404.12272) -- [What is A2A](https://a2a-protocol.org/latest/topics/what-is-a2a/) |
| 7 | [Pragmatic Vision for Interpretability](https://www.alignmentforum.org/posts/StENzDcD3kpfGJssR/a-pragmatic-vision-for-interpretability) -- [Towards Monosemanticity](https://transformer-circuits.pub/2023/monosemantic-features) -- [Scaling Monosemanticity](https://transformer-circuits.pub/2024/scaling-monosemanticity/) |
