Certainly! Here's a Markdown file (`git_commands.md`) with the necessary Git commands and information for future reference:

```markdown
# Git Commands and Information

## Initializing a Repository
```sh
# Initialize a new Git repository
git init
```

## Checking the Status
```sh
# Check the status of the repository
git status
```

## Adding Files
```sh
# Add a specific file to the staging area
git add <file_name>

# Add all files to the staging area
git add .
```

## Committing Changes
```sh
# Commit changes with a message
git commit -m "Your commit message"

# Commit changes with the default editor
git commit
```

## Viewing Commit History
```sh
# View commit history
git log

# View commit history with oneline summary
git log --oneline

# View detailed information about a specific commit
git show <commit_hash>
```

## Branching
```sh
# List all branches
git branch

# Create a new branch
git branch <branch_name>

# Switch to a branch
git switch <branch_name>

# Create and switch to a new branch
git switch -c <branch_name>
```

## Merging Branches
```sh
# Merge a branch into the current branch
git merge <branch_name>
```

## Handling Merge Conflicts
1. When a merge conflict occurs, Git will highlight the conflicting areas in the affected files.
2. Edit the files to resolve the conflicts, removing conflict markers.
3. Add the resolved files to the staging area:
   ```sh
   git add <file_name>
   ```
4. Commit the merge resolution:
   ```sh
   git commit -m "Resolved merge conflict"
   ```

## Ignoring Files
```sh
# Create a .gitignore file to specify files and directories to ignore
touch .gitignore

# Example .gitignore content:
# Ignore all .log files
*.log

# Ignore the node_modules directory
node_modules/
```

## Configuration
```sh
# Set the default editor for Git
git config --global core.editor "code --wait"

# Set the global username and email
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## Viewing and Comparing Changes
```sh
# View changes in the working directory
git diff

# View changes between the staging area and the latest commit
git diff --staged

# View changes between two commits
git diff <commit_hash1> <commit_hash2>
```

## Deleting Branches
```sh
# Delete a branch
git branch -d <branch_name>

# Force delete a branch
git branch -D <branch_name>
```

## Stashing Changes
```sh
# Stash changes
git stash

# List stashed changes
git stash list

# Apply the latest stash
git stash apply

# Apply and drop the latest stash
git stash pop

# Drop a specific stash
git stash drop stash@{index}
```

## Resetting Changes
```sh
# Unstage a file
git restore --staged <file_name>

# Discard changes in the working directory
git restore <file_name>

# Reset to a specific commit (keep changes in working directory)
git reset <commit_hash>

# Hard reset to a specific commit (discard all changes)
git reset --hard <commit_hash>
```

## Cloning a Repository
```sh
# Clone a remote repository
git clone <repository_url>
```

## Pushing and Pulling Changes
```sh
# Push changes to a remote repository
git push <remote_name> <branch_name>

# Pull changes from a remote repository
git pull <remote_name> <branch_name>
```

## Remote Repositories
```sh
# Add a remote repository
git remote add <remote_name> <repository_url>

# List remote repositories
git remote -v

# Remove a remote repository
git remote remove <remote_name>
```

## Tagging
```sh
# Create a new tag
git tag <tag_name>

# Push tags to the remote repository
git push <remote_name> --tags
```
