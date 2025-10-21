**Theme:** GitHub Organizations; Fork/Clone; Pull Requests; Fetch vs Pull
**Pattern:** 50‑10‑50‑10

---

## Learning Goals

- Know when to use **organizations**.
- Practice **fork** (copy to own account) vs **clone** (local copy).
- Open a **Pull Request**; discuss **fetch** vs **pull**.

## Timeline

### 0–50 min - Demo 1: Organizations & Collaboration

- Why orgs (permissions, teams, repos). If you have a class org, show it.
- Show transferring a repo to an org (or creating a new repo inside the org).

**10‑minute break**

### 60–110 min - Demo 2: Fork -> Clone -> Change -> PR

- Pairing flow: **Student A** owns the repo. **Student B** forks, clones, changes, pushes, opens PR.
- On local:

```bash
git clone https://github.com/<owner>/<repo>.git
cd <repo>

git add README.md
git commit -m "docs: add contributor <yourname>"
git push origin main
```

- Open a **PR** from fork -> upstream; mention reviewers; talk about review etiquette.
- **fetch vs pull**:

```bash
git fetch origin   # download refs only
git pull origin main  # fetch + merge into current branch
```

### 110–120 min - Breakout

- See `day-3-breakout-task.md` for the partner PR exercise.

---

## Exit Tickets

- Student can explain fork vs clone.
- At least one PR opened (or simulated, if working solo).
