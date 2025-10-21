**Goal:** Build a minimal chatbot UI that persists messages and makes one request to an AI provider.

## Steps

1. Create `index.html` with a messages list, an input, and a send button. Link `app.js`.
2. Implement `ChatSession` with `messages = []`, `addMessage`, `save()`, and `load()` using `localStorage`.
3. Implement a small `ChatService.send(prompt)` that calls an AI provider such as **Google Gemini** or **Cloudflare Workers AI**. Use a secure approach for any key; do not commit secrets.
4. Wire the UI: on send -> add user message -> call service -> add reply -> save -> render. Use `textContent` for safety and show a loading state.
5. Add a simple off‑topic guard that replies locally without network when the question is clearly out of scope.

**Deliverable:** Public repo `w7-d4-chat-ui`.

_note: This will be a required assignment on day 5._
