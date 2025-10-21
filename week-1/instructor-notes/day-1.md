**Theme:** Install & configure Git + VS Code; Prettier; Live Server; Chromebook paths

---

## Learning Goals

- Install/update **Git** and set global config (`user.name`, `user.email`, default branch).
- Install **VS Code**, configure **Prettier** and **Live Server**, set Bash as integrated terminal (Windows).
- Understand **Git vs GitHub** (tooling vs hosting/collaboration).
- Chromebook paths: **Linux (Beta)** _or_ **GitHub Codespaces**.

## Instructor Prep

- Whiteboard “Git vs GitHub” (2 circles + overlap).
- Have download links available (Git, VS Code).

---

## Timeline

### 0–50 min - Demo 1: Git & VS Code setup

**Talk-through (5 min):** Why Git; why VS Code; what “ACP” means (Add -> Commit -> Push).
**Install (20–25 min):**

- **Windows**
  - Install **Git for Windows** (include Git Bash). Choose **“Use Git from the command line and also from 3rd‑party software”** when prompted.
  - Install **VS Code**. In VS Code -> Extensions: install **Prettier** and **Live Server**.
  - VS Code -> Terminal -> **Select Default Profile -> Git Bash**.
- **macOS**
  - Install Git (Xcode CLI or Homebrew).
  - Install **VS Code**, add **Prettier** and **Live Server**.
- **ChromeOS**
  - _Option A (preferred for low‑power):_ **GitHub Codespaces** -> Create a codespace on new repo; VS Code web opens with terminal.
  - _Option B (Linux Beta):_ Settings -> **Developers -> Linux development environment -> Turn on** -> `sudo apt update && sudo apt install -y git`. Download VS Code `.deb` and install with Software app.

**Configure Git (all OS):**

```bash
git --version
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global init.defaultBranch main
```

**VS Code settings quick start (UI path):**

- _Settings_ -> search **“default formatter”** -> set to **Prettier**.
- Enable **Format On Save**.
- Set **Tab Size: 2**; ensure **End of Line: LF**.
- Create a **.prettierrc** at repo root:

```json
{ "singleQuote": true, "semi": true, "trailingComma": "es5", "printWidth": 100 }
```

**Micro‑demo (5 min):** New folder -> `index.html` -> start **Live Server** -> see hot‑reload.

> **Common pitfalls:** corporate firewalls, missing command‑line tools on macOS, Windows credential prompts, Chromebook permissions.

**10‑minute break**

### 60–110 min - Demo 2: Git vs GitHub • first ACP

- Draw the difference: Git = local VCS; GitHub = remote hosting + collaboration.
- Create a local folder, ACP a change, create a **new repo on GitHub**, connect and push:

```bash
mkdir hello-codex && cd hello-codex
git init
echo "# Hello Codex" > README.md
git add .
git commit -m "chore: init repo with README"
git remote add origin https://github.com/<username>/hello-codex.git
git branch -M main
git push -u origin main
```

- Verify on GitHub; walk through repo UI and basic settings.

### 110–120 min - Breakout (TA Checks)

- See `day-1-breakout-task.md` for the student checklist.
- TA/Instructor circulate; verify Git version, config, VS Code extensions, Live Server runs.

---

## Exit Tickets / Evidence

- `git --version` runs.
- `git config --global user.name/email` set.
- VS Code installed with **Prettier** + **Live Server**.
- Public GitHub repo created (hello‑codex).

## Troubleshooting Notes

- **MAC:** If “xcrun: error: invalid active developer path” -> `xcode-select --install`.
- **Windows:** If `.sh` isn’t recognized in VS Code terminal -> ensure default terminal is **Git Bash**.
- **ChromeOS:** If Linux isn’t available -> use **Codespaces** for now.
