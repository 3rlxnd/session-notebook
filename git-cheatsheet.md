# Git Cheat Sheet

## Configuration
git config --global user.name "Your Name"          # Set global username
git config --global user.email "you@example.com"  # Set global email
git config --list                                # View Git configuration

## Initialization
git init                           # Initialize a new repository
git clone <url>                    # Clone a repository

## Basic Commands
git status                         # Check the status of changes
git add <file>                     # Stage a specific file
git add .                          # Stage all changes
git commit -m "Message"            # Commit changes with a message
git log                            # View commit history

## Branching
git branch                         # List all branches
git branch <branch-name>           # Create a new branch
git checkout <branch-name>         # Switch to a branch
git checkout -b <branch-name>      # Create and switch to a branch
git merge <branch-name>            # Merge a branch into the current branch
git branch -d <branch-name>        # Delete a branch

## Remote Repositories
git remote add origin <url>        # Add a remote repository
git remote -v                      # View remote repositories
git push -u origin <branch-name>   # Push changes to remote (and set upstream)
git pull                           # Fetch and merge changes from remote
git fetch                          # Fetch changes from remote without merging

## Undoing Changes
git restore <file>                 # Discard changes in a file
git restore --staged <file>        # Unstage a file
git reset --soft HEAD~1            # Undo last commit, keep changes staged
git reset --mixed HEAD~1           # Undo last commit, keep changes unstaged
git reset --hard HEAD~1            # Undo last commit and discard changes

## Stashing
git stash                          # Save uncommitted changes for later
git stash list                     # List all stashes
git stash apply                    # Apply the latest stash
git stash drop                     # Remove the latest stash

## Tags
git tag                            # List all tags
git tag <tag-name>                 # Create a new tag
git push origin <tag-name>         # Push a tag to the remote repository
git tag -d <tag-name>              # Delete a tag locally
git push origin --delete <tag-name> # Delete a remote tag

## Logs and History
git log                            # View commit history
git log --oneline                  # View history as a single line per commit
git diff                           # Show changes between commits/files
git blame <file>                   # Show who made changes line by line

## Collaboration
git pull                           # Fetch and merge changes from remote
git fetch                          # Fetch changes without merging
git rebase <branch-name>           # Reapply commits on top of another branch
git cherry-pick <commit-hash>      # Apply a specific commit to the current branch

## Aliases (Optional)
git config --global alias.st status              # Shorten `git status` to `git st`
git config --global alias.co checkout           # Shorten `git checkout` to `git co`
git config --global alias.br branch             # Shorten `git branch` to `git br`
git config --global alias.cm "commit -m"        # Shorten `git commit -m` to `git cm`
git config --global alias.hist "log --oneline"  # Shorten `git log --oneline` to `git 
hist`

## Useful Tips
- Use `git help <command>` to get help for a specific command.
- Always pull changes before starting new work: `git pull`.
- Use `.gitignore` to exclude files from being tracked.

