📝 Lesson 5 – Pull requests

📖 What it does:
→ A pull request (PR) asks the original repo to accept your changes.
→ You push changes to your fork, then open a PR on GitHub.
→ It's the core of open‑source collaboration.

🛠️ Practice:
Make a change in your fork and open a PR.

🚀 Commands:
$ cd /storage/emulated/0/Download/Spoon-Knife
→ Enter your fork.
$ git switch -c my-fix
→ Create a branch for your change.
$ echo "Hello from Emperor" >> README.md
→ Make a small edit.
$ git add README.md && git commit -m "Add greeting"
→ Commit the change.
$ git push origin my-fix
→ Push the branch to your fork.
-------------------------------------
Now go to your fork on GitHub.
You'll see a "Compare & pull request" button.
Click it, add a description, and submit the PR.