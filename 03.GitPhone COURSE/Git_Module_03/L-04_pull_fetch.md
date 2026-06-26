📝 Lesson 4 – git pull & git fetch

📖 What it does:
→ git fetch downloads changes from remote but doesn't merge.
→ git pull downloads and merges in one step (fetch + merge).
→ Fetch is safer; pull is faster.

🛠️ Practice:
Use both fetch and pull to get remote updates.

🚀 Commands:
$ cd /storage/emulated/0/Download/git-practice
→ Use your sandbox or any repo with a remote.
$ git fetch origin
→ Download new data, but don't change your files.
$ git log origin/main --oneline -3
→ Inspect what was fetched.
$ git pull origin main
→ Fetch and merge into your current branch.
-------------------------------------

Use fetch to review changes first, pull to apply them.