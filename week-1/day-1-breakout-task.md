**Goal:** Prove your machine or Codespace is ready for Week 2 work.

### 1) Install & verify Git

- Run:

```
git --version
```

- Configure (use your real name/email that matches GitHub):

```
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global init.defaultBranch main
# Line endings
# Windows:
git config --global core.autocrlf true
# macOS/Linux:
git config --global core.autocrlf input
```

### 2) Install VS Code + extensions

- Install **Prettier** and **Live Server**.
- Set **Default Formatter = Prettier** and **Format On Save = On**.
- Create a `.prettierrc` file with:

```
{ "singleQuote": true, "semi": true, "trailingComma": "es5", "printWidth": 100 }
```

### 3) Live Server smoke test

- Create a folder `hello-codex`, add `index.html` with minimal HTML, and start **Live Server**.
- Confirm the page auto-refreshes when you save.

### 4) Create a public repo (hello-codex)

```
mkdir hello-codex && cd hello-codex
git init
echo "# Hello Codex" > README.md
git add .
git commit -m "chore: init"
git branch -M main
# Create a new empty repo on GitHub named hello-codex, then:
git remote add origin https://github.com//hello-codex.git
git push -u origin main
```
