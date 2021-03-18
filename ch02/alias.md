**create alias**  
`$ git config --global alias.unstage 'reset HEAD --'`  

```
$ git unstage fileA
// the same as
$ git reset HEAD --fileA 
```

`$ git config --global alias.last 'log -1 HEAD'`
```
$ git last
// the same as
$ git log -1 HEAD
```

**if create alias for external command rather than git system command, need to add !**  
`$ git config --global alias.visual '!gitk'`