## Git exercises

### Configuring Git
We do this by setting a couple of options in a file found in your home directory

```bash
git config --global user.name "Firstname Lastname"
git config --global user.email username@company.extension
```

Your name and email address is included in every change that you make, so it's easy to keep track of who did what

Also, unless you are a vimwizard, I would recommend changing your default editor to nano

```bash
git config --global core.editor nano
```

If you have a different favorite editor, you can type in the appropriate
command from the table below:

| Editor             | Configuration command                            |
|:-------------------|:-------------------------------------------------|
|Atom | `$ git config --global core.editor "atom --wait"`|
| nano               | `$ git config --global core.editor "nano -w"`    |
| Text Wrangler      | `$ git config --global core.editor "edit -w"`    |
| Sublime Text (Mac) | `$ git config --global core.editor "subl -n -w"` |
| Sublime Text (Win, 32-bit install) | `$ git config --global core.editor
"'c:/program files (x86)/sublime text 3/sublime_text.exe' -w"` |
| Sublime Text (Win, 64-bit install) | `$ git config --global core.editor
"'c:/program files/sublime text 3/sublime_text.exe' -w"` |
| Notepad++ (Win)    | `$ git config --global core.editor "'c:/program files
(x86)/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"`|
| Kate (Linux)       | `$ git config --global core.editor "kate"`       |
| Gedit (Linux)      | `$ git config --global core.editor "gedit -s -w"`   |
| emacs              | `$ git config --global core.editor "emacs"`   |
| vim                | `$ git config --global core.editor "vim"`   |

Make sure everything was entered correctly by typing `git config --list`

~~~{.output}
user.name=Dawn Childress
user.email=kirschbombe@gmail.com
core.editor=nano
~~~

### A new Git repository

First, verify that you are in your Home directory using the `pwd` command (print working directory)
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

4. Right now there is nothing (except our .git file) in our directory, so let's create a new file named `mammals.txt` using the `touch` command and edit the file using `nano`
```bash
$ touch mammals.txt
$ ls
mammals.txt
$ nano mammals.txt
```
This will open the file in nano. Let's add some content to our file:
```
dolphins
whales
seals
```
Use `CTRL + O` to write, and `CTRL + X` to exit.

Now let's see what git is up to with `git status`

~~~bash
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	mammals.txt

nothing added to commit but untracked files present (use "git add" to track)
~~~

Here, git is telling you that there are local files that you haven't told git to look at. Let's tell git to add our changes to the staging area using `git add`

~~~
$ git add mammals.txt
~~~

Now, when we run `git status`, git tells us that we've told it to keep track of a new file

~~~bash
On branch master

Initial commit

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   mammals.txt
~~~

If this was a mistake, we could correct it with `git rm`

5. 
Stage your changes:  git add . or git add [filename]
Commit your changes:  git commit -m "commit message"
Repeat 3-5
View your commit history: git log
