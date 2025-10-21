**Goal:** Add robust error handling around one real API call using `try/catch/finally` and `res.ok` checks.

## Steps

1. Create `index.html` and `script.js`.
2. Write a small `fetchJson(url, options)` helper that:
   - Uses `async/await`.
   - Checks `response.ok`; if false, throws an error with status + snippet.
   - Wraps `await response.json()` in `try/catch` to guard invalid JSON.
   - Shows a loading message and a readable error message in the UI.
3. Call a public endpoint of your choice (e.g., posts, users, or similar). Render 3–5 fields with `textContent`.
4. Trigger one controlled error (bad param or URL) and verify the message is helpful.

**Deliverable:** Public repo `w6-d1-error-handling`.

---
