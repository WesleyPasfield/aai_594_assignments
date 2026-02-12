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
- [ ] **Section 6.2:** Vector Search endpoint created successfully.
- [ ] **Section 6.3:** Delta Sync Index created and synced.
- [ ] **Section 6.4:** Similarity search queries returned results.
- [ ] **Section 6.5:** Endpoint and index **deleted** — cleanup cell ran successfully.

### 2. MCP Configuration (Required)

- [ ] **Section 7:** You.com MCP server configured in Cursor.

**Screenshot — MCP tool in use:**

![You.com MCP tool being used in Cursor Agent chat](screenshots/mcp_you_com.png)

### 3. Agent Skill (Optional, strongly encouraged)

- [ ] **Section 8:** `SKILL.md` created and included in submission folder.

---

## Short-answer Questions

### Q1: When should an agent use a SQL UC function vs. a Python UC function vs. Vector Search?

*Write your answer below (2-3 sentences):*

**[Your answer here]**

### Q2: Why did we delete the Vector Search endpoint after testing?

*Write your answer below (1-2 sentences):*

**[Your answer here]**

### Q3: How does adding an MCP server (like You.com) extend what an agent can do beyond UC functions and Vector Search?

*Write your answer below (2-3 sentences):*

**[Your answer here]**

---

## Grading Rubric

### Criterion 1: UC Function Tools (30%)

*Did the student create, document, and test UC functions correctly?*

| Meets or Exceeds Expectations | Approaches Expectations | Below Expectations | Inadequate Attempt |
|---|---|---|---|
| All three UC functions (SQL, Python, and student-created) are registered, have clear COMMENTs/docstrings, and produce correct test output. Student's custom function is original and useful for the UltraFeedback Expert agent. Code cells show outputs. | Two functions work correctly with reasonable documentation. Student's custom function is present but may have weak documentation or limited utility. | Only the provided functions work; student's custom function is missing or broken. COMMENTs/docstrings are vague or missing. | Little to no evidence of creating UC functions. Notebook cells are not executed. |

### Criterion 2: Vector Search (25%)

*Did the student successfully create, query, and clean up a Vector Search index?*

| Meets or Exceeds Expectations | Approaches Expectations | Below Expectations | Inadequate Attempt |
|---|---|---|---|
| Source table prepared correctly, endpoint and index created, similarity queries return relevant results. Student tried at least two different queries. Cleanup cell confirms endpoint and index are deleted. | Endpoint and index created; at least one query returned results. Cleanup was attempted. Minor issues (e.g., index still syncing in output). | Endpoint created but index creation failed or was not completed. Limited or no query results. Cleanup not confirmed. | No evidence of Vector Search work. |

### Criterion 3: External MCP Configuration (20%)

*Did the student configure and test an external MCP server?*

| Meets or Exceeds Expectations | Approaches Expectations | Below Expectations | Inadequate Attempt |
|---|---|---|---|
| You.com MCP configured in Cursor and tested. Screenshot shows the agent calling the MCP tool with visible results. Student's short-answer (Q3) demonstrates understanding of how MCP extends agent capabilities. | MCP configured and screenshot provided, but test results are minimal or Q3 answer is surface-level. | MCP configuration attempted but not working (no screenshot of successful tool use). | No MCP configuration attempted. |

### Criterion 4: Understanding and Reflection (15%)

*Do the short-answer questions show understanding of when and why to use different tool types?*

| Meets or Exceeds Expectations | Approaches Expectations | Below Expectations | Inadequate Attempt |
|---|---|---|---|
| All three short-answer questions are thoughtful and accurate. Student clearly distinguishes between SQL/Python/VS/MCP tool types and explains their trade-offs. Connects to course concepts (agentic workflows, tool selection). | Answers are present and mostly accurate but lack depth or specificity. May conflate tool types or miss key distinctions. | Answers are brief or inaccurate. Missing answers for one or more questions. | Short-answer section is empty or contains only placeholder text. |

### Criterion 5: Notebook Quality (10%)

*Is the notebook well-organized, complete, and shows all outputs?*

| Meets or Exceeds Expectations | Approaches Expectations | Below Expectations | Inadequate Attempt |
|---|---|---|---|
| All cells executed with visible outputs. Code is clean with helpful comments. Student's custom function cell is well-organized. Cleanup is confirmed. | Most cells executed. Minor issues with output visibility or organization. | Significant cells missing output. Notebook is disorganized or hard to follow. | Notebook not executed or missing major sections. |

---

## Notes (optional)

Add any notes, issues you ran into, or things you tried here.
