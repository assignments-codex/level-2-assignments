**Theme:** DOM basics; `getElementById`, `querySelector`; events & `preventDefault`; JSON review
**Style:** Live‑code minimal HTML and wire up JS for selection, events, and render.

## Learning Goals

- Select and update elements with `getElementById`/`querySelector`.
- Attach event listeners; call `event.preventDefault()` to stop default form navigation.
- Parse JSON from a text area and render a simple list into the DOM.

## Live‑Coding Demo Checklist

- Minimal page: a form with a text area (JSON) and a result `<ul>`.
- On submit: `preventDefault()`, parse JSON in try/catch, update the list.
- Use both selection APIs; show textContent vs innerHTML safety considerations.

## Common Pitfalls

- Forgetting to return false/prevent default; crashing on bad JSON without try/catch.
- Over‑using `innerHTML` for rendering (XSS risk). Prefer `textContent` and `createElement`.

## Assessment

**Day 3 - Graded In‑Class Assignment: DOM + JSON Render.**
Students build a tiny “JSON to list” tool using selection APIs, events, and error handling.
(See assignment sheet.)
