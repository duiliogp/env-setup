# linux

## .bashrc

Customizes the Bash prompt to show the current directory and the active Git branch.
```bash
PS1='\[\033[01;34m\]\W\[\033[00m\] \[\033[01;32m\]$(__git_ps1 "%s")\[\033[00m\] \$ '
```

