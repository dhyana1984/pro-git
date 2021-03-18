**search the matched pattern**
`$ git tag -l "v1.2.*"`

**lightweight tag is like a branch, pointer to a commit, annotated tag includes many information, author, email create time, tagging message. GPG can signature and validate on it.**  
**create annotated tag by -a option**    
`$ git tag -a v1.4 -m "my version 1.4"`    
**check the tag and commit**    
`$ git show v1.1`
**create lightweight tag**  
`$ git tag v1.1-lw`
**add tag to the old commit**  
`$ git log --pretty=oneline`
`$ git tag -a v1.3 [SHA value]`    

**git push will not push tag to remote, you have to push tag like push branch**
`$ git push origin v1.1`
`$ git push origin --tags # push all tag`  

**create branch base on a tag**  
`$ git checkout -b version2 v0.9`
