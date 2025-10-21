**Goal:** Practice ACP for each feature and keep commits small and clear.

## Steps

1. Create a new repo: `simple-web-page`.
2. Add `index.html` with base HTML.
3. Add these features, **one commit each**:
   - `Add header`
   - `Add paragraph`
   - `Add basic styles` (inline `<style>` is fine)
4. Push to GitHub and share your link in chat.

```bash
mkdir simple-web-page && cd simple-web-page
git init
echo '<!doctype html><html lang="en"><head><meta charset="utf-8"><title>Simple</title></head><body></body></html>' > index.html
git add index.html
git commit -m "feat: base HTML"


printf '<h1>Welcome</h1>\n' >> index.html
git add index.html
git commit -m "feat: add header"


printf '<p>This is a tiny page to practice ACP.</p>\n' >> index.html
git add index.html
git commit -m "feat: add paragraph"


cat >> index.html <<'HTML'
<style>
  body { font-family: sans-serif; text-align: center; margin-top: 40px; }
</style>
HTML
git add index.html
git commit -m "style: add basic styles"

git branch -M main
git remote add origin https://github.com/<username>/simple-web-page.git
git push -u origin main
```
