# Change Author of Commit
## Changing the last commit
```bash
git commit --amend --author="Brittany Carusone <brcarusone@gmail.com>"
```
[source](https://itnext.io/git-change-author-709783e69626)


## Changing the root commit
```bash
# step 1 - start rebase
git rebase -i --root

# step 2 - change pick to edit for commit to amend
edit <commit_id> <commit_msg>
pick <commit_id> <commit_msg>
...

# step 3 - save and quit then run
git commit --amend --author="Brittany Carusone <brcarusone@gmail.com>"
```
[source](https://www.reddit.com/r/github/comments/x1w5y0/comment/imgcami/?utm_source=share&utm_medium=web2x&context=3)