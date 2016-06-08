

**********************

# To download, install, and setup Git

1. Sign up for a Github account

2. Download and install latest version of [Git](https://git-scm.com/downloads)

3. (Optional*) Download and install [Git Extensions](https://sourceforge.net/projects/gitextensions/)(*Download this if you're on a Windows machine and would like to use Git Bash or Powershell rather than the Windows Prompt, or if you'd like some of the other functionality described at the website.)

4. Configure Git to remember your username and email

    `git config --global user.name "[yourUserName]"`

    `git config --global user.email "[yourEmailAddress]"`

**********************

# To clone a repository (make a local copy)

1. Navigate to directory in which you'll store your repo

    `cd [myPathToParentFolder]`

2. Clone/copy the repo

    `git clone [repoURL]`

3. Navigate to your local Repo folder

    `cd [myPathToRepo]`

**********************

# To create and switch between branches

1. See which branch you're currently on, and which are available

    `git branch`

2. Create a new branch (named 'yourBranch')

    `git checkout -b [yourBranch]`

3. Switch to a different branch (e.g., to Master)

    `git checkout Master`

**********************

# To make changes in yourBranch

1. Update your copy of Master branch (sync it with remote copy)

    `git checkout Master`  (if you're not already on Master branch)
    `git pull`

2. Create or switch to yourBranch (see above)

3. Do your work -- Add, Edit, and Delete files in the repo

4. Check status of yourBranch

    `git status`

5. Commit your changes (added and edited files) to yourBranch

    `git add --all`
    `git commit --all -m "[myCommitMessage]"`

6. Update git's remote copy of your Branch (sync local and remote)
 
    `git checkout [yourBranch]` (if you're not already on it)
    `git push`  (Note that if a remote copy of yourBranch does not yet exist, a message will tell you the command to create it.)

**********************

# To merge work done in yourBranch into the Master branch

1. Navigate to github.com and the appropriate repo
2. Compare Master branch with yourBranch
3. Create a Pull Request and Merge
4. Confirm Merge
5. (Hopefully you won't have to) Deal with any conflicts

**********************

# Some other useful commands

`pwd`  (Lists directory you're currently in)

`ls -a`  (Lists all files in current directory, including hidden ones)

`git checkout -- .`  (Discards all **unstaged** changes made in local branch (to indexed/tracked files))

`git checkout .`  (Discards **ALL** changes (staged and unstaged) made in local branch (to indexed/tracked files))

**********************


