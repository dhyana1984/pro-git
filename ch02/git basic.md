**track and manage current project**  
`$ git init`

**clone project to other folder**  
`$ git clone <url> myfolder`

**display the simple status**  
**untracked file: ??**  
**Staged file: A**  
**Modified: M**      
`$ git status -s(or --short)`

**.gitignore**
**/TODO ignore current TODO folder but not sub TODO folder**
**build/ ignore all files in build folder**

**git diff check files which was committed**
**git diff check all the files which not add to stage**  
`$ git diff`

**check all the  files already added to stage**
`$ git diff --staged`
`$ git diff --cached`  

**display the diff information but remove the diff detail and only keep the comment when close diff editor**  
`$ git diff -v`

**remove file track without deleting file**  
`$ git rm --cache <filename>`  


