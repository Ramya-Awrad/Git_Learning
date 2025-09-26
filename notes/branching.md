## Git Branching

### What is Branching:
- A branch is like a separate workspace inside your Git project.
- It allows you to work on features or fixes **without affecting the main code**
- Once your work is done, you can merge it back into the main branch


### Common Branching commands:
| Command | Purpose |
| `git branch` | List branches |
| `git branch <name>` | Create a new branch |
| `git checkout <name>` | Switch to a branch |
| `git checkout -b <name>` | Create and switch in one step |
| `git merge <name>` | Merge another branch into current one |
| `git branch -d <name>` | Delete a branch |


`git branch` What it does:
- List all local branches in your repo
- shows you which branch you are currently on (with a *)

`git branch <branch-name>` What it does:
- Create a new brnach 
- BUT: it does NOT switch to the branch yet

`git checkout <branch-name>` What it does:
- Switches to an existing branch
- changes the working directory to match that branche's version of files

`git checkout -b <name>` What it does:
- Creates and switches to a new branch in one step

`git merge <name>` What it does:
- Combines the changes from new branch into main
- If the changes don't overlap, Git auto-merges
- If changes conflict, Git will tell you to resolve them manually

`git branch -d <name>` What it does:
- Deletes the local branch after it's merged
- Use `-D` to force delete even if not merged

`git branch -a` What it does:
- List **all Branches** - Local and Remote

