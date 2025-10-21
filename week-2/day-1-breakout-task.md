**Goal:** Build a semantic HTML page that demonstrates default browser styles vs custom CSS and the CSS box model.

## Steps

1. Create `index.html` with semantic regions: `header` (with `nav` links), `main` with **three** `section` blocks (each with an `h2` + `p`), and a `footer`.
2. In one section, add a `<pre>` element showing multi‑line, spaced text.
3. Add a `<div class="box-demo">` and a `styles.css` file. Style it to make the **box model** visible:

   ```css
   .box-demo {
     width: 240px;
     height: 120px;
     padding: 12px;
     border: 2px solid #333;
     margin: 16px auto;
   }
   ```

4. Compare **user‑agent styles** to your **custom styles** by changing default paragraph font size/color and noting the difference.

**Deliverable (practice):** Push to a public repo named `w2-d1-structure-box-model` and (optionally) enable GitHub Pages.
