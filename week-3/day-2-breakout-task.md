**Goal:** Contrast `this` in different contexts and round‑trip JSON safely.

## Steps

1. Create `context.js`:
   - Build an object with a method that logs `this.name`.
   - Add an **arrow** method and observe the difference.
2. Create `json.js`:
   - `const text = '{"title":"Codex","year":2025}'`; parse with `try/catch`.
   - Stringify the result with `JSON.stringify(obj, null, 2)` and log it.
3. Commit after each file; push to `w3-d2-this-json`.
