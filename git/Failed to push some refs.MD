
## Error on push command
You made  
```
git push origin main returns:
```
and you reveided:  
```
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/monica-gatti/SparkPrj'
```
The cause may be a different branch name ( typically main vs master)
To fix it, check the branch

```
git branch -v 
```
to list the local branch.

```
git branch
```
To show the current local branch
If the name differs, do:
```
git branch -m master main
```
To rename local branch "master" in "main"

When you retry the git pull
```
git pull origin main
```
may be you get this error:
```
return "fatal: refusing to merge unrelated histories"
```
So, use:
git pull origin main --allow-unrelated-histories
