# 🚀 Advanced Git Concepts – Complete Guide

Now that you’ve learned the basics and mid-level topics, this guide covers advanced Git operations for **power users**, **collaborators**, and **open-source contributors**.

These features help with:
✅ Code history control  
✅ Clean commit workflows  
✅ Team collaboration  
✅ Project maintenance

---

## 📘 Table of Contents

1. [Rebase vs Merge](#1-rebase-vs-merge)
2. [Cherry-Pick](#2-cherry-pick)
3. [Interactive Rebase (Editing Commit History)](#3-interactive-rebase-editing-commit-history)
4. [Git Stash (Advanced Use)](#4-git-stash-advanced-use)
5. [Submodules](#5-submodules)
6. [Git Hooks](#6-git-hooks)
7. [Reflog Deep Dive](#7-reflog-deep-dive)
8. [Squash Commits](#8-squash-commits)
9. [Tagging Commits (Releases)](#9-tagging-commits-releases)
10. [Best Practices](#10-best-practices)

---

## 1. 🔁 Rebase vs Merge

### ➤ Merge:
`git merge feature-branch`  

✅ Keeps full history
❌ Results in extra merge commits

### ➤ Rebase:
`git rebase main`  

✅ Clean, linear history
❌ Rewrites commit hashes

#### 📘 When to use:

merge → Team projects with shared branches
rebase → Personal branches, before pull requests

## 2. 🍒 Cherry-Pick

Use cherry-pick to copy a specific commit from one branch to another.

➤ Command:
`git cherry-pick <commit-hash>`  

✅ Useful for bugfixes
❌ Can cause conflicts if the same changes exist elsewhere

## 3. ✍️ Interactive Rebase (Editing Commit History)

➤ Start Interactive Rebase:
`git rebase -i HEAD~3`  

📘 You’ll see:
pick a1b2c3d First commit
pick d4e5f6g Second commit
pick h7i8j9k Third commit


You can replace pick with:
reword → Edit commit message
edit → Modify the commit
squash → Combine with previous commit

## 4. 📦 Git Stash (Advanced Use)
➤ Save work-in-progress:
`git stash`  

➤ List stashes:
`git stash list`  

➤ Apply latest stash:
`git stash apply`  

➤ Apply specific stash:
`git stash apply stash@{1}`  

➤ Apply and remove from stash:
`git stash pop`  

➤ Stash specific files:
`git stash push -m "WIP: bug fix" index.html`  

## 5. 🧩 Git Submodules

Used when a Git repo depends on another Git repo (e.g., plugin, theme).

➤ Add a submodule:
`git submodule add https://github.com/other/project.git path/to/folder`  

➤ Initialize submodules:
`git submodule init`  
`git submodule update`  

➤ Clone with submodules:
`git clone --recurse-submodules <repo-url>`  

⚠️ Advanced concept — avoid unless really needed.

## 6. 🪝 Git Hooks

Hooks are scripts that run automatically on certain Git actions.

📁 Stored in .git/hooks/

🔹 Examples:
pre-commit: Run tests/lint before commit
post-merge: Notify or auto-setup after merging
pre-push: Prevent bad code from pushing

➤ Make hook executable:
`chmod +x .git/hooks/pre-commit`  

✅ Helps maintain code quality
⚠️ Local to your machine; not shared via repo

## 7. 🧭 Reflog Deep Dive

git reflog tracks everything your HEAD points to — even unreachable commits.

➤ Recover lost commits:
`git reflog`  
`git checkout <commit-id>`  

OR

`git reset --hard <commit-id>`  

✅ Lifesaver if you lose work
💡 Keep this in your toolbox!

## 8. 🧱 Squash Commits

Before pushing a feature branch, clean up with squash.

➤ Rebase with squash:
`git rebase -i HEAD~3`  

Use squash to combine small commits into one meaningful commit.

✅ Ideal before pull requests
❌ Do not squash after pushing to shared branches

## 9. 🔖 Tagging Commits (Releases)

Use tags to mark versions or releases.

➤ Create a lightweight tag:
`git tag v1.0`  

➤ Annotated tag (with message):
`git tag -a v1.0 -m "Initial release"`  

➤ Push tags to remote:
`git push origin --tags`  

✅ Helpful for deployment and version tracking

## 10. 🧠 Best Practices

✅ Use rebase interactively before PRs  
✅ Avoid rewriting history after pushing  
✅ Keep feature branches short-lived  
✅ Use stash when switching tasks  
✅ Use tags for versioning  
✅ Avoid submodules unless necessary  
✅ Explore hooks for automation  