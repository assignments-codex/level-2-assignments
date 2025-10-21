## System Info

- **OS:** Windows 11
- **Git:** `git version 2.x.x`
- **VS Code:** 1.xx.x
- **(If Chromebook) Codespaces:** yes/no

## Git Config

```bash
git config --global user.name
git config --global user.email
```

## Extensions

- Prettier
- Live Server
- (optional) GitLens

## ACP Log

| #   | Change            | Command(s) used                      | Commit message             |
| --- | ----------------- | ------------------------------------ | -------------------------- |
| 1   | Init repo         | `git init`                           | `chore: init repository`   |
| 2   | Add README        | `git add .` -> `git commit`          | `docs: add README`         |
| 3   | Create dev branch | `git checkout -b dev`                | `chore: create dev branch` |
| 4   | Add index.html    | `git add index.html` -> `git commit` | `feat: add index.html`     |
| 5   | Merge PR          | (via GitHub UI)                      | `merge: dev -> main`       |
