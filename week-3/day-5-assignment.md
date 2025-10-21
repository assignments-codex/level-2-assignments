## Objective

Demonstrate constructor vs factory, prototype methods, and a simple inheritance chain in one tiny domain model.

## Scope

1. **Constructor Function** – e.g., `function Animal(name){...}`; set at least two properties.
2. **Factory Function** – returns a plain object with similar shape.
3. **Prototype Method** – add at least one method on the constructor’s **prototype** and call it from an instance.
4. **Inheritance** – create a subtype (e.g., `Dog`) via `Object.create`, reset `constructor`, and override one method.

## ACP Expectations

Commit for each scope item; final commit message: `build: finish mini‑build`.

## Rubric (20 pts)

- **Constructor vs Factory** (0–5) - Both implemented correctly, differences clear.
- **Prototype Method** (0–5) - Shared behavior on the prototype works.
- **Inheritance** (0–5) - Subtype created, method override verified.
- **Clarity & ACP** (0–5) - Readable code and sensible commit log.
