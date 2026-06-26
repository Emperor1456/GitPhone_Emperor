📝 Lesson 3 – Syncing a fork

📖 What it does:
→ The original repo (upstream) may get new commits.
→ You sync your fork by adding an upstream remote and merging.
→ This keeps your fork up to date before making new contributions.

🛠️ Practice:
Add upstream and pull new changes into your fork.

🚀 Commands:
$ cd /storage/emulated/0/Download/Spoon-Knife
→ Go into your fork.
$ git remote add upstream https://github.com/octocat/Spoon-Knife.git
→ Link to the original repo.
$ git remote -v
→ You'll see origin (your fork) and upstream (original).
$ git fetch upstream
→ Download upstream changes without merging.
$ git switch main
→ Make sure you're on main.
$ git merge upstream/main
→ Merge upstream's main into your local main.
$ git push origin main
→ Push the updated main to your fork on GitHub.
-------------------------------------

Now your fork matches the original.