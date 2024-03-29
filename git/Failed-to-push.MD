
# Failed to push error

I receive  this error when pull-push-fetch:
_error: failed to push some refs to 'https://github.com_

To solve:

```
git reset 
git remote -v
git pull --rebase
git init
git add -A
git commit -m "Add your commit"
git branch -M main
git push origin main --force
```

## What are we doing?
- git reset: Git reset is primarily used to undo the staging index changes
- git remote -v : view connection with repository
- git pull --rebase: The git pull and git rebase are almost similar with some differences. You may have already heard of git fetch command which will fetch down all 
the changes from the remote repository server to your local workstation that you don’t have yet, it will not modify your working directory at all. 
It will simply get the data for you and let you merge it yourself. Next you can use git merge to merge the changes. Now instead of performing this git fetch 
followed by git merge, you can directly use git pull.
The git rebase is sort of an alternative to merge functionality. Instead of creating a new commit that combines the two branches, the git rebase moves the commits 
of one of the branches on top of the other.
See https://www.golinuxcloud.com/git-pull-vs-git-pull-rebase/

- git add -A : adds a change in the working directory to the staging area. ( -A = all)
