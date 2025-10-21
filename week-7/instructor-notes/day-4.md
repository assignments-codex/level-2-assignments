**Week‑7 focus:** `localStorage` + **Chat UI** shell (model provider optional, Workers AI recommended).
**Review anchors:** Week‑5/6 API mechanics; add persistence & small guardrails.

**Teach**

- `ChatSession` class: `messages`, `addMessage`, `save/load`.
- `ChatService` stub: `send(prompt)` returns canned reply (swap to real model if ready).
- Guardrails: short‑circuit obvious off‑topic prompts before network.
- Keep the UI minimal and keyboard‑friendly.

**Breakout - Chat UI + localStorage**

- Build the chat shell; persist messages; use a stubbed service or wire a real call if ready.
