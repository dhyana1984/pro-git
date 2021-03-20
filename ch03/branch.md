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