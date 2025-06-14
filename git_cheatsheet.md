# Git Cheatsheet for Open Source Contributors

## Basic Git Commands
```
git clone <url>             # Clone a repo
git status                  # See what's modified
git add <file>              # Stage a file
git commit -m "msg"         # Commit changes
git push origin <branch>    # Push to remote
git pull origin <branch>    # Pull from remote
```

## Branching
```
git checkout -b <branch>    # Create and switch to new branch
git checkout main           # Switch to main
git branch -d <branch>      # Delete local branch
```

## Remotes
```
git remote add upstream <url> # Add upstream remote
git fetch upstream             # Fetch changes from upstream
git merge upstream/main        # Merge changes from upstream
git rebase upstream/main       # Rebase onto upstream
```

## Commit Best Practices
- One change per commit
- Clear, descriptive commit messages
- Use `git log --oneline` to verify history

## Rebase & Conflict Resolution
```
git rebase main
# Resolve conflicts manually
git add <resolved_files>
git rebase --continue
```

## Pull Requests
- Fork > Branch > Commit > Push > PR
- Link PRs to issues
- Request reviews

