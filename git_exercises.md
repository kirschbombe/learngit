## Git exercises

### A new Git repository

In your Bash shell (Terminal, Babun), verify that you are in your Home directory using the `pwd` command (print working directory)
```bash
$ pwd
/Users/kirschbombe
```
1. To verify that we are not currently in a Git directory, we can use `git status`
```bash
$ git status
fatal: Not a git repository (or any of the parent directories): .git
```
2. Let's create a new project folder named `oceans` and initialize it as a Git repository
```bash
$ git init oceans
Initialized empty Git repository in /Users/kirschbombe/oceans/.git/
```
Using `git init oceans` creates the new folder "oceans" and initializes it as a git repository at the same time. We could also navigate into any existing directory and use `git init` to turn it into a git repo.

3. Now let's check that our new directory is there and move into it using the `ls` and `cd` commands
```bash
$ ls
oceans
$ cd oceans
$ pwd
/Users/kirschbombe/oceans
```

4. Right now there is nothing (except our .git file) in our directory, so let's create a new file named `pacific.txt` using the `touch` command
```bash
$ touch pacific.txt
$ ls
pacific.txt
```

5. 
Stage your changes:  git add . or git add [filename]
Commit your changes:  git commit -m "commit message"
Repeat 3-5
View your commit history: git log
