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

How to undo a committed mistake:

    `git reset --hard HEAD~x` <--VERY dangerous>

    OR

    `git reset --soft HEAD~x` <-Goes back x commits>
    `git reset <file>` <-Takes the file in that particular commit and unstages it>

How to discard untracked junk:

1. Check to see what files are being discarded.

    `git clean --dry-run -fxfd`

2. THEN actually discard those files (as long as you want them discarded, of course):

    `git clean -fxfd`

How to overwrite last commit (such as editing a commit message, or ammending a commit):

    `git add <file>` <-If wanting to add edits of file to the head commit, it needs to be added first>
    
    `git commit --amend` 


How to get out of VIM without ammending the head commit:

    -Delete all of the commit's messages used "Del" key then :wq

https://youtu.be/hv8dhOEzQcM
