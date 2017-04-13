# Intro to Git and GitHub

The slides are available here: http://slides.com/kirschbombe/git-7/fullscreen

You will need to install Git: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

If you want to use the Cloud9 IDE for this workshop, Git is preinstalled on these cloud-based Linux development environments. https://c9.io/ (signup is free, but requires a credit card)

You will also need a GitHub account. You can get one here: https://github.com

### Bash commands we'll use
* `cd` : change directory
* `cd ..` : move up to the parent directory
* `touch` : create new file here
* `pwd` : print working directory
* `cat` : "concatenate", used to print the contents of a file

### Basic git commands for working on our local repo
* `git init` : initialize a new git repo
* `git status` : lists files/folders that are unstated/staged, untracked, deleted - do this often!
* `git add` : add specified file(s) to staging
* `git add .` : add all edited files to staging
* `git commit -m “commit message”` : commits all staged changes (hint: Keep related changes together in one commit. Commits allow you to roll back and track your work, so try to commit every time you complete a task.)
* `git log` : prints a log of your commit history

### Git commands for working with branches
* `git branch [name]` : creates new branch
* `git checkout [branch name]` : switches to branch
* `git merge [branch to be merged]` : merge commits into current branch
* `git branch` : lists all branches
* `git branch -d [branch name]` : delete branch

### Git commands for working with remotes
* `git clone` : clone a remote repo to local
* `git push` : pushes commits to remote repo
* `git pull` : pull commits from remote repo
