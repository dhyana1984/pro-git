**check the objec that each branch point to**  
`$ git log --oneline --decorate`

**check the commit history and branch by graph**  
`$ git log --oneline --decorate --graph --all`

**check the last commit in each branch**  
`$ git branch -v`  

**filter all branches are already merged to current branch**
`$ git branch --merged`


**filter all branches are NOT  merged to current branch**
`$ git branch --no-merged`

**cannot delete the branch that was not merged to master**
`$ git branch -d <brand>`
**force to delete the branch**
`$ git branch -D <brand>`


**change local branch name**
`$ git checkout -b <myname> origin/<remoteb ranch>`

**set up stream for branch**
`$ git branch -u origin/<remote branch>`

**use up stream in a simple way**
`$ git merge origin/master`
`$ git merge @{u}`

**check all the tracked branch, and the up stream for each branch**
`$ git branch -vv`

**delete remote branch**
`$ git push origin --delete <branch>`