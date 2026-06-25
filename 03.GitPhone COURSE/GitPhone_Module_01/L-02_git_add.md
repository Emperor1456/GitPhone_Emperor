📝 Lesson 2 – git add

git add tells Git which changes to include in the next commit.
Think of it as a shopping cart: you pick what you want before checkout.

It moves files from "untracked/modified" to the staging area.

Practice
In the same git-practice sandbox:

🚀Commands:
. echo "first file" > file1.txt
. git status
. git add file1.txt
. git status
--------------------------------

Notice how the file turns green – that means it's staged.
