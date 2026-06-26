📝 Lesson 6 – git tag

📖 What it does:
→ git tag marks a specific commit as important.
→ Typically used for version releases (v1.0, v2.3).
→ Tags are permanent and can be pushed to remote.

🛠️ Practice:
Create and push a lightweight tag.

🚀 Commands:
$ cd /storage/emulated/0/Download/git-practice
$ echo "stable release" > release.txt && git add release.txt && git commit -m "Stable"
$ git tag v1.0
→ Create a lightweight tag on the current commit.
$ git tag
→ List all tags.
$ git show v1.0
→ Show tag details.
$ git push origin v1.0
→ Push the tag to GitHub.
-------------------------------------

For annotated tags with a message, use `git tag -a v1.0 -m "Release v1.0"`.