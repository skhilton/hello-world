---
layout: default
title: rebase
parent: github
has_children: true
nav_order: 3
---

# [Squash two commits together](https://github.com/todotxt/todo.txt-android/wiki/Squash-All-Commits-Related-to-a-Single-Issue-into-a-Single-Commit)

I made added and committed a file that said “points change to correct color” (commit A) continued coding and committing and then realized that I forgot to add a file to the “point change to correct color” commit. I had already pushed all of the changes.

I added, committed, and pushed the file I missed (commit B) and then
1. `git rebase -i HEAD~7` where 7 is one commit back from commit A  
2. changed the order of the commits so that commit B follows commit A directly  
3. Changed `pick` to `squash` for commit B  
4. closed the file  
5. `git push origin brush-selection --force` where brush-selection is my working branch
6. 
Another use for this series of commands is to clean up your git history.  
