## Git Branching

### What is Branching:
- A branch is like a separate workspace inside your Git project.
- It allows you to work on features or fixes **without affecting the main code**
- Once your work is done, you can merge it back into the main branch


### Common Branching commands:
| Command | Purpose |
|---------|---------|
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

# Merge Conflicts in Git:

## What is a Merge Conflict?  
- A merge conflict occurs when Git cannot automatically combine chnages between two branches. It usually happens when:
    - Two branches modify the same line in a file 
    - One branch deletes a file, while the other modifies it 
    - Files are edited in different branches, and Git is unsure which version to keep

### Real-life Example:
Imagine this scenario:
- You are working on a file called `hello.txt` in `feature` branch
- Some one else edited the same file in main branch 
- Now, when you try to merge `feature-1` into `main`, Git says:
    **I can't decide which version of the file to keep**
This is a Merge Conflict



