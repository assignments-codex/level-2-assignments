**Week‑7 focus:** **Inheritance, methods, `super`**; prefer composition for cross‑cutting concerns.
**Review anchor:** Week‑2/4 UI fundamentals (keep the output simple, accessible).

**Teach**

- `extends` + `super` basics; override a method.
- Service layering: `ApiService` -> `WeatherService` (URL builder, `normalize(json)`).
- Composition example: inject a `Cache`/`Formatter` helper instead of deep inheritance.

**Breakout - Services & Inheritance**

- Implement a base `ApiService` plus TWO children (e.g., PokeAPI + OpenLibrary) with `buildUrl`, `request`, `normalize`. Console‑demo both.
