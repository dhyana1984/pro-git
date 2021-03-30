**save data to .gi, -w ask hash-object save the data, or hash-object only return key --stin read content from stdin, hash-object request add a file path at the end if without --stin**  
`$ echo 'test content' | git hash-object -w --stdin`  

**git cat-file -p d670460b4b4aece5915caf5c68d12f560a9fe3e4 display file content**  
`$ git cat-file -p d670460b4b4aece5915caf5c68d12f560a9fe3e4`

**use git cat-file -t to get the type of the file, git save the file as blob**
`$ git cat-file -t 1f7a7a472abf3dd9643fd615f6da379c4acb3e3a`