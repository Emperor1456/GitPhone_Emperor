# 🔁 Module 04 – Final Review (Professional Git Craft)

## 🧪 Consolidation Challenge
Use a new directory `review04` initialized as a Git repo.

1. Create three commits: "C1", "C2", "C3" (use empty files or echo).
2. Rebase interactively to squash C2 and C3 into a single commit.
3. Create a branch `fix`, add a commit "Fix1". Cherry‑pick that commit into main.
4. Simulate a lost commit: reset main back one commit, then use `reflog` to recover it.
5. Create a tag `v1.0` at the latest commit.
6. Write a simple pre‑commit hook that forbids committing files with the word "TODO". Test it.
7. (Optional) Use `git bisect` on a series of commits where one introduces an error (you can simulate by creating a file with bad content). Practice identifying the bad commit.

After you finish, clean up `review04`.
