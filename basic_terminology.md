## Core concepts:

| Concept                  | Description                                                                   |
| ------------------------ | ----------------------------------------------------------------------------- |
| **Repository (Repo)**    | A directory tracked by Git, containing all project files and version history. |
| **Working Directory**    | The current checked-out version of the project files.                         |
| **Staging Area (Index)** | Area where changes are prepared before committing.                            |
| **Commit**               | A snapshot of the project's tracked files at a point in time.                 |
| **Branch**               | A separate line of development in a repository.                               |
| **HEAD**                 | A pointer to the current branch reference or commit.                          |
| **Remote**               | A version of your repository hosted elsewhere (e.g., GitHub).                 |
| **Clone**                | Creating a local copy of a remote repository.                                 |
| **Pull**                 | Fetch and integrate changes from a remote branch into the current branch.     |
| **Push**                 | Upload local branch commits to a remote repository.                           |


## Branching & Merging:

| Concept                | Description                                                  |
| ---------------------- | ------------------------------------------------------------ |
| **Merge**              | Combining two branches' changes into one.                    |
| **Rebase**             | Reapplying commits on top of another base tip.               |
| **Fast-forward Merge** | A merge where no new commits are needed (history is linear). |
| **Three-way Merge**    | Used when there’s divergence between branches.               |
| **Conflict**           | Happens when Git can't automatically merge changes.          |


## History & Inspection:

| Concept    | Description                                                              |
| ---------- | ------------------------------------------------------------------------ |
| **Log**    | Shows the commit history.                                                |
| **Diff**   | Shows changes between commits, branches, or working directory and index. |
| **Status** | Shows the current state of the working directory and staging area.       |
| **Blame**  | Shows which commit and author last modified each line of a file.         |
| **Show**   | Displays various types of Git objects (commits, tags, etc.).             |


## Remote Repositories:

| Concept             | Description                                         |
| ------------------- | --------------------------------------------------- |
| **Origin**          | Default name for a remote repository.               |
| **Fetch**           | Downloads objects and refs from another repository. |
| **Upstream**        | The main repo/branch your branch is tracking.       |
| **Tracking Branch** | A local branch that tracks a remote branch.         |


## Undo & recovery:

| Concept      | Description                                                        |
| ------------ | ------------------------------------------------------------------ |
| **Reset**    | Moves HEAD and optionally changes index/working directory.         |
| **Revert**   | Creates a new commit that undoes the effects of a previous commit. |
| **Checkout** | Switches branches or restores working tree files.                  |
| **Stash**    | Temporarily shelves changes without committing them.               |
| **Clean**    | Removes untracked files from the working directory.                |


## Advanced concpets:

| Concept         | Description                                                    |
| --------------- | -------------------------------------------------------------- |
| **Tag**         | Marks specific commits (often used for releases).              |
| **Cherry-pick** | Apply changes from a specific commit to another branch.        |
| **Submodule**   | Repository embedded within another repository.                 |
| **Hooks**       | Custom scripts triggered by Git actions (like pre-commit).     |
| **Worktree**    | Allows multiple working directories for one repository.        |
| **Reflog**      | Shows history of branch/HEAD changes (even lost commits).      |
| **Git Objects** | Internal representations like blobs, trees, commits, and tags. |
| **SHA-1 Hash**  | Unique identifier for commits and objects.                     |


## Confiuration and Utilities:

| Concept               | Description                                                      |
| --------------------- | ---------------------------------------------------------------- |
| **.gitignore**        | Specifies intentionally untracked files to ignore.               |
| **.gitattributes**    | Defines attributes per path, e.g., for merge strategies or diff. |
| **Git Config**        | Configures Git settings at global, system, or repo level.        |
| **Aliases**           | Shortcuts for Git commands.                                      |
| **Credential Helper** | Stores or caches authentication credentials.                     |

