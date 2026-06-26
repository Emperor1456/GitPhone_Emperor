📝 Lesson 3 – git cherry‑pick

📖 What it does:
→ git cherry‑pick copies a specific commit to the current branch.
→ It's like picking one useful change from another branch.

🛠️ Practice:
Cherry‑pick a single commit from one branch to another.

🚀 Commands:
$ cd /storage/emulated/0/Download/git-practice
$ git branch feature-b
$ git switch feature-b
$ echo "useful bugfix" > fix.txt && git add fix.txt && git commit -m "Fix bug"
$ git log --oneline
→ Note the commit hash of the fix.
$ git switch main
$ git cherry-pick <commit-hash>
→ The fix commit is applied to main.
$ git log --oneline
→ A new commit appears with the same change.
-------------------------------------

Cherry‑pick brings just the change, not the whole branch history.