📝 L-01 git branch – create a new branch
🚀 Commands:
$ git branch <name>
→ create a new branch
$ git branch
→ list all branches (* marks current)
$ git branch -d <name>
→ delete a branch
-----------------------------------------

📝 L-02 git switch – move between branches
🚀 Commands:
$ git switch <branch>
→ switch to an existing branch
$ git switch -c <branch>
→ create and switch in one step
$ git branch
→ confirm current branch (*)
-----------------------------------------

📝 L-03 fast-forward merge – linear merge
🚀 Commands:
$ git merge <branch>
→ fast-forward main to branch tip
$ git branch -d <branch>
→ delete merged branch
-----------------------------------------

📝 L-04 recursive merge – merge with commit
🚀 Commands:
$ git merge <branch>
→ create a merge commit
$ git log --oneline
→ see merge commit with two parents
-----------------------------------------

📝 L-05 merge conflicts – resolve clash
🚀 Commands:
$ git merge <branch>
→ triggers conflict if both changed same line
$ cat <file>
→ view conflict markers
$ echo "resolved" > <file>
→ manually resolve
$ git add <file>
→ stage resolved file
$ git commit -m "Resolve conflict"
→ complete merge
-----------------------------------------

📝 L-06 git stash – temporary shelf
🚀 Commands:
$ git stash
→ stash tracked changes
$ git stash list
→ list stashes
$ git stash pop
→ apply and remove latest stash
-----------------------------------------

📝 L-07 git restore – discard changes
🚀 Commands:
$ git restore <file>
→ discard unstaged modifications
$ git restore --staged <file>
→ unstage a file
-----------------------------------------

📝 L-08 git reset – undo commits
🚀 Commands:
$ git reset --soft HEAD~1
→ undo commit, keep changes staged
$ git reset HEAD~1
→ undo commit, keep changes unstaged (mixed)
$ git reset --hard HEAD~1
→ undo commit, discard changes
-----------------------------------------