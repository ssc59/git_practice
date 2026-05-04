# Git Essential Commands Cheat Sheet

## Configuration
- `git config --global user.name "Name"` - Set username
- `git config --global user.email "email"` - Set email
- `git config --list` - View all configuration

## Viewing History
- `git log` - Full commit history
- `git log --oneline` - Compact history
- `git log --oneline --graph --all` - Visual history
- `git log --author="Name"` - Filter by author
- `git log --since="1 week ago"` - Filter by date
- `git show` - Show last commit
- `git show abc123` - Show specific commit

## Undoing Changes
- `git restore <file>` - Discard working directory changes
- `git restore --staged <file>` - Unstage file
- `git revert <commit>` - Create new commit undoing a commit (safe)
- `git reset --soft HEAD~1` - Undo commit, keep changes staged
- `git reset HEAD~1` - Undo commit, unstage changes
- `git reset --hard HEAD~1` - Undo commit, delete changes (DANGER!)

## Stashing
- `git stash` - Save work in progress
- `git stash push -m "message"` - Stash with description
- `git stash list` - View all stashes
- `git stash show` - Preview latest stash
- `git stash pop` - Apply and remove stash
- `git stash apply` - Apply but keep stash
- `git stash drop` - Delete a stash
- `git stash clear` - Delete all stashes

## Fetching and Pulling
- `git fetch` - Download changes (don't merge)
- `git pull` - Download and merge changes (fetch + merge)
- `git log main..origin/main` - See remote commits

## Time Travel
- `git checkout <commit>` - View old commit (detached HEAD)
- `git switch main` - Return to branch

## Remember
- Use `revert` for pushed commits (safe)
- Use `reset` only for local commits (rewrites history)
- Always `fetch` or `pull` before starting work
- Stash when you need to switch contexts quickly
- Never reset commits that are on GitHub!
