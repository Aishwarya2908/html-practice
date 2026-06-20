Got it — you want **one single copyable Markdown file** that includes *all steps we did* plus the *problems we encountered and fixes*. Here’s the full content you can paste directly into a `.md` file:

```markdown
# GitHub + VS Code Setup Guide (Beginner Friendly)

This document captures all the steps we followed, the problems we encountered, and the fixes we applied.  
Use it as a checklist when setting up on a new computer.

---

## 1. Install Git
- Download from [git-scm.com](https://git-scm.com/downloads).
- During installation, ensure **“Add Git to PATH”** is selected.
- Verify installation:
  ```bash
  git --version
  ```

---

## 2. Create a GitHub Repository
1. Go to [GitHub](https://github.com).
2. Click **New Repository**.
3. Name it (e.g., `html-practice`).
4. Choose **Public** or **Private**.
5. Optionally initialize with a README.
6. Click **Create Repository**.

---

## 3. Clone Repo to Local Machine
- In terminal:
  ```bash
  git clone https://github.com/<username>/<repo>.git
  ```
- This creates a local folder with your repo.

---

## 4. Open Repo in VS Code
- Open VS Code → **File → Open Folder** → select the cloned repo folder.

---

## 5. Basic Git Workflow
- Stage changes:
  ```bash
  git add .
  ```
- Commit changes:
  ```bash
  git commit -m "Your commit message"
  ```
- Push changes:
  ```bash
  git push origin main
  ```
- Pull latest changes:
  ```bash
  git pull origin main
  ```

---

## 6. Problems We Encountered & Fixes

### ❌ Problem 1: `git` not recognized
Error:
```
git : The term 'git' is not recognized...
```
**Fix:**  
- Add Git to PATH:
  - `C:\Program Files\Git\bin`
  - `C:\Program Files\Git\cmd`
- Restart terminal/PC.

---

### ❌ Problem 2: Git works in CMD/PowerShell but not in VS Code terminal
**Fix:**  
- In VS Code, press **Ctrl + Shift + P** → **Terminal: Select Default Profile** → choose **PowerShell**, **Command Prompt**, or **Git Bash**.
- Restart VS Code.

---

### ❌ Problem 3: Where does VS Code put cloned repos?
- By default, if **Git: Default Clone Directory** is empty, repos go to your **user folder** (`C:\Users\<YourName>`).
- **Fix:**  
  - In VS Code settings, search for **Git: Default Clone Directory**.
  - Set it to your preferred folder, e.g.:
    ```
    C:\Users\Aishwarya\Projects
    ```

---

## 7. Optional: Set Default Terminal Working Directory
- In VS Code settings, search for:
  ```
  terminal.integrated.cwd
  ```
- Set it to your projects folder (e.g. `C:\Users\Aishwarya\Projects`).

---

## 8. Configure Git Identity

After installing Git, set your name and email so commits are linked to you:

bash
git config --global user.name "Aishwarya"
git config --global user.email "aishwarya2908@gmail.com"
 
## 9. Install GitLens Extension


## ✅ Final Notes
- Always **clone repos into your chosen projects folder**.
- Always **use the same terminal profile** (PowerShell, CMD, or Git Bash).
- If Git commands fail, check PATH and restart VS Code/PC.

---
```

---

✨ Copy everything above into a file named `github-vscode-setup.md`. That way, you’ll have a ready-made guide to repeat the setup on any new PC.  

Would you like me to extend this doc with **SSH key setup steps** so you can avoid typing your GitHub username/password every time you push?