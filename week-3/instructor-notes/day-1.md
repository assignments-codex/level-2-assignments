**Theme:** Variables, types, operators; objects & properties; dot vs bracket notation
**Style:** Virtual class; live‑code small, verifiable snippets learners can mirror quickly.

## Learning Goals

- Declare and mutate variables using `let`/`const` (avoid `var` except for contrast).
- Read/write primitive types and identify truthy/falsy values in conditionals.
- Create objects and access/update properties with **dot** and **bracket** notation (dynamic keys).

## Live‑Coding Demo Checklist

- Variables & types quick tour; show reassignment rules.
- Operators: arithmetic, comparison (`==` vs `===`), logical.
- Build a `person` object and access/mod properties via dot/bracket; demo a **dynamic key**:
  ```js
  const key = "firstName";
  const person = { firstName: "Ada", role: "Engineer" };
  console.log(person[key]); // Ada
  ```

## Common Pitfalls

- Using `==` instead of `===`; accidental global vars; mutating const objects vs. reassigning the binding.
- Misunderstanding bracket notation for spaces/dashes or dynamic keys.

## Optional Extensions

- Show object shorthand and computed properties:
  ```js
  const k = "score";
  const v = 42;
  const stats = { [k]: v }; // { score: 42 }
  ```

### Breakout (Student Task)

Learners complete **Day 1 Breakout Task - JS Basics & Objects** .
