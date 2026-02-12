# AAI 594 — Assignment 1 Submission

**Name:**  
**Date:**

> **Setup:** Create a `screenshots/` folder in the same directory as this file. Save your screenshot images there and reference them by filename (e.g. `screenshots/cli_workspace_list.png`). Your submission folder should look like:
>
> ```
> assignment_1/
> ├── AAI_594_Assignment_1_Lab.ipynb   ← executed notebook with outputs
> ├── SUBMISSION_1.md                  ← this file
> └── screenshots/
>     ├── cli_workspace_list.png       ← Section 6 (required)
>     ├── cursor_databricks_connect.png← Section 7 (if completed)
>     └── external_endpoint.png        ← Section 8 (if completed)
> ```

---

## Required (Sections 1–6)

### Sections 1–5: Notebook

Submit your executed notebook (`.ipynb` with cell outputs or HTML export) alongside this file. The notebook outputs serve as evidence for:

- [ ] Dataset downloaded and loaded (Section 2)
- [ ] Unity Catalog table `main.default.assignment_file` created (Section 3)
- [ ] Delta table written and exploration cell shows rows + schema (Section 4)
- [ ] Foundation Model demo returned an LLM response (Section 5)
- [ ] Ran the "Try it yourself" exploration cell (SQL query, schema, row count)

### Section 6: Databricks CLI

Paste a screenshot of your terminal showing the output of `databricks workspace list /` (proves the CLI is installed and authenticated).

<!-- Replace the placeholder below with your screenshot -->
![Databricks CLI workspace list](screenshots/cli_workspace_list.png)

---

## Optional but Strongly Encouraged (Sections 7–8)

### Section 7: Cursor + Databricks Connect

Paste a screenshot of Cursor with the Databricks extension connected (e.g. the extension panel showing your workspace, or a successful Databricks Connect query result).

<!-- Replace the placeholder below with your screenshot, or delete this section if skipped -->
![Cursor Databricks extension](screenshots/cursor_databricks_connect.png)

### Section 8: External Model Endpoint

Paste a screenshot showing **one** of the following:

- The endpoint in **Ready** state in the Databricks Serving UI, **or**
- The `predict()` response output in a notebook or terminal

<!-- Replace the placeholder below with your screenshot, or delete this section if skipped -->
![External model endpoint](screenshots/external_endpoint.png)

---

## Notes (optional)

Add any notes, issues you ran into, or things you tried here.
