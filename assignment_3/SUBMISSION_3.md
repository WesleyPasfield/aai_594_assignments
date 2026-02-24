# AAI 594 — Assignment 3 Submission

**Name:**  
**Date:**

> **Setup:** Create a `screenshots/` folder in the same directory as this file. Save your screenshot images there and reference them by filename. Your submission folder should look like:
>
> ```
> assignment_3/
> ├── AAI_594_Assignment_3_Lab.ipynb   ← executed notebook with all outputs
> ├── SUBMISSION_3.md                  ← this file
> ├── SKILL.md                         ← bonus: agent skill (if completed)
> └── screenshots/
>     ├── mcp_you_com.png              ← Section 7 (required)
>     └── skill_in_cursor.png          ← Section 8 (if completed)
> ```

---

## Deliverables

### 1. Executed Notebook

Submit your executed notebook (`.ipynb` with cell outputs) alongside this file. The notebook should include:

- [ ] **Section 3:** Dataset verification cell ran successfully (row count, columns, schema).
- [ ] **Section 4.1:** SQL function `lookup_source_info` created and tested with output visible.
- [ ] **Section 4.2:** Python function `analyze_instruction` created and tested with output visible.
- [ ] **Section 4.3:** Your own UC function created and tested with output visible.
- [ ] **Section 5:** `SHOW USER FUNCTIONS` output listing all registered functions.
- [ ] **Section 6.1:** Embeddings source table created with 100 unique instructions.
- [ ] **Section 6.2:** Embeddings computed and saved to Delta table.
- [ ] **Section 6.3:** SQL search function `search_similar_instructions` created.
- [ ] **Section 6.4:** Search queries returned relevant results.

### 2. MCP Configuration (Required)

- [ ] **Section 7:** You.com MCP server installed from Databricks Marketplace and tested in AI Playground.

**Screenshot — MCP tool in use:**

![You.com MCP tool being used in Databricks AI Playground](screenshots/mcp_you_com.png)

### 3. Agent Skill (Optional, strongly encouraged)

- [ ] **Section 8:** `SKILL.md` created and included in submission folder.

---

## Short-answer Questions

### Q1: When should an agent use a SQL UC function vs. a Python UC function vs. an external MCP tool?

*Write your answer below (2-3 sentences):*

**[Your answer here]**

### Q2: What are the trade-offs of keyword-based search (LIKE matching) vs. embedding-based semantic search for an agent tool?

*Write your answer below (2-3 sentences):*

**[Your answer here]**

### Q3: How does adding an MCP server (like You.com) extend what an agent can do beyond UC functions?

*Write your answer below (2-3 sentences):*

**[Your answer here]**

---

## Grading Rubric

### Criterion 1: UC Function Tools (30%)

*Did the student create, document, and test UC functions correctly?*

| Meets or Exceeds Expectations | Approaches Expectations | Below Expectations | Inadequate Attempt |
|---|---|---|---|
| All three UC functions (SQL, Python, and student-created) are registered, have clear COMMENTs/docstrings, and produce correct test output. Student's custom function is original and useful for the UltraFeedback Expert agent. Code cells show outputs. | Two functions work correctly with reasonable documentation. Student's custom function is present but may have weak documentation or limited utility. | Only the provided functions work; student's custom function is missing or broken. COMMENTs/docstrings are vague or missing. | Little to no evidence of creating UC functions. Notebook cells are not executed. |

### Criterion 2: Semantic Search with Embeddings (25%)

*Did the student compute embeddings, create the search function, and test it?*

| Meets or Exceeds Expectations | Approaches Expectations | Below Expectations | Inadequate Attempt |
|---|---|---|---|
| Embeddings source table created with 100 instructions. Embeddings computed and saved to Delta table. SQL search function registered and tested with at least two different queries returning relevant results. | Embeddings table created and search function registered. At least one query returned results. Minor issues (e.g., incomplete embedding run). | Embeddings table created but search function is missing or broken. Limited or no query results. | No evidence of embeddings or search work. |

### Criterion 3: External MCP Configuration (20%)

*Did the student install and test an external MCP server in Databricks?*

| Meets or Exceeds Expectations | Approaches Expectations | Below Expectations | Inadequate Attempt |
|---|---|---|---|
| You.com MCP installed from Databricks Marketplace and tested in AI Playground. Screenshot shows the agent calling the MCP tool with visible results. Student's short-answer (Q3) demonstrates understanding of how MCP extends agent capabilities. | MCP installed and screenshot provided, but test results are minimal or Q3 answer is surface-level. | MCP installation attempted but not working (no screenshot of successful tool use). | No MCP configuration attempted. |

### Criterion 4: Understanding and Reflection (15%)

*Do the short-answer questions show understanding of when and why to use different tool types?*

| Meets or Exceeds Expectations | Approaches Expectations | Below Expectations | Inadequate Attempt |
|---|---|---|---|
| All three short-answer questions are thoughtful and accurate. Student clearly distinguishes between SQL/Python/MCP tool types and explains their trade-offs. Connects to course concepts (agentic workflows, tool selection). | Answers are present and mostly accurate but lack depth or specificity. May conflate tool types or miss key distinctions. | Answers are brief or inaccurate. Missing answers for one or more questions. | Short-answer section is empty or contains only placeholder text. |

### Criterion 5: Notebook Quality (10%)

*Is the notebook well-organized, complete, and shows all outputs?*

| Meets or Exceeds Expectations | Approaches Expectations | Below Expectations | Inadequate Attempt |
|---|---|---|---|
| All cells executed with visible outputs. Code is clean with helpful comments. Student's custom function cell is well-organized. | Most cells executed. Minor issues with output visibility or organization. | Significant cells missing output. Notebook is disorganized or hard to follow. | Notebook not executed or missing major sections. |

---

## Notes (optional)

Add any notes, issues you ran into, or things you tried here.
