Call one approved public API and render a single field on the page. Keep it simple so the full demo fits in 5–10 minutes.

Time
5–10 minutes

Submission
Meet with a TA or Instructor to demonstrate the items below. After the interview, submit your repo link and live site URL in the LMS.

Approved API choices (pick one)

- SWAPI: `https://swapi.dev/api/people/1/` -> render the character name
- PokéAPI: `https://pokeapi.co/api/v2/pokemon/pikachu` -> render the pokemon name
- OpenLibrary: `https://openlibrary.org/search.json?q=harry+potter` -> render the first book title

Interview flow

1. Setup

   - Open a small repo with `index.html` and `app.js` (deployed on GitHub Pages).
   - Show the exact endpoint you will call.

2. Fetch and render

   - Write a minimal `fetchJson(url)` that uses `async/await`, checks `response.ok`, and handles JSON parse errors.
   - Call the chosen endpoint and render one field with `textContent`:
     - SWAPI: `data.name`
     - PokéAPI: `data.name`
     - OpenLibrary: `data.docs[0].title` (guard if `docs` is empty)

3. Error state

   - Trigger one error (bad ID or query) and show a friendly message instead of crashing.

4. Live coding (chosen by TA/Instructor)
   - Change the ID/name/query and re-fetch.
   - Add one small UI touch (e.g., “Loading…” text before the request, then clear it).
   - Commit with a clear message.

Rubric (20 pts)

- **API call** (0–5): Correct endpoint; `fetch` with `async/await`; guards `response.ok` and JSON parse.
- **Render** (0–5): One field displayed with `textContent`; layout remains simple and readable.
- **Error handling** (0–5): Friendly message on failure; app does not crash on a bad query/ID.
- **Clarity & ACP** (0–5): Small, well-named functions; deployed link works; brief README; incremental commits.

Deliverables (after the interview)

- Public repo link
- Live site URL
