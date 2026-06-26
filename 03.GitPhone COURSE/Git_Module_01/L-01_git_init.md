📝 Lesson 1 – git init

📖 What it does:
→ git init turns any folder into a Git‑tracked project.
→ It creates a hidden .git folder. That’s it.
→ You run it once when you begin a new project.

🛠️ Practice:
Run these in Termux (inside a sandbox to keep things clean):

🚀 Commands:
$ cd /storage/emulated/0/Download
→ Go to the Download folder.
$ mkdir git-practice && cd git-practice
→ Create and enter a sandbox folder.
$ git init
→ Initialise a Git repository.
$ ls -a
→ List all files, including hidden .git.
$ git status
→ Check repo state (nothing to commit yet).
-------------------------------------

You’ll see the .git folder and “nothing to commit” – that means Git is alive and watching.