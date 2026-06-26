📝 L-01 git init – create a new repo
🚀 Commands:
$ git init
→ initialise repo (creates .git)
$ ls -a
→ see hidden .git folder
$ git status
→ show current state
-----------------------------------------

📝 L-02 git add – stage changes
🚀 Commands:
$ git add <file>
→ stage a specific file
$ git add .
→ stage everything in current folder
$ git status
→ see what's staged (green)
-----------------------------------------

📝 L-03 git commit – save staged snapshot
🚀 Commands:
$ git commit -m "message"
→ create a commit with a message
$ git log --oneline
→ view compact commit history
-----------------------------------------

📝 L-04 git log – view commit timeline
🚀 Commands:
$ git log
→ full history (press q to quit)
$ git log --oneline
→ compact view
$ git log --oneline -N
→ show last N commits
-----------------------------------------

📝 L-05 git status – check repo state
🚀 Commands:
$ git status
→ show untracked, modified, staged files
-----------------------------------------

📝 L-06 .gitignore – ignore files
🚀 Commands:
$ .gitignore file
→ list patterns, one per line
$ git status
→ verify ignored files are gone
-----------------------------------------

📝 L-07 git diff – inspect changes
🚀 Commands:
$ git diff
→ show unstaged changes
$ git diff --staged
→ show staged changes
-----------------------------------------

📝 L-08 first push – upload repo to GitHub
🚀 Commands:
$ git remote add origin <url>
→ link local to remote
$ git push -u origin main
→ upload and set upstream
-----------------------------------------