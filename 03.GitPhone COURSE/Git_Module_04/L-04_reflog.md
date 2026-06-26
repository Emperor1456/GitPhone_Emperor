📝 Lesson 4 – git reflog

📖 What it does:
→ git reflog records every move of HEAD.
→ It lets you recover lost commits, resets, or rebases.
→ Reflog is local — it is not pushed.

🛠️ Practice:
Lose a commit with reset, then recover it via reflog.

🚀 Commands:
$ cd /storage/emulated/0/Download/git-practice
$ echo "precious" > treasure.txt && git add treasure.txt && git commit -m "Treasure"
$ git reset --hard HEAD~1
→ The commit appears gone.
$ git reflog
→ Find the hash of the "Treasure" commit.
$ git cherry-pick <treasure-hash>
→ Apply it back.
-------------------------------------

The reflog is your safety net — use it to undo almost anything.