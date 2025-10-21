Build and demo a basic site layout using a styling framework (e.g., Bootstrap or Tailwind). Include a header, a footer, and one component chosen by your instructor (carousel, form, image/gallery, or accordion). Keep it simple so the full demo fits in 5–10 minutes.

Time
5–10 minutes

Submission
Meet with a TA or Instructor to demonstrate the items below. After the interview, submit your repo link and live site URL in the LMS.

What to prepare

- A small starter repo with your chosen framework loaded by CDN
- A deployed link (e.g., GitHub Pages)
- (Optional) Have the single doc snippet you’ll use open so you do not hunt through docs

Interview flow

1. Include the framework

   - Show the exact CDN snippet you used from the docs.
   - Prove it loaded by adding one obvious utility class (spacing or color).

2. Layout structure

   - Create `index.html` with semantic `header`, `main`, and `footer`.
   - Header: site name/brand and a simple nav (links can be placeholders).
   - Footer: small text or links.

3. Instructor-chosen component (pick one; keep it minimal)

   - **Carousel**: 2–3 slides with next/prev controls or auto-slide; no custom styling beyond utilities.
   - **Form**: label + input + button with required/validation styling.
   - **Image/Gallery**: one responsive image or a small 2–4 image grid with proper `alt`.
   - **Accordion**: two collapsible sections using framework classes or a tiny JS toggle.
   - Point to the exact snippet you used (do not browse docs extensively).

4. Responsiveness

   - Demonstrate one breakpoint change (e.g., stacked on mobile -> horizontal at `md`).
   - Name the utility classes that enable the change.

5. Live coding (chosen by TA/Instructor)
   - Add a small spacing or color utility.
   - Adjust a breakpoint on a layout section.
   - Add an accessibility touch (e.g., `aria-expanded` on accordion button or proper `<label for>` on a form field).
   - Commit the change with a clear message.

Rubric (20 pts)

- **Framework usage** (0–5): Correct CDN include; documented utilities/components used; choices explained briefly.
- **Layout & component** (0–5): Header, main, footer present; chosen component works with a minimal, focused setup.
- **Responsiveness & a11y** (0–5): Clear breakpoint behavior; basic accessibility (labels/alt/aria) shown.
- **Clarity & ACP** (0–5): Clean HTML; small, meaningful commits; deployed link works; clear, concise demo.

Deliverables (after the interview)

- Public repo link
- Live site URL
