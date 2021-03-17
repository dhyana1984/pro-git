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