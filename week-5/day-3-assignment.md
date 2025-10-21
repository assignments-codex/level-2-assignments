**Goal:** Use the Postman VS Code extension to replicate a request, then make the same request with JavaScript.

## Steps

1. Install **Postman** in VS Code (Extensions -> search “Postman”). Sign in if prompted. Recreate one request from Day 1 or Day 2.
2. In a new folder, add `index.html` and `script.js`. Write a minimal `fetch` **GET** to the same endpoint. Log the JSON. Add a quick `try/catch` and `res.ok` guard.
3. Read the API docs and add **one** query parameter or header from the documentation. Confirm it changes the response.
4. Keep it simple—no frameworks. Use `textContent` for any on-page output.

**Deliverable:** Public repo `w5-d3-postman-vscode-js` with the two files and a brief `README.md` (endpoint used, one note from docs).

## Rubric (20 pts)

- **JavaScript fetch implementation** (0–8): Correct GET; includes `res.ok` check and `try/catch`; JSON logged or shown.
- **Docs-driven change** (0–4): Adds exactly one parameter or header from docs; effect is demonstrated.
- **Output & safety** (0–4): Any on-page output uses `textContent`; minimal UI clear and functional.
- **Clarity & ACP** (0–4): README is brief and accurate; commits are incremental and meaningful.
