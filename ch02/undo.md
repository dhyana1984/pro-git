**fix last commit. below sample will create 1 commit but add the forgotten file to the first commit**  
`$ git commit -m 'first commit'`  
`$ git add forgoten file`  
`$ git commit --amend`  

**move file out of stage**  
`$ git reset HEAD file`  

**revert the file which is modified. this is very dangous, the file will overwrite. any commit change could be back but change which not commit cannot be back if lost**  
`$ git checkout -- file`  

**in fact, git status will display those comand**  
```
On branch study
Your branch is up to date with 'origin/study'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ../../undo.md

nothing added to commit but untracked files present (use "git add" to track)
```

