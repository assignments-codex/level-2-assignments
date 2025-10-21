**Theme:** Visualize APIs in Postman, then mirror a simple GET in code
**Emphasis:** Postman is a _visual primer_; the goal is **writing JS that consumes APIs**.

## Learning Goals

- Build the mental model: HTTP method -> URL (path vs query) -> headers -> body -> JSON response.
- Show that **APIs differ** (param names, response shapes, status codes).
- Use Postman (app, web, or VS Code extension) to probe endpoints, then replicate the same request with `fetch`.

## Live‑Coding Demo Checklist

- Quick Postman setup (extension optional). Create 3 GETs that **differ in how input is passed**:
  1. **Path param:** `https://pokeapi.co/api/v2/pokemon/pikachu`
  2. **Query param:** `https://openlibrary.org/search.json?q=harry+potter`
  3. **Compound query:** `https://api.github.com/search/repositories?q=react+language:JavaScript&sort=stars&order=desc`
- For each, note: _where_ the input goes (path vs `?q=`), _shape_ of the response (e.g., `docs/items`), and any rate limits.
- Translate one request to code (live): minimal `fetch(url) -> if (!res.ok) throw … -> res.json()` and log a field.

## Common Pitfalls

- Assuming `q` is universal; not all APIs use the same param names.
- Parsing without checking `res.ok` first.

## Optional Extensions

- Postman variables/environments only to reduce typing-keep it light this week.

### Breakout

Students complete **Day 1 Breakout – Postman Request Patterns** .
