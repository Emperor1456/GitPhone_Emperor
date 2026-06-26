📝 Lesson 8 – git reset

📖 What it does:
→ git reset undoes commits by moving the branch pointer.
→ It can keep or discard changes depending on the mode.
→ Three modes: soft (keep changes staged), mixed (keep changes unstaged), hard (discard everything).

🛠️ Practice:
Create commits, then undo them with different reset modes.

🚀 Commands:
$ echo "v1" > version.txt && git add version.txt && git commit -m "v1"
→ Commit version 1.
$ echo "v2" > version.txt && git add version.txt && git commit -m "v2"
→ Commit version 2.
$ git log --oneline
→ Two commits visible.
$ git reset --soft HEAD~1
→ Undo last commit, keep changes staged.
$ git status
→ version.txt changes still staged.
$ git commit -m "v2 again"
→ Recommit the same changes.
$ git reset HEAD~1
→ Undo last commit, keep changes unstaged (mixed is default).
$ git status
→ Changes are present but unstaged.
$ git reset --hard HEAD~1
→ Discard the last commit and changes completely.
$ git log --oneline
→ Only v1 remains.
$ cat version.txt
→ File is back to v1 content.
-------------------------------------

Use reset carefully — especially --hard.