**Goal:** Build a small weather app using a service class and minimal UI states.

## Steps

1. Create `index.html` with an input for a city, a button, and a results area. Link `app.js`.
2. Implement `WeatherService` with:
   - `buildUrl(city)`
   - a guarded `request` (checks `response.ok`, handles network/JSON errors)
   - `normalize(json) -> { city, temp, description }`
3. On submit: prevent default, show a loading message, call the service, and render normalized fields with `textContent`.
4. Handle one error path (bad city or network) with a readable message.

**Deliverable:** Public repo `w7-d3-weather-app`.

## Rubric (20 pts)

- **Service & Model** (0–5): Clear `WeatherService` design; correct `buildUrl`, guarded `request`, and `normalize`.
- **UI & DOM** (0–5): Minimal, accessible UI; renders `{ city, temp, description }` with `textContent`.
- **States & Errors** (0–5): Loading shown; friendly error for bad city/network; no crashes on bad JSON.
- **Clarity & ACP** (0–5): Small, well-named functions; brief README; incremental commits.
