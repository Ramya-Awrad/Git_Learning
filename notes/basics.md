# Git Basics :
A complete beginner-friendly guide to understanding Git and version control.

---
## 📌 What is Git?
- Git is a Distributed Version Control System used to track code changes.
- It tracks changes to your files and helps teams to collaborate without overwriting each others work.
- Every developer has a full copy of the project history.
- Git is used in combination with remote repositories like GitHub, GitLab, Bitbucket.

---
## 📌 What is GitHub?

- GitHub is a **cloud-based hosting service** for Git repositories.
- It enables:
  - Remote collaboration
  - Version control over the internet
  - Code reviews
  - Issue tracking
  - Project management (via Projects and Issues)

## 🆚 Git vs GitHub

| Git | GitHub |
|-----|--------|
| Installed on your computer | Online hosting platform |
| Tracks code and changes | Helps share code and collaborate |
| Works offline | Works online |
| Command-line tool | Web-based UI for Git repos |

## 🛠️ Installing Git

- Download from: [https://git-scm.com/](https://git-scm.com/)
- After installing, check the version:

`git --version`

---

## 📝 Create a GitHub Account

Go to [https://github.com/](https://github.com/) and sign up.

---

# 🔧 Git Configuration

git config --global user.name "Your Name"
git config --global user.email "your@email.com"

Check all configs: 

`git config --list`

---

## 📁 Initializing a Git Repository

Turn any folder into a Git repo:

`git init`

This creates a hidden .git/ folder that stores all Git data.

---

🧾 Git File States
| State | Meaning |
|-------|---------|
| Untracked | File is not tracked by Git |
| Modified | File has been changed but not staged |
| Staged | File is marked to be committed |
| Committed | Changes saved permanently in local history |

---

## 📌 Basic Git Workflow

Create or modify files

Stage them using git add

Commit the changes using git commit

Example:

```git status                     # Check what's going on```
```git add index.html             # Stage a file```
```git commit -m "Add index file" # Save the snapshot```

## 📝 git status:

Check the current status of files in your repo:

`git status`

It Shows:
New files (untracked)
Modified files
Staged files ready to commit

## ➕ git add

Add a file to the staging area:

`git add file.txt`

Add all files:

`git add .`

Note: Files are not saved until you commit.

## ✅ git commit

Save a snapshot of the staged files:

`git commit -m "Meaningful commit message"`

Every commit creates a unique SHA-1 hash ID.

## 📖 git log

See your commit history:

`git log`

Short version:

`git log --oneline`

With graph:

`git log --oneline --graph --all`

## 🔍 git diff

Compare changes:

Before staging:

`git diff`

After staging (vs last commit):

`git diff --staged`

## 🗑️ git rm

Remove a tracked file:

`git rm file.txt`
`git commit -m "Remove file"`

To untrack but keep the file locally:

`git rm --cached file.txt`

## 📂 .gitignore

Tell Git to ignore certain files/folders:

Example .gitignore:

node_modules/
*.log
.env
.DS_Store


Add .gitignore to your repo root.


## Complete Summary of the above:

| Command         | Purpose                  |
|-----------------|--------------------------|
| `git init`      | Initialize Git repo      |
| `git status`    | Check status of files    |
| `git add`       | Stage files              |
| `git commit -m` | Save snapshot            |
| `git log`       | View commit history      |
| `git diff`      | Compare file changes     |
| `git rm`        | Delete file from repo    |
| `.gitignore`    | Exclude files from Git   |

