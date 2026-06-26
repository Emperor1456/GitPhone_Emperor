📝 L-01 git clone – copy remote repo
🚀 Commands:
$ git clone <url>
→ download entire repo
-----------------------------------------

📝 L-02 Forking – GitHub copy
🚀 Commands:
→ Use GitHub Fork button
→ Then clone your fork
-----------------------------------------

📝 L-03 Syncing fork – keep up to date
🚀 Commands:
$ git remote add upstream <original-url>
→ add original repo
$ git fetch upstream
→ download updates
$ git merge upstream/main
→ merge into local main
$ git push origin main
→ update fork on GitHub
-----------------------------------------

📝 L-04 git pull & fetch – get remote changes
🚀 Commands:
$ git fetch <remote>
→ download only
$ git pull <remote> <branch>
→ download and merge
-----------------------------------------

📝 L-05 Pull request – propose changes
🚀 Commands:
$ git push origin <branch>
→ push to your fork
→ Open PR on GitHub
-----------------------------------------

📝 L-06 Code review – address feedback
🚀 Commands:
$ git commit --amend
→ update last commit
$ git push origin <branch> --force
→ update PR
-----------------------------------------

📝 L-07 Force‑push etiquette – rewrite safely
🚀 Commands:
$ git push origin <branch> --force
→ overwrite remote (own branches only)
-----------------------------------------