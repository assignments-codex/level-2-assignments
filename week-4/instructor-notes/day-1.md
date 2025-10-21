**Theme:** Styling frameworks overview (Bootstrap/Bootswatch) -> Tailwind setup -> utility‑first basics
**Style:** Virtual class; short comparison, then spend most time in Tailwind.

## Learning Goals

- Clarify _why_ teams use frameworks; compare component vs. utility approaches.
- Set up **Tailwind via CDN** and apply first utilities.
- Practice class stacking and small, incremental changes.

## Live‑Coding Demo Checklist

- Quick tour: Bootstrap button and a Bootswatch theme swap (2–3 minutes, just to show the idea).
- Create `index.html`; add Tailwind via CDN; show a sample utility stack on a card:
  ```html
  <div class="max-w-md mx-auto p-6 rounded-lg shadow bg-white">
    <h1 class="text-2xl font-semibold mb-2">Hello Tailwind</h1>
    <p class="text-slate-600">Utility‑first styling in minutes.</p>
    <button
      class="mt-4 px-4 py-2 rounded bg-indigo-600 text-white hover:bg-indigo-700"
    >
      Action
    </button>
  </div>
  ```
- Explain responsive _class prefixes_ (e.g., `md:`, `lg:`) and how they override base classes.

## Common Pitfalls

- Duplicating classes that fight each other; unreadable long class lines (encourage grouping logically).
- Forgetting that responsive variants add on top of base styles.

## Optional Extensions

- Show `container` + `max-w-*` + `space-*` utilities to structure sections quickly.

### Breakout (Student Task)

Students complete **Day 1 Breakout Task – Frameworks overview -> Tailwind setup** .
