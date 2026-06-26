📝 Lesson 4 – Recursive merge

📖 What it does:
→ A recursive merge creates a new merge commit.
→ Happens when both branches have new work.
→ The merge commit ties the two histories together.

🛠️ Practice:
Create two divergent branches and merge them.

🚀 Commands:
$ git branch feature
→ Create a feature branch.
$ git switch feature
→ Move to feature.
$ echo "feature work" > feature.txt
→ Create a feature file.
$ git add feature.txt && git commit -m "Add feature"
→ Commit on feature.
$ git switch main
→ Back to main.
$ echo "main work" > main.txt
→ Create a file on main.
$ git add main.txt && git commit -m "Update main"
→ Commit on main.
$ git merge feature
→ Merge feature into main (recursive).
$ git log --oneline
→ A merge commit appears, joining both histories.
$ git branch -d feature
→ Clean up the merged branch.
-------------------------------------

A merge commit has two parents — it records the fact of the merge.