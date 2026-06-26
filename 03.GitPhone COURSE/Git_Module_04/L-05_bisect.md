📝 Lesson 5 – git bisect

📖 What it does:
→ git bisect finds the commit that introduced a bug.
→ It uses binary search, letting you test commits quickly.
→ You mark each checked commit as "good" or "bad".

🛠️ Practice:
Simulate a bug and find it with bisect.

🚀 Commands:
$ cd /storage/emulated/0/Download/git-practice
$ echo "v1" > app.txt && git add app.txt && git commit -m "v1 good"
$ echo "v2" >> app.txt && git add app.txt && git commit -m "v2 good"
$ echo "bug introduced" >> app.txt && git add app.txt && git commit -m "v3 bug"
$ echo "v4" >> app.txt && git add app.txt && git commit -m "v4 still bug"
$ git bisect start
→ Start bisecting.
$ git bisect bad HEAD
→ Mark current commit as bad.
$ git bisect good <first-commit-hash>
→ Mark a known good commit.
→ Git will checkout a middle commit.
→ Test it: `cat app.txt` (look for "bug introduced").
$ git bisect bad
→ If it contains the bug, mark it bad.
→ Git narrows down.
→ Repeat until it identifies the first bad commit.
$ git bisect reset
→ End the bisect session.
-------------------------------------

Bisect automates debugging — it's fast even with thousands of commits.