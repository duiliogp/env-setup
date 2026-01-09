# git

## Initial config
```bash
# Sets the Git username and email for the current repository only.
git config user.name "Your name"
git config user.email "your-github-email@example.com"

# Updates the 'origin' remote to point to the new repository URL
git remote set-url origin https://git.example.com/user/project.git
```


## Commits
```bash
# Undo the last commit but keep the changes staged.
git reset HEAD~1 --soft

# Undo the last commit and delete all changes.
git reset HEAD~1 --hard
```


## Files 
```bash

# Add the skip-worktree flag to a specific file (Git will ignore local changes)
git update-index --skip-worktree path/to/file

# Remove the skip-worktree flag from a specific file
git update-index --no-skip-worktree path/to/file


# List all files that have the skip-worktree flag enabled
git ls-files -v | grep '^S'

# List only the file paths that are marked as skip-worktree
git ls-files -v | grep '^S' | cut -c3-

# Remove the skip-worktree flag from all files that have it
git ls-files -v | grep '^S' | cut -c3- | xargs git update-index --no-skip-worktree
```

## Logs
```bash
# Lists commits from a specific author, showing hash, author, date, message, and the files changed.
git log --author="username" --pretty=format:"%h | %an | %ad | %s" --date=short --name-only
```




