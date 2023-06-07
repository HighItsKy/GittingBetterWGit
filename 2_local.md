- Summary
- Review: > git {status,add,diff,commit,reset}
- > git-add -p
- Intro to git graphs
- aliases

How to unstage a staged file:
    `git restore --staged <file>`
    OR
    `git reset {<filename>}`
How to do a partial commit:
    `git add -p`
How to go back x ammount of commits:
    `git reset --soft HEAD~x`
    `git reset` <-Will unstage changes made (so you can edit and restage)
How to go back x ammount of commits AND remove changes (BAD BAD DANGER DANGER):
    `git reset --hard HEAD~x`
How to make the log look more readable:
    `git log --oneline --decorate --graph --all`
How to alias the log:
    `git config --global alias.pl 'log --oneline --decorate --graph --all'`
