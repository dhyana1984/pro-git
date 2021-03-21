**check trailing whitespace, run this before commit**  
`$ git diff --check`  

**push to server repo as up stream branch**  
`$ git push -u origin <branch>`  

**git commit -am is cannot apply to the new created file, just apply to the exists change**  
`$ git commit -am <commit message>`  
**equals to**  
`$ git add .`     
`$ git commit -m <commit message>`  

**create branch and set up stream**  
`$ git checkout -b <branch> origin/<remote branch>`  

**pick commit**  
`$ git cherry-pick <sha1 code>`  

**release flow**  

**1.add tag**  
`$ git tag -s v1.5 'release note'`  
**2.get the version, like v1.6.2-rc1-20-g8c5b85c, the latest tag and commit count and sha1**  
`$ git describe master`  
**3.get the archive or building, git will generate the .tar or .zip file**  
```
$ git archive master --prefix='project/' | gzip > `git describe master`.tag.gz
$ git archive master --prefix='project/' --format=zip > `git describe master`.zip
```

两个反引号 空格 反引号uvm 空格 两个反引号