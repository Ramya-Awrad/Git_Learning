# 🟢 Basic Git Interview Questions & Answers

1. What is Git? Why use it?
Answer: Git is a distributed version control system (DVCS). It tracks changes in your code, allows multiple people to work together, supports branching/merging, and keeps history so you can go back or undo things.

2. Difference between Git and other version control systems (e.g. SVN, CVS)?
Answer: Key differences:
Git is distributed, every clone is a full copy of the repo.
Branching and merging are cheap and fast in Git.
You can work offline and commit locally.
History rewriting (rebase) is possible.
SVN is centralized — there’s one central server, and developers commit to that.

3. What is a repository (repo)? What are local and remote repositories?
Answer: A repo holds project files, history, metadata, commit history, branches, etc.
Local repo is on your machine (with .git folder).
Remote repo is hosted (GitHub, GitLab, etc.) which you push to and pull from.

4. How do you initialize a Git repository?
Answer: Use git init inside a project directory. That creates the .git folder and starts tracking changes.

5. What is git clone?
Answer: git clone <repo-url> copies a remote repository to your machine, including full history, sets up origin remote automatically.

6. What is the staging area (index)? How does git add work?
Answer: The staging area (index) is where you prepare changes to be committed. git add <file> adds changes from working directory to staging area; then git commit moves from staging to actual history.

7. What is a commit? What data does it store?
Answer: A commit is a snapshot of your working tree, with metadata: author, timestamp, message, pointer to parent commit(s), and pointers to tree / blobs representing files.

8. What is git status and git diff?
Answer:
git status shows which files are untracked, modified, staged, etc.
git diff shows actual differences (line by line) between working directory / staging area / different commits.

9. How do you create and switch branches?
Answer:
git branch <branch-name> to create a branch.
git checkout <branch-name> to switch.
Or in one step: git checkout -b <branch-name>.

10. What is git merge? What is fast-forward merge?
Answer:
git merge <branch> merges the specified branch into the current branch.
A fast-forward merge happens when your branch has not diverged: the target branch pointer simply moves forward to the other branch’s tip (no new commit needed).


