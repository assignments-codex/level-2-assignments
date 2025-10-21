**Theme:** `this` keyword; JSON parse/stringify
**Style:** Live‑code tiny examples to contrast `this` bindings; keep JSON examples practical.

## Learning Goals

- Explain how `this` changes in **method**, **stand‑alone function**, **constructor**, and **arrow** contexts.
- Parse JSON strings into objects and stringify objects with spacing; handle bad JSON safely.

## Live‑Coding Demo Checklist

- Object method vs arrow in a method:
  ```js
  const user = {
    name: "Lin",
    say() {
      console.log(this.name);
    }, // 'Lin'
    sayArrow: () => console.log(this && this.name), // likely undefined in modules
  };
  user.say();
  user.sayArrow();
  ```
- Constructor pattern vs plain function call (`new` vs missing `new`).
- JSON round‑trip with error handling:
  ```js
  try {
    const obj = JSON.parse('{"ok":true}');
    console.log(JSON.stringify(obj, null, 2));
  } catch (e) {
    console.error("Invalid JSON");
  }
  ```

## Common Pitfalls

- Expecting arrow functions to have their own `this`.
- Confusing JSON with JS objects (quotes around keys/strings).

## Optional Extensions

- `JSON.stringify(obj, replacer, space)` with a replacer array or function.

### Breakout (Student Task)

Learners complete **Day 2 Breakout Task - `this` & JSON Drills** .
