**check trailing whitespace, run this before commit**  
`$ git diff --check`  

**push to server repo as up stream branch**  
`$ git push -u origin <branch>`  

**git commit -am is cannot apply to the new created file, just apply to the exists change**  
`$ git commit -am <commit message>`  
**equals to**  
`$ git add .`    
`$ git commit -m <commit message>`