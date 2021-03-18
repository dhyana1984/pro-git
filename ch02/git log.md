**list all the log history, the latest in the top**
`$ git log`  
**-p will display the diff in each commit, -2 means display the latest 2 commit**  
`$ git log -p -2`  

**--pretty can change the log out put format**  
`$ git log --pretty=oneline`  

**--pretty=format can define the log out put log**  
`$ git log --pretty=format:"%h - %an, %ar : %s"`  

**out put using customized format and graph**   
`$ git log --pretty=format:"%h %s" --graph`  

**--since or --after to out put the log after that date**  
`$ git log --since= 2.weeks` 

**--until or --before to out put the log before that date**  
`$ git log --since= 2.weeks` 

**-S(string look for)**  
`$ git log -S <function_name>`

**--author find the author's commit, --grep find key word in commit information**  

**to add a path or filename to out put log only for that path or filename. but this should be in the end of command with -- , the space in front and end of --**  
`$ git log -p -- testfolder/testoutput`
`$ git log -p -- test.txt`