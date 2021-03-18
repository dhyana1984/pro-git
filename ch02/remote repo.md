**display remote repo, origin is the default remote repo name by git**  
`$ git remote`  
`$ git remote -v #display the remote repo url`  

**add remote repo**  
`$ git remote add [shortname] [url]`  
`$ git fetch [shortname] # to get the code and branches`  

**get data from remote repo. the diffrentce between git pull is that git fetch will not merge remote code automatically but git pull will do that. git clone will pull data from remote and set master branch to track the remote master banch**  
`$ git fetch [remote-name]`  

**check remote repo information**  
`$ git remote show [remote-name]`  

**rename local remote repo， please note this will change remote repo branch name**  
`$ git remote rename [ol-dname] [new-name]`  

**remove repo**
`$ git remote rm origin`