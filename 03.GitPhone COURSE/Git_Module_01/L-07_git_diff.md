📝 Lesson 7 – git diff

📖 What it does:
→ git diff shows exact line‑by‑line changes.
→ Compares working directory to staging area.
→ Use it to review work before committing.

🛠️ Practice:
In git-practice, make a change and inspect it.

🚀 Commands:
$ echo "version 1" > code.py
→ Create a file.
$ git add code.py
→ Stage it.
$ echo "version 2" > code.py
→ Modify the file.
$ git diff
→ Show unstaged changes (added lines green, removed lines red).
$ git diff --staged
→ Show staged changes (none, because we haven't re‑staged).
$ git add code.py
→ Stage the new version.
$ git diff --staged
→ Now shows difference between staged and last commit.
-------------------------------------

git diff helps you catch mistakes before they become commits.