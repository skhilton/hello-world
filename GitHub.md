---
layout: page
title: Github
permalink: /github/
---
* TOC
{:toc}
## New Branch
### [creating a new branch](https://www.freecodecamp.org/forum/t/push-a-new-local-branch-to-a-remote-git-repository-and-track-it-too/13222)

```
git checkout -b feature_branch_name
git push -u origin feature_branch_name
```

### [creating a local copy of a new remote branch](https://www.git-tower.com/learn/git/faq/checkout-remote-branch)

There may be a remote branch on github that is not on your local machine.
To checkout this branch use:  

```
git checkout --track origin/feature_branch_name
```

### [stashing changes to switch branches](http://www.codeblocq.com/2016/02/Stash-your-changes-before-switching-branch/)  

on the development branch  
```
git stash save "message"  
git checkout master   
git chckout development-branch   
git stash pop  
```

### [delete a branch](https://koukia.ca/delete-a-local-and-a-remote-git-branch-61df0b10d323)
```
git branch -d branch_name
git branch -D branch_name
```

## Rebase
### [Squash two commits together](https://github.com/todotxt/todo.txt-android/wiki/Squash-All-Commits-Related-to-a-Single-Issue-into-a-Single-Commit)

I made added and committed a file that said “points change to correct color” (commit A) continued coding and committing and then realized that I forgot to add a file to the “point change to correct color” commit. I had already pushed all of the changes.

I added, committed, and pushed the file I missed (commit B) and then
1. `git rebase -i HEAD~7` where 7 is one commit back from commit A  
2. changed the order of the commits so that commit B follows commit A directly  
3. Changed `pick` to `squash` for commit B  
4. closed the file  
5. `git push origin brush-selection --force` where brush-selection is my working branch

Another use for this series of commands is to clean up your git history.  
