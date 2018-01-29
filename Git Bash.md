# GIT BASH COMMANDS

### CONFIG
  Configure the author name and email address to be used with commits.

    git config --global user.name "Sam Smith"
    git config --global user.email sam@example.com

### INIT
  _Create a new local repository._
    `git init`

### CLONE
  Check out a repository.  
  *Create a working copy of a local repository:*
    `git clone /path/to/repository`
  *For a remote server*
    `git clone username@host:/path/to/repository`

### STATUS
  _List the files you've changed and those you still need to add or commit_
    `git status`

### ADD
  _Add one or more files to staging (index)_
    `git add <filename>
    git add .`

### COMMIT
  *Commit changes to head (but not yet to the remote repository):*
    `git commit -m "Commit message"`

  *Commit any files you've added with git add, and also commit any files you've changed since then:*
    `git commit -a`

### PUSH
  _Send changes to the master branch of your remote repository:_
    `git push origin master`

### REMOTE
  _If you haven't connected your local repository to a remote server, add the server to be able to push to it:_
    `git remote add origin <server>`

  _List all currently configured remote repositories:_
    `git remote -v`

### BRANCHES
  _Create a new branch and switch to it:_
    `git checkout -b <branchname>`

  _Switch from one branch to another:_
    `git checkout <branchname>`

  _List all the branches in your repo, and also tell you what branch you're_ currently in:
    `git branch`

  _Delete the feature branch:_
    `git branch -d <branchname>`

  _Push the branch to your remote repository, so others can use it:_
    `git push origin <branchname>`

  _Push all branches to your remote repository:_
    `git push --all origin`

  _Delete a branch on your remote repository:_
    `git push origin :<branchname>`

  _Rename a branch:_
    `git branch -m <new branch name>`
    `git branch -m <old branch name> <new branch name>`
