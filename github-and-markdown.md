
# GitHub Cheat Sheet

## **Repository Management**

### Initializing and Cloning
- `git init`  
  Initialize a new Git repository.

- `git clone <url>`  
  Clone an existing repository.

### Adding and Committing Changes
- `git add <file>`  
  Stage a file for commit.  
  - `git add .`: Stage all changes.

- `git commit -m "<message>"`  
  Commit staged changes with a message.

- `git commit --amend -m "<new message>"`  
  Amend the last commit with a new message.

### Branch Management
- `git branch`  
  List all branches.

- `git branch <branch-name>`  
  Create a new branch.

- `git checkout <branch>`  
  Switch to an existing branch.

- `git switch <branch>`  
  Switch to an existing branch (alternative to `checkout`).

- `git switch -c <branch-name>`  
  Create and switch to a new branch.

- `git branch -d <branch-name>`  
  Delete a branch.

### Merging and Rebasing
- `git merge <branch>`  
  Merge the specified branch into the current branch.

- `git rebase <branch>`  
  Reapply commits on top of another base branch.

### Stashing Changes
- `git stash`  
  Save changes to a stash for later.

- `git stash list`  
  List all stashes.

- `git stash apply`  
  Apply the latest stash without deleting it.

- `git stash drop`  
  Delete the latest stash.

### Remote Repositories
- `git remote -v`  
  List remote connections.

- `git remote add <name> <url>`  
  Add a new remote repository.

- `git push`  
  Push commits to the default remote branch.

- `git push -u <remote> <branch>`  
  Push to a remote branch and set it as upstream.

- `git pull`  
  Fetch and merge changes from the remote repository.

- `git fetch`  
  Fetch changes without merging.

### Undoing Changes
- `git reset <file>`  
  Unstage a file.

- `git reset --soft <commit>`  
  Undo commits but keep changes staged.

- `git reset --hard <commit>`  
  Undo commits and discard changes.

- `git checkout -- <file>`  
  Discard changes to a file.

- `git revert <commit>`  
  Create a new commit to reverse a previous one.

### Viewing History and Status
- `git status`  
  Show the working directory and staging area status.

- `git log`  
  Show commit history.  
  - `git log --oneline`: Compact history.

- `git diff`  
  Show changes not staged for commit.

- `git diff --staged`  
  Show changes staged for commit.

### Tagging
- `git tag`  
  List all tags.

- `git tag <tag-name>`  
  Create a lightweight tag.

- `git tag -a <tag-name> -m "<message>"`  
  Create an annotated tag.

- `git push origin <tag>`  
  Push a tag to the remote repository.

## **Miscellaneous Commands**
- `git config --global user.name "<name>"`  
  Set the global username.

- `git config --global user.email "<email>"`  
  Set the global email.

- `git clean -f`  
  Remove untracked files.

- `git cherry-pick <commit>`  
  Apply a specific commit from another branch.

- `git blame <file>`  
  Show who made changes to each line of a file.

- `git show <commit>`  
  Show details of a specific commit.

---

### **Tips**
- Use `git help <command>` to get detailed information about any command.
- Alias frequently used commands for efficiency (e.g., `alias gs="git status"`).

