📝 Module 2 – Practice Set

🛠️ Task:
Simulate a feature workflow with branching, merging,
conflict resolution, stashing, restoring, and resetting.

🚀 Commands:
$ cd /storage/emulated/0/Download/git-practice
→ Enter your sandbox.
$ git branch feature && git switch feature
→ Create and switch to feature branch.
$ echo "Feature content" > feature.txt
→ Create feature work.
$ git add feature.txt && git commit -m "Add feature"
→ Commit on feature.
$ git switch main
→ Back to main.
$ echo "Main content" > main.txt
→ Create main work.
$ git add main.txt && git commit -m "Update main"
→ Commit on main.
$ git merge feature
→ Recursive merge feature into main.
$ git branch -d feature
→ Delete feature branch.
$ echo "conflict line" > shared.txt
→ Create a file for conflict demo.
$ git add shared.txt && git commit -m "Add shared file"
→ Commit on main.
$ git branch conflict-br && git switch conflict-br
→ Create and switch to a new branch.
$ echo "different line" > shared.txt
→ Change the same file differently.
$ git add shared.txt && git commit -m "Change on branch"
→ Commit the conflicting change.
$ git switch main
→ Return to main.
$ git merge conflict-br
→ Trigger merge conflict.
$ echo "resolved line" > shared.txt
→ Resolve by picking one version.
$ git add shared.txt && git commit -m "Resolve conflict"
→ Complete merge.
$ git branch -d conflict-br
→ Clean up.
$ echo "unstaged work" >> shared.txt
→ Make an unstaged change.
$ git stash
→ Stash it.
$ git stash pop
→ Bring it back.
$ git restore shared.txt
→ Discard changes.
-------------------------------------

All Module 2 skills practiced.