# Git_Learning
My Git learning journey with notes and examples

## Roadmap:

1. Basics:  
✅ Goal: Understand what Git is and how to use it locally.

| Topic                | What to Learn                                                    |
| -------------------- | ---------------------------------------------------------------- |
| ✅ What is Git?       | Version control, difference between Git and GitHub.              |
| ✅ Git Installation   | Install Git on Windows/Mac/Linux.                                |
| ✅ Basic Git Commands | `git init`, `git status`, `git add`, `git commit`, `git config`. |
| ✅ File States        | Untracked, Staged, Committed.                                    |
| ✅ Viewing Changes    | `git log`, `git diff`.                                           |

- Practice:
    - Create a local Git repo
    - Track a file, make changes, commit it


2. Working with branches:  
✅ Goal: Learn branching & merging to manage feature development

| Topic                 | What to Learn                                  |
| --------------------- | ---------------------------------------------- |
| ✅ Branching           | `git branch`, `git checkout -b`, `git switch`. |
| ✅ Merging             | `git merge`, fast-forward vs. 3-way merge.     |
| ✅ Resolving Conflicts | How to handle and fix merge conflicts.         |
| ✅ Git Log with Graph  | `git log --oneline --graph --all`.             |

- Practice:
    - Create a feature branch
    - merge it back into main/master
    - Resolve a simple conflict


3. Remote repositories:  
✅ Goal: Collaborate using remote git repositories

| Topic               | What to Learn                        |
| ------------------- | ------------------------------------ |
| ✅ Cloning           | `git clone <url>`.                   |
| ✅ Remote Basics     | `git remote`, `git remote -v`.       |
| ✅ Pushing & Pulling | `git push`, `git pull`, `git fetch`. |
| ✅ Tracking Branches | `origin/main`, `upstream`.           |
| ✅ SSH vs HTTPS      | Authentication methods for GitHub.   |

- Practice:
    - Create a GitHub Repo
    - Push local repo to GitHub
    - Collaborate with a friend


4. Undoing & fixing mistakes:  
✅ Goal: Learn to recover from common git mistakes

| Topic              | What to Learn                      |
| ------------------ | ---------------------------------- |
| ✅ Undo Last Commit | `git commit --amend`, `git reset`. |
| ✅ Unstage a File   | `git restore --staged <file>`.     |
| ✅ Discard Changes  | `git restore <file>`.              |
| ✅ Revert Commit    | `git revert <commit>`.             |
| ✅ Reflog           | `git reflog` to find lost commits. |

- Practice:
    - Try committing a mistake and undo it
    - Recover a deleted file using reflog


5. Advanced Git features:  
✅ Goal: Learn power-user tools for real-world collaboration

| Topic         | What to Learn                      |
| ------------- | ---------------------------------- |
| ✅ Rebase      | `git rebase`, interactive rebase.  |
| ✅ Cherry-pick | Apply commits from other branches. |
| ✅ Stashing    | `git stash`, stash apply/pop.      |
| ✅ Tags        | `git tag`, signed tags.            |
| ✅ Submodules  | Working with repos inside repos.   |
| ✅ Worktrees   | Multiple working directories.      |

- Practice:
    - Rebase a feature branch onto main
    - Stash changes and apply them later


6. Git internals & optimization:  
✅ Goal: Understand how git works under the hood

| Topic                | What to Learn                          |
| -------------------- | -------------------------------------- |
| ✅ Git Object Model   | Commits, trees, blobs, SHA-1 hashes.   |
| ✅ .git Directory     | What's stored inside `.git/`.          |
| ✅ Git Hooks          | Automate tasks like pre-commit checks. |
| ✅ Git Attributes     | Merge strategies, diff settings.       |
| ✅ Large Repositories | Best practices for managing big repos. |

- Practice:
    - Explore `.git` folder
    - Create a `pre-commit` hookscript


## Visual Git Roadmap


```text
Level 1: Basics
├── git init / add / commit / status / log
├── .gitignore / config

Level 2: Branching
├── git branch / checkout / merge
├── conflict resolution

Level 3: Remote Work
├── git push / pull / fetch / clone
├── SSH / HTTPS / remotes

Level 4: Undo & Recovery
├── git reset / restore / revert / reflog

Level 5: Advanced Tools
├── git rebase / cherry-pick / stash
├── tags / submodules / worktrees

Level 6: Internals
├── object model / .git folder
├── hooks / attributes
```
