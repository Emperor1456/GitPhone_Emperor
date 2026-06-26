📝 Lesson 5 – Merge conflicts

📖 What it does:
→ A merge conflict happens when Git cannot merge changes automatically.
→ It occurs when the same line is edited in both branches.
→ Git marks the file and asks you to choose what to keep.

🛠️ Practice:
Create a conflict between two branches and resolve it.

🚀 Commands:
$ git branch conflict-demo
→ Create a branch to simulate conflict.
$ git switch conflict-demo
→ Move to the new branch.
$ echo "version from conflict-demo" > conflict.txt
→ Create a file with one version.
$ git add conflict.txt && git commit -m "Edit from conflict-demo"
→ Commit on the feature branch.
$ git switch main
→ Return to main.
$ echo "version from main" > conflict.txt
→ Create the same file with a different version.
$ git add conflict.txt && git commit -m "Edit from main"
→ Commit on main.
$ git merge conflict-demo
→ Merge triggers a CONFLICT warning.
$ cat conflict.txt
→ View conflict markers (<<<<<<<, =======, >>>>>>>).
$ echo "resolved version" > conflict.txt
→ Manually write the final version.
$ git add conflict.txt
→ Stage the resolved file.
$ git commit -m "Resolve merge conflict"
→ Complete the merge.
$ git branch -d conflict-demo
→ Clean up the branch.
-------------------------------------

Conflict markers guide you, but you decide the final content.