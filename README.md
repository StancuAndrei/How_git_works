# How_git_works

#After instalation of GIT, you need to configure it:
  - **git config --global user.name "username"**
  - **git config --global user.email "you email"**
(optional: make notepad++ default editor)
**HEAD** - kind of a '_pointer_' hat points to last commit of the current branch

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

#Advanced GIT commands (branching, mergin, etc):
  - **git dif 'one commit hash code' '2nd comming hash code'** - shows difference between these commits, what was changed, etc
  - **git checkout -b 'branch name'** - creates a new branch, different than the master/main branch and also moves you to the newly created branch
  - **git checnout 'branch name'** - moves to a different branch
  - **git merge 'name of the branch that u want to merge'** - while on master branch use this command to merge the updates from a different branch
  - **git tag 'tag name'** - creates a tag for the latest commit  **git tag -d 'tag name'** - deletes the tag
  - **git tag -a v1.0 -m 'release 1.0'** - create a annoted tag named v1.0 with a message
  - **git stash** - saves progress in a stash
  - **git reset 'commit id' --soft** - one way of reseting ( least destructive of them all) changes where HEAD is pointed = there is also --mixed which is default/ --hard = any changines and stuff on staging area wipes out all of them
  - 
