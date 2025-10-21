**Goal:** Send a request in JavaScript, show a few fields on the page, and keep any API key out of your public repo.

## Steps

1. Create `index.html` and `script.js`. Add a simple page with a button, an input if needed, and a results area.
2. Write a small `fetchJson(url, options)` helper that:
   - uses `async/await`
   - checks `response.ok` and throws an error with the status if it is not ok
   - catches JSON parse errors
   - shows a short "loading" message and a clear error message on the page
3. Call one public endpoint and render a few fields using `textContent`. Keep it small and readable.
4. If the API needs a key:
   - While testing locally, set a variable like `const API_KEY = "your-real-key-here"`.
   - Before pushing to GitHub, change it to `const API_KEY = "YOUR_API_KEY_HERE"`.
   - Do not include screenshots or code that show your real key.
   - In your `README.md`, add a short note telling the grader how to paste their own key into `API_KEY` to run your page.
5. Trigger one error on purpose (for example, a bad query or empty input) and show a friendly message on the page.

**Deliverable:** Public repo `w5-d4-js-apis-keys` with `index.html`, `script.js`, and a short `README.md` that lists:

- the endpoint you used
- the fields you displayed
- how to set `API_KEY` locally before testing
