**Goal:** Build a tiny list that loads paged results and handles rate-limit feedback.

## Approved APIs (pick one)

- PokéAPI — /pokemon?offset=0&limit=10
- SWAPI — /people/?page=1
- OpenLibrary — /search.json?q=javascript&page=1
- Rick and Morty API — /character/?page=1
- GitHub Search — /search/repositories?q=react&page=1&per_page=10

## Steps

1. Create `index.html` and `app.js`. Add Next and Prev buttons and a small results area.
2. Fetch page 1 on load. Show a loading message while fetching.
3. On Next and Prev, update the current page and reload results.
4. Render 5–10 rows using `textContent`. Also display the current page number and total items if the API provides it.
5. Handle a rate-limit or error path:
   - If you receive a 429 or a rate-limited 403, show a friendly message and disable the buttons briefly.
   - Log any helpful headers (for example, remaining requests) if available.
6. Keep functions small and well named. Commit after each feature.

**Deliverable:** Public repo `w6-d3-pagination-mini-app` with your code and a brief `README.md` (API chosen, parameters used, any rate-limit headers you observed).

## Rubric (20 pts)

- **Pagination mechanics** (0–5): Next/Prev work; current page is tracked and shown; loads correct data.
- **Render & UX** (0–5): 5–10 rows rendered with `textContent`; loading message present; layout is clear.
- **Rate-limit/error handling** (0–5): Friendly error message; buttons disabled briefly; relevant headers logged if available.
- **Clarity & ACP** (0–5): Small, readable functions; brief README; incremental commits.
