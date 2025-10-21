**Goal:** Call an AI provider and a Weather API in Postman, using variables for keys and URLs.

## Steps

1. Pick one AI provider and one weather endpoint. Examples: **Google Gemini**, **Hugging Face Inference API**, **Cloudflare Workers AI** (POST), and **OpenWeather/WeatherAPI** (GET).
2. Create environment variables: `api_key`, `account_id` (if needed), and `base_url` for each provider. Do **not** commit keys anywhere public.
3. Build a minimal **POST** to the AI provider (a short prompt in JSON) and a **GET** to the weather endpoint (city query param). Send and review **response shape** for both.
4. Add short notes in Postman (description fields): required headers, body structure, and how query parameters differ across APIs.

**Deliverable:** Public repo `w5-d2-ai-weather` with `POSTMAN.md` summarizing both calls and differences (no keys).
