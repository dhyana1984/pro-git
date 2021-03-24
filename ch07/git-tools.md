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

**stash current work space. new file will not be stashed, should add to stage first**  
`$ git stash`  
**check stash list**    
`$ git stash list`  
**return stash content, default apply the last one. note that in powershell, {} is not correct, should use 'stash@{1}'**  
`$ git stash apply`  
`$ git stash apply @{n}`  
**delete stash content**  
`$ git stash drop`  