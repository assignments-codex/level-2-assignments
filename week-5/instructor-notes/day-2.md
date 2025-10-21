**Theme:** Convert requests explored in Postman into small JS utilities and a minimal UI

## Learning Goals

- Write `fetch` helpers for **path‑param** and **query‑param** styles.
- Handle errors and empty states.
- Render first N results safely (avoid raw `innerHTML` where possible).

## Live‑Coding Demo Checklist

- Build a tiny page with an input + select (`Which API?`).
- Implement two functions:
  ```js
  const getPokemon = (name) =>
    fetch(`https://pokeapi.co/api/v2/pokemon/${name}`);
  const searchBooks = (q) =>
    fetch(`https://openlibrary.org/search.json?q=${encodeURIComponent(q)}`);
  ```
- A shared `loadJson` helper that guards `res.ok` and wraps `try/catch`.
- Render list items with `textContent` to avoid injection.

## Common Pitfalls

- Forgetting `encodeURIComponent` for query strings.
- Assuming identical response shapes across APIs-normalize before rendering.

### Breakout

Students complete **Day 2 Breakout – Translate Two Postman GETs to `fetch`** .
