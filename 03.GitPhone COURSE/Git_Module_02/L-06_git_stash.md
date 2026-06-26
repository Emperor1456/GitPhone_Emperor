📝 Lesson 6 – git stash

📖 What it does:
→ git stash temporarily saves uncommitted changes.
→ It gives you a clean working directory instantly.
→ Use it when you need to switch branches but aren’t ready to commit.

🛠️ Practice:
Make a change, stash it, then bring it back.

🚀 Commands:
$ echo "work in progress" > wip.txt
→ Create a file with unfinished work.
$ git status
→ wip.txt shows as untracked.
$ git add wip.txt
→ Stage the file (stash works on tracked changes).
$ git stash
→ Stash the staged change and revert to a clean state.
$ git status
→ Working directory is clean.
$ git stash list
→ Show all stashed changes.
$ git stash pop
→ Re-apply the most recent stash and remove it from the list.
$ git status
→ wip.txt is back as staged.
-------------------------------------

Stashing is like a temporary shelf for your code.