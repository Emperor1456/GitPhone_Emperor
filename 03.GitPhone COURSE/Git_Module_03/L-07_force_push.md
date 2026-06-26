📝 Lesson 7 – Force‑push etiquette

📖 What it does:
→ Force‑push overwrites remote history.
→ Use it only on your own branches and after informing collaborators.
→ Never force‑push to shared branches (main, develop).

🛠️ Practice:
Practice a force‑push on a throwaway branch.

🚀 Commands:
$ cd /storage/emulated/0/Download/git-practice
$ git branch test-force && git switch test-force
→ Create and switch to a test branch.
$ echo "old" > file.txt && git add file.txt && git commit -m "Old"
→ Commit something.
$ git push origin test-force
→ Push the branch (if remote exists).
$ git reset --hard HEAD~1
→ Remove that commit locally.
$ git push origin test-force --force
→ Overwrite the remote branch.
$ git branch -d test-force
→ Delete local branch when done.
-------------------------------------

Only force‑push your own feature branches.