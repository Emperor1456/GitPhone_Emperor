📝 Lesson 2 – Interactive rebase

📖 What it does:
→ Interactive rebase lets you edit, squash, or reorder commits.
→ It's a cleanup tool before sharing work.
→ Opens an editor with a list of recent commits.

🛠️ Practice:
Squash multiple commits into one.

🚀 Commands:
$ cd /storage/emulated/0/Download/git-practice
$ echo "part 1" > work.txt && git add work.txt && git commit -m "Part 1"
$ echo "part 2" >> work.txt && git add work.txt && git commit -m "Part 2"
$ echo "part 3" >> work.txt && git add work.txt && git commit -m "Part 3"
$ git rebase -i HEAD~3
→ An editor opens with the last 3 commits.
→ Change "pick" to "squash" for the 2nd and 3rd commit.
→ Save and exit.
→ Combine commit messages.
$ git log --oneline
→ Three commits become one.
-------------------------------------

Interactive rebase rewrites history — use before pushing.