# git


```bash
# Sets the Git username and email for the current repository only.
git config user.name "Your name"
git config user.email "your-github-email@example.com"

# Updates the 'origin' remote to point to the new repository URL
git remote set-url origin https://git.example.com/user/project.git

# Lists commits from a specific author, showing hash, author, date, message, and the files changed.
git log --author="username" --pretty=format:"%h | %an | %ad | %s" --date=short --name-only

# Undo the last commit but keep the changes staged.
git reset HEAD~1 --soft

# Undo the last commit and delete all changes.
git reset HEAD~1 --hard

# Tells Git to ignore local changes to that file/folder.
git update-index --skip-worktree filename.js

# Tells Git to track changes again for that file/folder.
git update-index --no-skip-worktree filename.js

```





