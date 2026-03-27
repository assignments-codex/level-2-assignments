**Goal:** Practice the ACP loop and pushing to GitHub.

1. Create a project folder and initialize Git.
2. Add an `index.html` and `.gitignore` (put `node_modules/` inside `.gitignore` even if you don't use it yet).
3. Make **two** small features, each with its own commit.
4. Create a repo on GitHub and push.

```
mkdir acp-practice && cd acp-practice
git init
echo "node_modules/" > .gitignore
echo "
ACP Practice" > index.html
git add .
git commit -m "feat: initial structure"
echo "

# Feature 1

" >> index.html
git add index.html
git commit -m "feat: add header"
echo "

Feature 2

" >> index.html
git add index.html
git commit -m "feat: add paragraph"

git branch -M main
git remote add origin https://github.com//acp-practice.git
git push -u origin main
```
