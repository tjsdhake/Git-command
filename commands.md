# Git Command Cheat Sheet

## Getting Started
- **Initialize a repository:**
  ```bash
  git init
Initializes a new Git repository.

Clone an existing repository:
bash
Copy code
git clone <repository_url>
Clones a remote repository to your local machine.
Basic Snapshotting
Check the status of your repo:

bash
Copy code
git status
Shows the status of working directory and staging area.

Add files to staging area:

bash
Copy code
git add <file_name>
Adds a specific file to the staging area.

bash
Copy code
git add .
Adds all changed files in the current directory to staging.

Commit changes:

bash
Copy code
git commit -m "commit message"
Commits the staged changes with a message.

View commit history:

bash
Copy code
git log
Shows the commit history for the current branch.

bash
Copy code
git log --oneline
Shows commit history in one-line format.

Branching & Merging
Create a new branch:

bash
Copy code
git branch <branch_name>
Creates a new branch.

Switch to another branch:

bash
Copy code
git checkout <branch_name>
Switches to the specified branch.

Create and switch to a new branch:

bash
Copy code
git checkout -b <branch_name>
Creates and switches to a new branch.

Merge a branch:

bash
Copy code
git merge <branch_name>
Merges the specified branch into the current branch.

Undoing Changes
Unstage a file:

bash
Copy code
git restore --staged <file_name>
Removes a file from the staging area.

Discard changes in a file:

bash
Copy code
git restore <file_name>
Restores the file to its previous committed state.

Remote Repositories
Add a remote repository:

bash
Copy code
git remote add origin <remote_repository_url>
Links your local repository to a remote one.

View remote repositories:

bash
Copy code
git remote -v
Lists all remote repositories connected to your local repo.

Push changes to a remote repository:

bash
Copy code
git push origin <branch_name>
Pushes the local branch to the remote repository.

Pull changes from a remote repository:

bash
Copy code
git pull origin <branch_name>
Fetches and integrates changes from the remote branch.

Stashing
Stash changes:

bash
Copy code
git stash
Temporarily saves your changes without committing.

Apply stashed changes:

bash
Copy code
git stash apply
Applies the most recent stash.

Tagging
Create a tag:

bash
Copy code
git tag <tag_name>
Tags a commit for marking releases or versions.

Push tags to a remote repository:

bash
Copy code
git push origin --tags
Pushes all tags to the remote repository.

Other Useful Commands
Check differences:

bash
Copy code
git diff
Shows the changes in tracked files that are not yet staged.

Remove a file from the repo:

bash
Copy code
git rm <file_name>
Removes the file from the repository.

View branches:

bash
Copy code
git branch
Lists all the branches in the repo.

Delete a branch:

bash
Copy code
git branch -d <branch_name>
Deletes a branch after it’s merged.

Resetting
Hard reset to a specific commit (Dangerous!):

bash
Copy code
git reset --hard <commit_hash>
Resets your working directory and index to the state of the specified commit, discarding all changes.

Soft reset to keep changes staged:

bash
Copy code
git reset --soft <commit_hash>
Moves HEAD to a specific commit but keeps your changes in the staging area.

Rebase
Rebase current branch onto another branch:
bash
Copy code
git rebase <branch_name>
Moves or combines commits from one branch onto another branch.
Viewing Commit Graphs
Graph of commits and branches:
bash
Copy code
git log --graph --oneline --all
Displays a visual graph of all commits and branches.
