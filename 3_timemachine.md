- Summary
- Review aliases: st, pl, co
- Hopping around commits
- Undo uncommitted mistake (staged)
- Undo entire commit
- Undo commited mistake
- Discard unstaged junk (pre-add)
- Discard untracked junk (new)
- Overwrite the last commit (bonus)
- Fixing old mistakes (bonus)
- Undo rebase (bonus)

How to hop around:
    `git co <commit hash>`
How to undo an uncommited mistake (OR staged mistake i.e., retrieving a deleted file):
    `git restore <file>`
    OR
    `git co -- <file>`