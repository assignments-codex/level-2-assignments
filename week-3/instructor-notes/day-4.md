**Theme:** Promises; async/await; `fetch`; `setTimeout`
**Style:** Live‑code two async flows: a promise demo and a small `fetch` reader (JSONPlaceholder).

## Learning Goals

- Create and consume a Promise; convert `.then/.catch` into `async/await`.
- Use `fetch` to retrieve JSON; handle network/JSON errors distinctly.
- Use `setTimeout` for simple delay demos and to visualize the event loop.

## Live‑Coding Demo Checklist

- Promise -> async/await equivalence:
  ```js
  const p = new Promise((res) => setTimeout(() => res("done"), 500));
  p.then((v) => console.log(v));
  (async () => {
    console.log(await p);
  })();
  ```
- Fetch with guards:
  ```js
  async function loadUser(id) {
    const r = await fetch(`https://jsonplaceholder.typicode.com/users/${id}`);
    if (!r.ok) throw new Error("HTTP " + r.status);
    return r.json();
  }
  ```

## Common Pitfalls

- Forgetting `await`, swallowing errors, assuming `fetch` rejects on 404 (it doesn’t).

## Optional Extensions

- Add a loading state and a minimal retry button.

### Breakout (Student Task)

Learners complete **Day 4 Breakout Task - Async & Fetch Mini‑drills** .
