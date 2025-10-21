**Goal:** Practice the ACP loop and pushing to GitHub.

## Steps

1. Create a project folder and initialize Git.
2. Add an `index.html` and `.gitignore` (put `node_modules/` inside `.gitignore` even if you don’t use it yet).
3. Make **two** small features, each with its own commit.
4. Create a repo on GitHub and push.

```bash
mkdir acp-practice && cd acp-practice
git init
echo "node_modules/" > .gitignore
echo "<!doctype html><title>ACP Practice</title>" > index.html
git add .
git commit -m "feat: initial structure"
echo "<h1>Feature 1</h1>" >> index.html
git add index.html
git commit -m "feat: add header"
echo "<p>Feature 2</p>" >> index.html
git add index.html
git commit -m "feat: add paragraph"

git branch -M main
git remote add origin https://github.com/<username>/acp-practice.git
git push -u origin main
```
