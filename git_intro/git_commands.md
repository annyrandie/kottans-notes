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
    $ git commit --amend (modify last commit)
    $ git revert <SHA-of-commit-to-revert> (undo the changes that were made by the provided commit, creates a new commit to     record the change )
    
    
_*resetting commits*_

    $ git reset <reference-to-commit> (reset commit)
    $ git reset --mixed HEAD^ (unstage changes - move changes to working directory)
    $ git reset --soft HEAD^ (move changes directly to the Staging Index.)
    $ git reset --hard HEAD^ ( takes the changes made in commit and erases them.)
    
    
    ^ – indicates the parent commit
    ~ – indicates the first parent commit
      
    
_*git log*_

    $ git log
    $ git log --oneline (SHA and message)
    $ git log -p
    $ git log --decorate (shows description of commits)
    $ git log --oneline --decorate (display also branches)
    $ git log --oneline --decorate --graph --all (shows all branches and commits in the repository)
    
_*git tag*_

    $ git tag -a v1.0
    $ git tag
    $ git tag -d v1.0  (delete tag)
    $ git tag -a v1.0 <SHA> (to tag a commit that occurred farther back in the repo's history)
    
_*git branching*_

    $ git branch (list all branches)
    $ git branch backup (make a safe backup)
    $ git branch <branch name> (create a branch)
    $ git checkout <branch name> (checkout to a branch)
    $ git branch <branch name> SHA (create a branch from definite commit)
    $ git branch -d <branch name> (delete branch)
    $ git checkout -b <branch name> (create and checkout to a branch)
    $ git checkout -b <branch name1> <branch name1> (create and checkout the branch <branch name1> starting with <branch name2>)
    
_*git merge*_

    $ git merge <name-of-branch-to-merge-in>
    $ git reset --hard HEAD^ (undo the merge)
    
      
  ## Work with remote repozitories on github  
    
_*git remote *_

    $ git remote add origin <URL> (is used to add a connection to a new remote repository)
    $ git remote -v (is used to see the details about a connection to a remote)
    $ git remote rename <current name> <new name> (rename remoute repository)
    
_*push to remote*_

    $ git push origin master ($ git push <remote-shortname> <branch>) (to send commits from a local repository to a remote repository)
    
    to avoid SSL: GIT_SSL_NO_VERIFY=true git push origin master
    
_*git pull*_

    $ git pull origin master
    
    to avoid SSl: GIT_SSL_NO_VERIFY=true git pull origin master
    
_*git log*_

    $ git log --stat (to show information about changes)
    
_*git fetch*_

    $ git fetch upstream master (to get the changes from upstream remote repository)
    
_*git rebase*_

    $ git rebase -i HEAD~3 (squash 3 commits)

### Rebase Commands

    Let's take another look at the different commands that you can do with git rebase:

    - use p or pick – to keep the commit as is
    - use r or reword – to keep the commit's content but alter the commit message
    - use e or edit – to keep the commit's content but stop before committing so that you can:
        - add new content or files
        - remove content or files
        - alter the content that was going to be committed
    - use s or squash – to combine this commit's changes into the previous commit (the commit above it in the list)
    - use f or fixup – to combine this commit's change into the previous one but drop the commit message
    - use x or exec – to run a shell command
    - use d or drop – to delete the commit


    
    
    





