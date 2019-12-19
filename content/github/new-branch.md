---
layout: default
title: new branch
parent: github
nav_order: 2
---

# [creating a new branch](https://www.freecodecamp.org/forum/t/push-a-new-local-branch-to-a-remote-git-repository-and-track-it-too/13222)

```
git checkout -b feature_branch_name
git push -u origin feature_branch_name
```

# [creating a local copy of a new remote branch](https://www.git-tower.com/learn/git/faq/checkout-remote-branch)

There may be a remote branch on github that is not on your local machine.
To checkout this branch use:  

```
git checkout --track origin/feature_branch_name
```

# [stashing changes to switch branches](http://www.codeblocq.com/2016/02/Stash-your-changes-before-switching-branch/)  

on the development branch  
```
git stash save "message"  
git checkout master   
git chckout development-branch   
git stash pop  
```

# [delete a branch](https://koukia.ca/delete-a-local-and-a-remote-git-branch-61df0b10d323)
```
git branch -d branch_name
git branch -D branch_name
```
