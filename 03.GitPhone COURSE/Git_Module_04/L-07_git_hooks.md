📝 Lesson 7 – Git hooks

📖 What it does:
→ Git hooks are scripts that run automatically on Git events.
→ pre‑commit hook runs before a commit is created.
→ pre‑push hook runs before a push.
→ Hooks enforce quality: linting, testing, commit message checks.

🛠️ Practice:
Create a simple pre‑commit hook that rejects commits without a message.

🚀 Commands:
$ cd /storage/emulated/0/Download/git-practice
$ ls .git/hooks
→ See all sample hook files.
$ echo '#!/bin/sh' > .git/hooks/pre-commit
$ echo 'if git log -1 --pretty=%B | grep -q .; then exit 0; else echo "Commit message required!"; exit 1; fi' >> .git/hooks/pre-commit
→ Write a hook script.
$ chmod +x .git/hooks/pre-commit
→ Make it executable.
$ git commit -m "" 2>/dev/null
→ This will fail because message is empty.
$ git commit -m "Valid message"
→ This passes.
-------------------------------------

Hooks live only in your local .git folder.
To share hooks, store them in the repo and symlink or copy them.