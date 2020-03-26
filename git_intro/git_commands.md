# Git commands

_*Config git*_

    $ git cofig --list (all list of configuration)
    $ git config --global user.name "Hanna Pereverzieva"
    $ git config --global user.email myemail@example.com
    $ git config --global core.editor <your-editor's-config-went-here>
    $ git config --global core.editor "code --wait"


_*Init git repo*_

    $ git init
    
        ls - used to list files and directories
        mkdir - used to create a new directory
        cd - used to change directories
        rm - used to remove files and directories
        touch <file> - add file to project folder
    
    
_*Clone repo*_

    $ git clone 'url'
    
    $ git clone 'url' 'directory'
    
_*git status*_

    $ git status
    
    $ git log
    
    $ git diff (to see changes that have been made but have not been committed)
    
_*add to staging index*_

    $ git add <file1> <file2> … <fileN> (specific file)
    $ git add . (all files)
    
    $ git rm --cached <file>..." (to unstage file)

_*git commit*_

    $ git commit
    $ git commit -m "message"
    
_*git log*_

    $ git log
    $ git log --oneline (SHA and message)
    $ git log -p
    $ git log --decorate (shows description of commits)
    
_*git tag*_

    $ git tag -a v1.0
    $ git tag
    $ git tag -d v1.0  (delete tag)
    $ git tag -a v1.0 <SHA> (to tag a commit that occurred farther back in the repo's history)
    





