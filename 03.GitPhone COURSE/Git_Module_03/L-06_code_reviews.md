📝 Lesson 6 – Code reviews

📖 What it does:
→ After opening a PR, maintainers may request changes.
→ You update your branch, push again, and the PR updates.
→ Use `git commit --amend` or add new commits to address feedback.

🛠️ Practice:
Simulate a review cycle by amending a commit.

🚀 Commands:
$ cd /storage/emulated/0/Download/Spoon-Knife
$ git switch my-fix
→ Ensure you're on the PR branch.
$ echo "Reviewed" >> README.md
→ Make a review‑requested change.
$ git add README.md
→ Stage it.
$ git commit --amend -m "Add greeting (reviewed)"
→ Amend the last commit instead of adding a new one.
$ git push origin my-fix --force
→ Force‑push because history changed.
-------------------------------------

Always communicate with maintainers before force‑pushing.