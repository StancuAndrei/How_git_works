# How_git_works

#After instalation of GIT, you need to configure it:
  - **git config --global user.name "username"**
  - **git config --global user.email "you email"**
(optional: make notepad++ default editor)

#Commands:
  - **git init** - initializez a new git repository
  - **git status** - checks the status
  - **git add (file name)** - saves the changes made ( can use '**git add .**' to save all files )
  - **git comming -m "commit message"** - makes commit of the changes
          - -m = leaves a message
          - -a = commits the changes while adding the latest file changes
  - **git init .** - initaite repo for existing project
  - **git log** - lists all the changes that were made
  - **git show** - shows last commit info
  - **git ls-files** - lists all files tracked by git
  - **git reset HEAD "file name"** - unstage the changes of the file ( doesnt reset the changes ON the file BUT the commit for that change )
  - **git checkout -- "file name"** - resets the last changes made to a file ( works with the COMMAND ABOVE (git reset.. ) )
  - **git help 'log/commit/status'"** - lists parameteres to combine and do different stuff for e.g **git log --oneline -- graph --decorate --all** )
  - **git config --global alias._hist_ "log --oneline -- graph --decorate --all** - makes an alias, kind of a shortcut, which is global, can be invoked like **git hist**

#Renaming and deleting files with GIT:
  - **git mv "file name" "new name"** - _moves_ the name of that file to another name, bassicaly changes the name
  - **git rm "file name"** - removes the file
  - 
