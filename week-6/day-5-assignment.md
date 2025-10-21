**Goal:** Build a working **Postman** request to a free AI provider that could be reused in a JavaScript project. Examples of acceptable providers: **Google Gemini** or **Cloudflare Workers AI**.

## Steps

1. **Choose provider and read docs**

   - Identify the endpoint, required headers, model identifier, and request body shape.
   - Decide the **response field** that contains the returned text (e.g., `result.response` or provider equivalent).

2. **Set up variables**

   - Use a Postman **environment** for anything secret or instance‑specific (e.g., `{{API_TOKEN}}`, `{{ACCOUNT_ID}}`, `{{MODEL_ID}}`, `{{BASE_URL}}`).
   - Do **not** commit real secrets. Mask/redact tokens in screenshots.

3. **Build the request in Postman**

   - Method and URL per the provider docs (usually `POST`).
   - Headers per docs (for example, `Authorization: Bearer {{API_TOKEN}}` and `Content-Type: application/json`).
   - Body: include a short prompt and any model parameters required by the provider.
   - Send and verify a **200 OK** with a valid response body.

4. **Document how JS would reuse it**

   - In `README.md`, include:
     - The endpoint and headers you used (with **variables**, not raw tokens).
     - A **JavaScript `fetch`** snippet that match your Postman request (use placeholders like `${API_TOKEN}`).
     - The **response field path** your JS would read for text output.

5. **Add screenshots to `README.md`**
   Include **all** of the following, with secrets masked:
   - Request overview showing **method + URL** and **Headers** tab.
   - **Body** tab content (prompt payload).
   - **Response** tab with the status code and the JSON showing the text field.
   - **Environment** view showing variable names (values masked or dummy).

**Deliverable:** Public repo `w6-d5-ai-postman` containing **README.md with screenshots** `fetch` snippet (placeholders only; no secrets).

## Rubric (20 pts)

- **Request Correctness** (0–5): Correct endpoint/headers/body per provider docs; valid response field identified.
- **Screenshots & Hygiene** (0–5): All required screenshots present; variables used; secrets masked; no exports needed.
- **Reusability for JS** (0–5): README includes a minimal `fetch` snippet that matches the Postman request.
- **Clarity & Organization** (0–5): Clean repo; clear instructions; meaningful commits.
