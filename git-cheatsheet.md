# Git Cheat Sheet

## Setup
```
git config --global user.name “[firstname lastname]”
git config --global user.email “[valid-email]"
git config --global color.ui auto
```
## Setup & Init
```
git init
git clone [url]
```
## Stage & Snapshot
```
git status
git add [file]
git reset [file]
git diff
git diff --staged
git commit -m “[descriptive message]”
git commit -am “[descriptive message]”
```
## Branch & Merge
```
git branch
git branch [branch-name]
git checkout
git merge [branch]
git log
```
## INSPECT & COMPARE
```
git log
git log branchB..branchA
git log --follow [file]
git diff branchB...branchA
git show [SHA]
```
## SHARE & UPDATE
```
git remote add [alias] [url]
git fetch [alias]
git merge [alias]/[branch]
git push [alias] [branch]
git pull
```
## TRACKING PATH CHANGES
```
git rm [file]
git mv [existing-path] [new-path]
git log --stat -M
```
## REWRITE HISTORY
```
git rebase [branch]
git reset --hard [commit]
```
## IGNORING PATTERNS
```
logs/*.notespattern*/
```
```
git config --global core.excludesfile [file]
```
## TEMPORARY COMMITS
```
git stash
git stash list
git stash pop
git stash drop
```
