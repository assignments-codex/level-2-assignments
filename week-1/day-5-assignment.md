**Weight:** Week 1 single graded item
**Due:** Submit by end of day (link to your public GitHub repo in Moodle)
**Work mode:** Individual (pair for help is okay; submit your own repo)
**AI policy:** You may read docs/tutorials, but **do not have AI write your commands or content**.

---

## Objective

Prove you are fully set up for the rest of the course and can complete the **ACP** workflow on your own:

- Git installed and globally configured
- VS Code configured with **Prettier** and **Live Server**
- GitHub repo created, changes pushed
- Branch created, **PR opened and merged**
- Clear evidence of the workflow in your README

---

## What to Submit

A **public GitHub repository** named `week1-setup-<firstname-lastname>` containing:

1. `README.md` with the following sections filled out:
   - **System Info**
     - OS (Windows/macOS/ChromeOS + version)
     - Git version (`git --version`)
     - VS Code version (Help -> About)
   - **Git Config** (paste output):
     ```bash
     git config --global user.name
     git config --global user.email
     ```
   - **Extensions Installed**: Prettier, Live Server (and any others)
   - **ACP Log** (table with at least 5 entries)
     | # | Change | Command(s) used | Commit message |
     | - | ------ | --------------- | -------------- |
     | 1 | Init repo | `git init` | `chore: init repository` |
     | 2 | Add README | `git add .` -> `git commit` | `docs: add README` |
     | 3 | Create dev branch | `git checkout -b dev` | `chore: create dev branch` |
     | 4 | Add index.html | `git add index.html` -> `git commit` | `feat: add index.html` |
     | 5 | Merge PR | (via GitHub UI) | `merge: dev -> main` |
   - **Screens** (optional): Include small screenshots if helpful.
2. Source files used (`index.html` is fine).
3. Evidence of branch work: a merged **Pull Request** into `main`.

> **Chromebook users:** If using **Codespaces**, note that in **System Info** and include your Codespaces URL (no screenshots required).

---

## Steps (Suggested)

1. Create and initialize a new local folder or Codespace.
2. Configure Git (if not already done).
3. Create `README.md` and `index.html` and make a few small commits.
4. Create repo on GitHub, connect remote, and push.
5. Create a `dev` branch, make a tiny change, push, open a **PR** to `main`, and **merge** it.
6. Update your README’s **ACP Log** with the steps you actually ran.

---

## Rubric (100 pts)

| **Criteria**                  | **Exceeds (20)**                                                                                                             | **Meets (16)**                                      | **Approaches (12)**                           | **Not Evident (0)** |
| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- | --------------------------------------------- | ------------------- |
| Git Installed & Global Config | Version shown; `user.name` & `user.email` correct; default branch set to `main`; line endings configured appropriately by OS | Version shown; `user.name` & `user.email` set       | Partial/unclear evidence of install or config | No evidence         |
| VS Code + Extensions          | VS Code installed; Prettier + Live Server working; `.prettierrc` present; Format on Save enabled                             | VS Code installed; Prettier + Live Server installed | Only one extension or settings missing        | No evidence         |
| Repo & Remote                 | Public GitHub repo connected; clean history; clear commit messages                                                           | Repo connected and pushed                           | Repo exists but not pushed or unclear history | No repo             |
| Branch, PR, Merge             | `dev` branch created, PR opened & merged; student understands PR flow                                                        | Branch created; PR merged                           | Branch exists; no PR or merge                 | No branch work      |
| README Quality & ACP Log      | Complete, neat, reproducible steps with ACP table and versions                                                               | Mostly complete                                     | Partial sections; unclear                     | Missing or minimal  |

**Passing threshold:** 70/100

---

## Submission

- Submit your **public repo URL** on Moodle. Ensure visibility is **Public**.

## Academic Honesty

This is a **readiness** check. We need _your_ configuration and _your_ commands. If you’re stuck, ask a TA-instead of using an AI to do it for you.
