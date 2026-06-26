📝 Lesson 6 – .gitignore

📖 What it does:
→ .gitignore tells Git which files/folders to ignore.
→ Logs, secrets, and build outputs should never be tracked.
→ Create a .gitignore file and list patterns inside.

🛠️ Practice:
In git-practice, create a file you want to hide, then ignore it.

🚀 Commands:
$ touch secret.log
→ Create a log file.
$ git status
→ secret.log appears as untracked.
$ echo "secret.log" > .gitignore
→ Add pattern to ignore file.
$ git status
→ secret.log no longer shown.
$ cat .gitignore
→ View ignored patterns.
-------------------------------------

Now secret.log stays local. Use .gitignore for any file
that shouldn't be committed.