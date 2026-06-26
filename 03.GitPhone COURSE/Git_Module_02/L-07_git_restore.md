📝 Lesson 7 – git restore

📖 What it does:
→ git restore discards changes in your working directory.
→ Use it to undo modifications you don't want to keep.
→ Works on unstaged files, or can unstage files from the index.

🛠️ Practice:
Make a change, restore it, then restore a staged file.

🚀 Commands:
$ echo "temporary nonsense" > temp.txt
→ Create a file with unwanted content.
$ git add temp.txt && git commit -m "Add temp file"
→ Commit the file so it's tracked.
$ echo "more junk" >> temp.txt
→ Append unwanted changes to the file.
$ git status
→ temp.txt shows as modified.
$ git restore temp.txt
→ Discard the unstaged modification.
$ cat temp.txt
→ The file is back to its committed state.
$ echo "staged junk" >> temp.txt
→ Make another change.
$ git add temp.txt
→ Stage the change.
$ git restore --staged temp.txt
→ Unstage the change (it moves back to modified).
$ git restore temp.txt
→ Now discard the modification completely.
$ git status
→ Working directory is clean again.
-------------------------------------

Use restore to throw away changes safely.