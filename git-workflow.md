# Git Push and Pull Best Practices

## Daily Workflow

1. **Start your day:**
   - `git pull` - Get latest changes
   
2. **Make changes:**
   - Edit files
   - Test your code
   
3. **Commit frequently:**
   - `git status` - See what changed
   - `git diff` - Review changes
   - `git add <files>` - Stage changes
   - `git commit -m "Clear message"` - Commit
   
4. **Push regularly:**
   - `git push` - Upload to GitHub
   - Push at least once per session
   
5. **Before finishing:**
   - `git status` - Ensure nothing is uncommitted
   - `git push` - Final push of the day

## Key Commands

- `git fetch` - Download info about changes (doesn't apply them)
- `git pull` - Download AND apply changes (fetch + merge)
- `git push` - Upload your commits to GitHub
- `git status` - Check current state
- `git diff` - See unstaged changes
- `git diff --staged` - See staged changes
- `git log --oneline` - View commit history

## Remember

- Pull before you start working
- Commit often with clear messages
- Push frequently to back up work
- Always pull before pushing if working with others
- Use `git status` liberally - it's your friend!
