📝 Module 1 – Practice Set

🛠️ Task:
Create a new project from scratch, track it,
connect it to GitHub, and push it.
This will use everything you learned.

🚀 Commands:
$ cd /storage/emulated/0/Download
→ Go to your workspace.
$ mkdir project-alpha && cd project-alpha
→ Create and enter a fresh folder.
$ git init
→ Initialise the repo.
$ echo "# Project Alpha" > README.md
→ Create a README.
$ git status
→ Check that README is untracked.
$ git add README.md
→ Stage the README.
$ git commit -m "Initial commit"
→ Commit the snapshot.
$ git log --oneline
→ Verify the commit.
$ echo "log/" > .gitignore
→ Ignore a log folder.
$ mkdir log && echo "test" > log/app.log
→ Create a file inside ignored folder.
$ git status
→ Confirm the log folder is ignored.
$ git diff
→ No changes (because ignored).
$ git remote add origin <your-repo-url>
→ Link to GitHub (create an empty repo first).
$ git branch -M main
→ Ensure the branch is main.
$ git push -u origin main
→ Upload to GitHub.
-------------------------------------

Refresh GitHub. You should see README.md
but no log/ folder.