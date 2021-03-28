**check commit information, just use 4 to 5 sha1 code**  
`$ git show dc463`  

**reference the parent commit, ^ means current commit's parent commit**  
**below command show last commit**  
`$ git show HEAD^`  
**you can add a number after ^, means the last n commit. but this only works in merges commit, because merge commit has multiple parent commit**  
`$ git show a7263^2`  

**another method to reference to parent is ~, below is the same**  
`$ git show HEAD^`  
`$ git show HEAD~`  
**but you can add number after ~ to reference to nth parent, like HEAD~2 means HEAD parent's parent**  
`$ git show HEAD~2`  
**below is the same**  
`$ git show HEAD^^^`  
`$ git show HEAD~3`  

**check all the commit that chould get from <branch1> but cannot get from <branch2>**  
`$ git log <branch2>..<branch1>`    
`$ git log origin/<branch>..HEAD`  
`$ git log origin/<branch>..`  

**check all the commits in <branch1> or <branch2> but not in <branch3>**  
`$ git log <branch1> <branch2> ^<branch3>`  
`$ git log <branch1> <branch2> --not <branch3>`  

**check all not both commit in <branch1> and <branch2>**    
`$ git log --format=oneline  --left-right <branch1>...<branch2>`  

**stash current work space. only tracked file will be stashed, add -u to stash untracked file**  
`$ git stash`  
`$ git stasu -u`  
**check stash list**    
`$ git stash list`  
**return stash content, default apply the last one. note that in powershell, {} is not correct, should use 'stash@{1}'**  
`$ git stash apply`  
`$ git stash apply @{n}`  
**delete stash content**  
`$ git stash drop @{n}`  

**stash the file that not staged**  
`$ git stash --keep-index`  

**create a new branch based on last stash, you must commit the same file which was modified in current branch but not commit in stash, the stash will be dropped when branch created**  
`$ git stash branch`   

**clean the untracked file, add -n to preview what was done, or add -i by using interactive mode**
**-d means clean the sub folder**  
`$ git clean -n -d`  
`$ git clean -d -f -i`  
**git clean only delete untracked file that not matched in .gitignore, if want to delete all untracked file, add -x**  
`$ git clean -n -d -x`  

# Search in file  
**search file, -n means display line number**  
`$ git grep -n <key word>`  
**--count means how many matched in file**  
`$ git grep --count <key word>`  
**search the key word in which method or function**  
`$ git grep -p <key word> *.cs`
**search by multiple string, --break and --heading will format the out put to make more clear**  
`$ git grep --break --heading -n -e '<key word>' --and -e '<key word>'`  
**search in old version**  
`$ git grep --break --heading -n -e '<key word>' --and -e '<key word>' v1.x.x`  

# Search in log  
**git log -S to display commit that add or delete the key word**  
`$ git log -S <key word> --oneline`  
**display the change log(as patch) of the function in that file, note that the file path should be correct like ./src/services/accountInfo.js or /Users/jason/Repository/pro-git/ch07/git-tools.md**   
`$ git log -L :<function name>:<file path> `

# Re-write history
**modify last commit, this will create a new sha1, like rebase, don't use this in the pushed branch**  
`$ git commit --amend`  

**re-write all the commit by script, use --all to implement this in all the branches**  
`$ git filter-branch --tree-filter 'rm -f password.txt' HEAD` 
