# git

Sets the Git username and email for the current repository only.
```bash
git config user.name "Your name"
git config user.email "your-github-email@example.com"
```

Lists commits from a specific author, showing hash, author, date, message, and the files changed.
```bash
git log --author="username" --pretty=format:"%h | %an | %ad | %s" --date=short --name-only
```

