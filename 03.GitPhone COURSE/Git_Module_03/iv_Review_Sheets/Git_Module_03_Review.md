# 🔁 Module 03 – Final Review (GitHub & Open‑Source)

## 🧪 Consolidation Challenge
For this review, you will simulate a collaborative workflow using a local "remote".

1. Create a bare repository `remote.git` (use `git init --bare`).
2. Clone `remote.git` into a directory `local1`.
3. Inside `local1`, create a file `project.md` with "Start", commit, and push to `remote`.
4. Clone `remote.git` again into `local2`.
5. In `local2`, add a line "Feature from local2", commit, and push.
6. In `local1`, pull the changes from `remote`.
7. Simulate a fork: create a new directory `fork` and clone `remote.git` into it. Add a file, commit, push (imagine it's your fork). Then create a pull request note explaining what you changed.
8. Practice force‑push safely: make an amend in `local1`, then push with `--force-with-lease`.

Clean up by deleting all test directories.
