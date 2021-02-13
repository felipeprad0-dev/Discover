# Innitial settings 
    
    This configuration will be done only once by the computer and the effect will remain after updates. 
    We can change them at any time running these commands again.

# Identity 
    With git installed, open the terminal and type: 
        `git config --global user.name "Nome Completo Aqui"`
        `git config --global user.email email@aqui`

    This setting is important because each commit will use this information, stamping immutably on the commits created. 
    To replace this information with a different name for a specific project, run the command without the `--global` option within that project.

# Editor 
    There is the option to change the default editor (vim) to another
    `git config --global core.editor "code -w"`

# Show settings 
    Can check the settings with the command below
    `git config --list` 



# GIT CONFIG 
    * Allows to see and to assign configuration variables such as name and email.
    * These variables can be stored in three different places: 
      1. /etc/gitconfig: valid for all users on the system and all repositories. If you pass the option`--system` to `git config`, it reads and writes to this file. 
      2. ~/.gitconfig ou ~/.config/git/config: only for own user. You can make Git read and write to this file by passing the option `--global`.
      3. config in the directory Git (that is, .git/config) of any repository you are using: specific to this repository.

    Each level overrides the values ​​in the previous level, that is, values ​​in .git / config prevail over etc / gitconfig.


## Git Help 
    `git help` open a help menu, which can be considered the Git manual.