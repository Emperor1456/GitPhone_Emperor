📝 Lesson 1 – git rebase

📖 What it does:
→ git rebase moves commits to a new base.
→ It rewrites history to make it linear.
→ Use it to keep feature branches up to date with main.

🛠️ Practice:
Rebase a feature branch onto main.

🚀 Commands:
$ cd /storage/emulated/0/Download/git-practice
$ echo "main line" > base.txt && git add base.txt && git commit -m "Base commit"
$ git branch feature
$ echo "feature work" >> base.txt && git add base.txt && git commit -m "Feature work"
$ git switch main
$ echo "main update" > main.txt && git add main.txt && git commit -m "Main update"
$ git switch feature
$ git rebase main
→ feature commits are now on top of main.
$ git log --oneline
→ History is linear.
-------------------------------------

Never rebase commits that have been pushed to a shared branch.