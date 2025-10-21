## Objective

Build a small tool that takes JSON from a `<textarea>`, prevents the default form submit, parses it, and renders a list into the DOM.

## Requirements

1. **DOM Selection & Update** – Use `getElementById` **and** `querySelector` to select elements and update text/attributes safely.
2. **Event Handling** – Add a `submit` listener; call `event.preventDefault()`; do not reload the page.
3. **JSON Integration** – Parse user input with `try/catch`. On success, render a list of items; on failure, show a readable error.
4. **Render Safely** – Use `textContent` and element creation (not raw `innerHTML` injection).

## ACP Expectations

Commit after each requirement with clear messages.

## Rubric (20 pts)

- **DOM Selection & Update** (0–5) - Correct use of both APIs; visible updates.
- **Event Handling** (0–5) - Proper listener and `preventDefault` usage.
- **JSON Integration** (0–5) - Correct parse/stringify flow with error handling.
- **Code Quality & ACP** (0–5) - Clear structure, naming, and commit history.
