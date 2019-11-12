### Basic Git Commands 1
~~~~~~
1. git config
   git config –global user.name “[name]”  
   git config –global user.email “[email address]”  
This command sets the author name and email address respectively to be used with your commits.
~~~~~~~
~~~~~~~
2. git clone
   git clone [url] 
This command is used to obtain a repository from an existing URL. URL should be in (https://)
   git clone --single-branch --branch <branchname> <remote-repo>
This will clone a specific branch (branchname). 
   or 
   git clone -branch new_feature git://remoterepository.git
This would clone only the new_feature branch from the remote Git repository.
~~~~~~~
~~~~~~~
3. git add
   git add [file]  
This command adds a file to the staging area.
   git add *  
This command adds one or more to the staging area.
~~~~~~~
~~~~~~
4. git commit
   git commit -m “[ Type in the commit message]”  
This command records or snapshots the file permanently in the version history.
   git commit -a  
This command commits any files you’ve added with the git add command and also commits any files you’ve changed since then.
~~~~~~~~
~~~~~~~~
5. git diff
   git diff  
This command shows the file differences which are not yet staged.
   git diff –staged 
This command shows the differences between the files in the staging area and the latest version present.
   git diff [first branch] [second branch]  
This command shows the differences between the two branches mentioned.
~~~~~~~~~~
~~~~~~~~~
6. git reset
   git reset [file]  
This command unstages the file, but it preserves the file contents.
  git reset [commit]  
This command undoes all the commits after the specified commit and preserves the changes locally.
  git reset –hard [commit] 
This command discards all history and goes back to the specified commit.
~~~~~~~~~~~
~~~~~~~~~~
7. git status
   git status  
This command lists all the files that have to be committed.
~~~~~~~~~~~~~
~~~~~~~~~~~~~~~
8. git rm
   git rm [file]  
This command deletes the file from your working directory and stages the deletion.
   git rm --cached [file] 
   Note: 
    If you just use rm, you will need to follow it up with git add <fileRemoved>.  git rm does this in one step.
    You can also use git rm --cached which will remove the file from the index (staging it for deletion on the next commit), 
    but keep your copy in the local file system.
~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~
9. git log
   git log  
This command is used to list the version history for the current branch.
~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~
10. git branch
    git branch  
This command lists all the local branches in the current repository.
    git branch [branch name]  
This command creates a new branch.
    git branch -d [branch name]  
This command deletes the feature branch.
    git branch -a
This will give the list of all branch. 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
11. git checkout
    git checkout [branch name]  
This command is used to switch from one branch to another.
    git checkout -b [branch name]  
This command creates a new branch and also switches to it.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
12. git merge
    git merge [branch name]  
This command merges the specified branch’s history into the current branch.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~
13. git remote
    git remote add [variable name] [Remote Server Link]  
This command is used to connect your local repository to the remote server.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~
14. git push
    git push [variable name] master  
This command sends the committed changes of master branch to your remote repository.
    git push [variable name] [branch]  
This command sends the branch commits to your remote repository.
   git push –all [variable name]  
This command pushes all branches to your remote repository.
   git push [variable name] :[branch name]  
   eg.
   Raj@Nawaraj MINGW64 ~/Desktop/CS6400-2019-03-Team40 (role_authentication)
   $ git push -u origin role_authentication

This command deletes a branch on your remote repository.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
15. git pull
    git pull [Repository Link]  
This command fetches and merges changes on the remote server to your working directory.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~
16. git stash
    git stash save  
This command temporarily stores all the modified tracked files.
    git stash pop  
This command restores the most recently stashed files.
    git stash list  
This command lists all stashed changesets.
    git stash drop  
This command discards the most recently stashed changeset
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~
17. If index lock 
    git rm -f ./.git/index.lock
    git init 
This will removed lock git 
~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~~~
18. To go to directory 
    cd [directory]
    ***********************
    Create directory
    mkdir user1
~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~
19. To create branch 
    git branch user1  
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
20. To checkout branch 
    Git checkout user1
    eg.
    $ git branch role_authentication

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
