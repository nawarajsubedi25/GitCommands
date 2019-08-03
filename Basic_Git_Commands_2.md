### Basic Git Commands 2
~~~~~~
1. To check URL 
   git config remote.origin.url
~~~~~~~~~
~~~~~~~~~~~~~~
2. To Add URL 
-> Note use https for using gitbash
   git remote add origin git@github.com:nawarajsubedi25/REGISTRATION_FOR_MWMCVB-.git
~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~
3. To Set URL 
   git remote set-url origin git@github.com:roshankoirala05/g2-poc.git
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
4. To Create new branch and Push 
   Note: It will delete your all previous commit 
   git push -f origin Nawaraj
   **************************************************
   To push in your branch 
   git push -u origin Nawaraj
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 5. Specific error when merging 
    Error in  nawarajsubedi25:~/workspace (Nawaraj) $ git pull origin Nawaraj
    Warning: Permanently added 'github.com,192.30.253.113' (RSA) to the list of known hosts.
    From github.com:roshankoirala05/g2-poc
     * branch            Nawaraj    -> FETCH_HEAD
    fatal: refusing to merge unrelated histories
    $ git pull --allow-unrelated-histories origin Nawaraj
    *******************************************************************************************
    Warning: Permanently added 'github.com,192.30.253.112' (RSA) to the list of known hosts.
    From github.com:roshankoirala05/g2-poc
     * branch            Nawaraj    -> FETCH_HEAD
    Auto-merging js/markerclusterer.js
    CONFLICT (add/add): Merge conflict in js/markerclusterer.js
    Auto-merging js/index.js
    CONFLICT (add/add): Merge conflict in js/index.js
    Auto-merging index.php
    CONFLICT (add/add): Merge conflict in index.php
    ******************************************************************************************
    --> choose the file from the source branch and reject any changes from your current branch
    $ git checkout --theirs file_name  

    --> reject any changes from the source branch using command:
    $ git checkout --ours file_name
    nawarajsubedi25:~/workspace (Nawaraj|MERGING) $ git checkout --ours index.php
    nawarajsubedi25:~/workspace (Nawaraj|MERGING) $ git checkout --ours Registration.php
    nawarajsubedi25:~/workspace (Nawaraj|MERGING) $ git checkout --ours js/index.js
    nawarajsubedi25:~/workspace (Nawaraj|MERGING) $ git checkout --ours js/markerclusterer.js
    $ git add
    $ git commit -m "Autofill city, state and country after typing zipcode"
    $ git push -u origin Nawaraj
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~
6. create a new repository on the command line
    echo "# formValidationWithJquery" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git remote add origin git@github.com:nawarajsubedi25/formValidationWithJquery.git
    git push -u origin master
    **********************************************************************************
    or push an existing repository from the command line
    git remote add origin git@github.com:nawarajsubedi25/formValidationWithJquery.git
    git push -u origin master
~~~~~~~~~~~~~~~~~~~~~~
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
7. Completely remove the last commit 
    git reset -- hard 918cc06 
    git push – force origin master 
    or 
    git reset – hard HEAD^
    git push – force origin master 
    ************************************************
    Undo last commit before push or edit last commit 
    git reset HEAD^
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

