**Theme:** Local repo; ACP; `.gitignore`; remote; branches; merge vs rebase
**Pattern:** 50‑10‑50‑10

---

## Learning Goals

- Initialize a local repo; **ACP** changes with meaningful commit messages.
- Connect to GitHub; set upstream; understand tracking branches.
- Create **dev** and **bugfix** branches; compare **merge vs rebase** (conceptual).

## Timeline

### 0–50 min - Demo 1: From folder to remote

- Initialize repo; create README + `index.html`; `.gitignore` basics:

```bash
mkdir local-git-repo && cd local-git-repo
git init
echo "node_modules/" > .gitignore
echo "<!doctype html><title>Week 1</title>" > index.html
git add .
git commit -m "feat: initial files with .gitignore"
git remote add origin https://github.com/<username>/local-git-repo.git
git branch -M main
git push -u origin main
```

- Explain **upstream (-u)** and tracking.

**10‑minute break**

### 60–110 min - Demo 2: Branching • Merge vs Rebase

```bash
git checkout -b dev
echo "<h1>Hello</h1>" >> index.html
git add index.html
git commit -m "feat: add header"


git checkout main
git merge dev


git checkout dev
git rebase main
```

- Whiteboard pros/cons. Keep rebase conceptual this week; prefer **merge** for student work.

### 110–120 min - Breakout

- See `day-2-breakout-task.md`; TAs verify ACP and remote push.

---

## Instructor Notes & Pitfalls

- Students often forget `git add .` or push to the wrong remote.
- Emphasize **small commits** and **present‑tense** messages (“add header”, not “added”).

## Exit Tickets

- Repo exists on GitHub with at least 2 commits.
- `dev` branch exists; student can switch branches.
