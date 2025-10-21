**Goal:** Finish and refine your chatbot with clear UX, persistence, and a correct AI request. Keep the design class‑driven.

## Steps

1. OOP design

   - Ensure `ChatSession` persists messages reliably (save/load/clear).
   - Ensure `ChatService` returns a short text reply from your chosen provider.

2. UX and safety

   - Show loading and error states.
   - Render with `textContent`. Provide a “clear chat” action.

3. AI request and keys

   - Follow the provider’s docs for endpoint, headers, and body.
   - Use a secure key approach approved by your instructor. Do not hard‑code secrets.

4. Review and polish
   - Keep functions small and well named.
   - Add a short `README.md` with how to run and which provider you used.

**Deliverable:** Public repo `w7-d5-chatbot-final` with your code and `README.md`.

## Rubric (20 pts)

- **OOP Design** (0–5): Clear class responsibilities; `ChatSession` and `ChatService` work together.
- **AI Request & Secure Handling** (0–5): Correct endpoint/headers/body; no secrets committed; approach documented.
- **UX & Persistence** (0–5): Loading/error states; safe rendering; messages persist; clear chat action.
- **Clarity & ACP** (0–5): Small functions; tidy repo; helpful README; incremental commits.
