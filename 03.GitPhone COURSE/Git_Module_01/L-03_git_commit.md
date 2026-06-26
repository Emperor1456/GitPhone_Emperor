📝 Lesson 3 – git commit

📖 What it does:
→ git commit saves staged changes as a permanent snapshot.
→ Every commit gets a unique hash and message.
→ Commit often – each one is a restore point.

🛠️ Practice:
Run these in the same git-practice sandbox:

🚀 Commands:
$ git commit -m "First commit"
→ Create a commit with the message "First commit".
$ git log --oneline
→ View compact commit history.
$ git status
→ Check repo state (clean, nothing left to commit).
-------------------------------------

You’ll see the commit message, a short hash, and “nothing to commit” – meaning the snapshot is safely stored.