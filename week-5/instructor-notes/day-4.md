**Theme:** Error handling patterns; POST; optional “secure a key via a tiny proxy”

## Learning Goals

- Distinguish _network OK_ vs _JSON OK_ vs _app‑level_ errors.
- Do a simple POST with JSON headers.
- (Optional) Retrieve a key from a tiny proxy (Render) to avoid exposing secrets.

## Live‑Coding Demo Checklist

- Guard pattern:
  ```js
  async function load(url) {
    const res = await fetch(url);
    if (!res.ok) throw new Error("HTTP " + res.status);
    return res.json();
  }
  ```
- JSONPlaceholder POST demo; discuss common 4xx/5xx response handling.
- Show minimal proxy handshake (if time).

### Breakout

Students complete **Day 4 Breakout – Fetch drills + optional proxy** .
