**Goal:** Implement a base class and two child classes that specialize behavior, using `extends` and `super`.

## Steps

1. Create `ApiService` with a `request(url)` method (stub or real fetch) and a `buildUrl()` placeholder.
2. Implement two child services (choose any public APIs). Each child defines `buildUrl()` and a `normalize(json)` that returns a common shape (e.g., `{ title, extra }`).
3. Override one method in a child and call `super` within it.
4. Console‑demo both children with two calls total and log normalized outputs.

**Deliverable:** Public repo `w7-d2-inheritance`.
