📝 Lesson 3 – Fast-forward merge

📖 What it does:
→ A fast‑forward merge moves the main branch forward.
→ Happens when no new commits exist on main.
→ It keeps history linear and clean.

🛠️ Practice:
Create a branch, add a commit, and merge it back.

🚀 Commands:
$ git branch hotfix
→ Create a branch called hotfix.
$ git switch hotfix
→ Move to hotfix.
$ echo "fix" > patch.txt
→ Create a new file.
$ git add patch.txt && git commit -m "Apply hotfix"
→ Stage and commit the fix.
$ git switch main
→ Return to main.
$ git merge hotfix
→ Fast‑forward main to include hotfix.
$ git log --oneline
→ Both branches now point to the same commit.
$ git branch -d hotfix
→ Delete the merged branch.
-------------------------------------

No merge commit is created — history stays clean.