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
