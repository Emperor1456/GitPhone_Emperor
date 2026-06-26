📝 L-01 git rebase – rewrite history linear
🚀 Commands:
$ git rebase <branch>
→ move commits on top of branch
-----------------------------------------

📝 L-02 Interactive rebase – edit history
🚀 Commands:
$ git rebase -i HEAD~N
→ squash, reorder, edit commits
-----------------------------------------

📝 L-03 git cherry‑pick – copy a commit
🚀 Commands:
$ git cherry-pick <hash>
→ apply specific commit here
-----------------------------------------

📝 L-04 git reflog – recovery log
🚀 Commands:
$ git reflog
→ see all HEAD movements
$ git cherry-pick <hash>
→ recover lost commit
-----------------------------------------

📝 L-05 git bisect – find a bug
🚀 Commands:
$ git bisect start
$ git bisect bad HEAD
$ git bisect good <hash>
→ test, mark good/bad
$ git bisect reset
→ end session
-----------------------------------------

📝 L-06 git tag – mark release
🚀 Commands:
$ git tag <name>
→ create lightweight tag
$ git push origin <tag>
→ push tag to remote
-----------------------------------------

📝 L-07 Git hooks – automate actions
🚀 Commands:
→ write script in .git/hooks/
→ chmod +x <hook-file>
→ runs automatically
-----------------------------------------