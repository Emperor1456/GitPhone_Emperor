📝 Lesson 2 – git add

📖 What it does:
→ git add tells Git which changes to include next commit.
→ Think of it as a shopping cart before checkout.
→ Moves files from "untracked/modified" to staging area.

🛠️ Practice:
In the same git-practice sandbox:

🚀 Commands:
$ echo "first file" > file1.txt
→ Create a new file.
$ git status
→ file1.txt appears as untracked (red).
$ git add file1.txt
→ Stage the file.
$ git status
→ file1.txt now appears as staged (green).
-------------------------------------

Notice how the file turns green – that means it's staged.