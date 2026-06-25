📝 Lesson 1 – git init

What it does:
git init turns any folder into a Git‑tracked project.
It creates a hidden .git folder. That’s it.
You run it once when you begin a new project.

Practice
Run these in Termux (inside a sandbox to keep things clean):

🚀Commands:
. cd /storage/emulated/0/Download
. mkdir git-practice && cd git-practice
. git init
. ls -a (List All- Shows all folders/files)
. git status
--------------------------------

You’ll see the .git folder and “nothing to commit” – that means Git is alive and watching.