📝 Lesson 1 – git clone

📖 What it does:
→ git clone copies an entire remote repository to your phone.
→ It downloads all files, commits, and branches.
→ It automatically sets up a remote named origin.

🛠️ Practice:
Clone a public repository into your workspace.

🚀 Commands:
$ cd /storage/emulated/0/Download
→ Go to workspace.
$ git clone https://github.com/torvalds/linux.git
→ Clone the Linux kernel (it's huge, maybe try a smaller repo).
$ cd linux
→ Enter the cloned repo.
$ git remote -v
→ origin is already set to the URL.
$ git log --oneline -5
→ See recent commits from the project.
-------------------------------------

For practice, clone a smaller repo like `git clone https://github.com/octocat/Spoon-Knife.git`.