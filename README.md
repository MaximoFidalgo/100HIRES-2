# 🛠️ My development setup

This README documents the **step-by-step process** I followed to set up **Cursor**, **AI extensions (Claude & Codex)**, **Git**, and **GitHub** on **Windows**. It is meant as a personal log and a quick reference for anyone repeating the same workflow.

---

## 💻 1. Install Cursor

- Visited the official site **[cursor.com](https://cursor.com)** and downloaded the Windows installer.
- Ran the installer and completed the first-launch wizard (theme, keyboard shortcuts, optional imports from VS Code if offered).
- **Why Cursor:** It is a code editor built around AI assistance (chat, inline edits, and agent-style workflows) while staying familiar if you already know VS Code.

---

## 🧩 2. Install Claude and Codex extensions

- Opened the **Extensions** view in Cursor (same idea as in VS Code: sidebar or `Ctrl+Shift+X`).
- Searched for and installed:
  - **Claude** — Anthropic’s assistant inside the editor (chat, code help, etc., depending on the extension’s features).
  - **Codex** — OpenAI’s coding agent workflow as an extension (CLI/agent integration from within Cursor).
- After installation, I **reloaded the window** when prompted so the extensions activated cleanly.

---

## 🐙 3. Create a GitHub account

- Went to **[github.com](https://github.com)** and signed up with email (and verified the account when GitHub sent the confirmation mail).
- **GitHub** hosts Git repositories in the cloud: backups, history, collaboration, and a public (or private) home for projects.
- Optional but useful: enabled **two-factor authentication (2FA)** under account security settings.

---

## 🔗 4. Connect Claude and Codex to Cursor

- Each extension typically asks you to **sign in** or paste an **API key** the first time you use it.
- I followed the on-screen prompts (browser OAuth or token copy/paste) until both tools showed as **authenticated** in Cursor.
- **Result:** I can use Claude and Codex workflows **without leaving the editor**, with permissions and billing tied to the accounts I linked.

> *Exact menus can change with app updates; if something fails, check the extension’s page in the marketplace for the latest sign-in steps.*

---

## 📦 5. Install Git for Windows

- Downloaded **Git for Windows** from **[git-scm.com](https://git-scm.com/download/win)**.
- Ran the installer and kept sensible defaults (e.g. **Git Bash**, line-ending handling for Windows, default editor) unless I had a specific preference.
- Verified the install in a terminal:

  ```bash
  git --version
  ```

- **Git** is the local tool that tracks file changes (`commit`, `branch`, `merge`) and talks to **GitHub** over HTTPS or SSH when you `push` / `pull`.

---

## 📁 6. Create a repository on GitHub

- Logged into GitHub → **Repositories** → **New**.
- Chose a **repository name**, visibility (**Public** or **Private**), and whether to add a **README**, **.gitignore**, or **license** (I could start empty and add files from my PC later).
- After creation, GitHub showed the **remote URL**, for example:
  - HTTPS: `https://github.com/<username>/<repo>.git`
  - or SSH: `git@github.com:<username>/<repo>.git`

---

## ⬆️ 7. Push this `README.md` to GitHub

**Typical flow** (adjust folder and branch name to match your repo):

1. Open a terminal in the project folder (or open the folder in Cursor and use the integrated terminal).
2. If the folder was **not** yet a Git repo:

   ```bash
   git init
   git remote add origin https://github.com/<username>/<repo>.git
   ```

   If you **cloned** GitHub’s empty repo first, `git remote` is usually already set.

3. Stage, commit, and push:

   ```bash
   git add README.md
   git commit -m "Add README documenting setup steps"
   git branch -M main
   git push -u origin main
   ```

- **Branch note:** Some older repos use `master` instead of `main`; use the name GitHub shows for your default branch.
- **First push:** GitHub may ask you to log in (browser, **Personal Access Token**, or **SSH key** depending on how you configured authentication).

---

## 📋 Summary

| Step | What I did |
|------|------------|
| 🖥️ Editor | Installed **Cursor** from the official site |
| 🤖 AI in-editor | Installed **Claude** and **Codex** extensions |
| 🔐 Accounts | Created **GitHub**; signed in / linked extensions in **Cursor** |
| 📦 Version control | Installed **Git** on Windows |
| ☁️ Remote | Created a **GitHub repository** |
| ⬆️ Publish | Committed and **pushed** this `README.md` |

---

## 📌 Next steps

When you add real application code to this folder, extend this README with **how to run the project**, **dependencies**, and **environment variables** so others (or future you) can get started quickly.
