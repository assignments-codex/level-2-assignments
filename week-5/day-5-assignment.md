**Goal:** Practice a reusable API workflow with a GET call, a POST call, and safe rendering.

## Steps

1. Create `index.html` and `script.js`. Include a simple output area for messages/results. Trigger your code with a button or on page load.
2. Write:
   - one GET request function (async/await, checks `response.ok`, parses JSON)
   - one POST request function (async/await, checks `response.ok`, parses JSON)
   - one render function that outputs a few fields using element creation + `textContent`
3. Use one public GET endpoint (no key), example:
   - https://swapi.dev/api/people/1/ Display a few fields.
4. Use one POST endpoint, example:
   - https://jsonplaceholder.typicode.com/posts Display the returned id plus one other field.
5. Include a `main()` that calls your functions (and wires events if you use a button).
6. If you use an API key, do not commit it:
   - local testing: `const API_KEY = "your-real-key-here"`
   - before pushing: `const API_KEY = "YOUR_API_KEY_HERE"`

**Deliverable:** Public repo with `index.html`, `script.js`, and a short `README.md` listing:

- GET endpoint used
- POST endpoint used
- fields you displayed
- how to set API\_KEY locally (only if you used a key)

**ACP:** Commit as you add features.

## Rubric (20 pts)

- GET function design (0-5): Uses async/await, checks `response.ok`, parses JSON correctly.
- POST function design (0-5): Uses async/await, checks `response.ok`, parses JSON correctly.
- Rendering safety (0-5): Uses element creation + `textContent` (no raw `innerHTML` injection).
- Clarity + ACP (0-5): Small readable functions, good naming, sensible commit history.
