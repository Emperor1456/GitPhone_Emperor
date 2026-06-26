📝 Lesson 5 – git status

📖 What it does:
→ git status tells you the current state of your repo.
→ It shows what’s untracked, modified, or staged.
→ Use it before every commit – it’s your safety check.

🛠️ Practice:
Run these in git-practice:

🚀 Commands:
$ git status
→ Nothing to commit – clean working tree.
$ echo "new" > file.txt
→ Create a new file.
$ git status
→ file.txt shown as untracked (red).
$ git add file.txt
→ Stage the file.
$ git status
→ file.txt shown as staged (green).
-------------------------------------

Untracked files appear in red, staged in green.
That’s how you know what will go into the next commit.