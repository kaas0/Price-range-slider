✅ Git Bash Checklist
1. Setup (first time on your PC)
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --global init.defaultBranch main

2. Start a new repo from the folder
git init
git add .
git commit -m "chore: initial commit"

3. Connect to GitHub remote
git remote add origin https://github.com/USERNAME/js-info-starter.git
git branch -M main
git push -u origin main

4. Daily workflow
# Check status of files
git status

# Stage new/changed files
git add <file>        # add specific file
git add .             # add everything

# Commit with a message
git commit -m "feat: add arrays exercise"

# Push to GitHub
git push

5. Get latest changes
git pull

6. Branching (optional but powerful)
# Create and switch to new branch
git checkout -b feature/stopwatch-ui

# Switch back to main
git checkout main

# Merge branch into main
git merge feature/stopwatch-ui

# Push branch to GitHub
git push -u origin feature/stopwatch-ui

7. Log & history
git log --oneline --graph --decorate --all

8. Undo (careful!)
git restore <file>            # discard local changes in a file
git reset HEAD~1 --soft       # undo last commit (keep changes staged)
git reset HEAD~1 --hard       # undo last commit (delete changes)

9. Clone an existing repo (if you switch PC)
git clone https://github.com/USERNAME/js-info-starter.git
cd js-info-starter

10. Housekeeping
git remote -v         # check remote URLs
git branch            # list branches
git fetch --all       # update info about remote branches