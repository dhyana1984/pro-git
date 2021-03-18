**git config folder, 3 override 2, 2 override 1**  
1. /etc/git config: all the user and repository values in system  
2. ~/.gitconfig or ~/.config/git/config: yourself use --global option to write or read variable
3. .git/config: config file in current project
In windows, git is in $HOME(c:\User\$USER)

**setup idendity information**  
`$ git config --global user.name "<username>"`  
`$ git config --global user.email "<email>"`  

**setup personal editor**  
`$ git config --global core.editor vscode`  
`$ $ git config --global core.editor "'c:/Program Files/Notepad++/notepad++.exe'" -multiInst -nossesion`  

**check config**  
`$ git config --global`
`$ git config <key>`