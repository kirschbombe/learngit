## Setup

To participate in this workshop, you will need access to the software described below (Bash shell, Github account, Git command line tool, your favorite text editor). Options for Mac, Linux, and Windows are outlined below. In addition, you will need an up-to-date web browser.

### The Bash Shell    
Bash is a commonly-used shell that gives you the power to do simple tasks more quickly.

#### Windows
* Download the Babun Windows shell (http://babun.github.io).
* Run the installer using the steps bellow:
    * Unzip the downloaded file and double-click the `install.bat` file to install the program.
    * This will open a shell window and begin installation.
    * When install is complete, you will see a message that your program has installed successfully :)

**Optional: Set your HOME directory in Babun to your Windows user home folder**
The default HOME directory for Babun is set to a sub-folder in your Windows Home directory - something like: `C:\Users\[username]\.babun\cygwin\home\[username]`
To set your Babun HOME directory to `C:\Users\[username]`, follow these steps:
* From your Babun shell, execute `rundll32 sysdm.cpl,EditEnvironmentVariables` or search in the Start menu for `env` and select "Select Edit environment variables for your account”
* Select “New”
    * Name: HOME
    * Value: `C:\Users\[username]`
    * Click on “OK”
* Click on “OK” again
* In Babun, run `babun install`
* Restart Babun. Your HOME directory should now be you Windows user directory.

Babun will provide you with both Bash and Git already installed.

#### Mac OS X
The default shell in all versions of Mac OS X is Bash, so no need to install anything.  You access Bash from the Terminal (found in `/Applications/Utilities`). See the Git installation [video tutorial](https://www.youtube.com/watch?v=9LQhwETCdwY) for an example on how to open the Terminal. You may want to keep Terminal in your dock for this workshop.

#### Linux
The default shell is usually Bash, but if your machine is set up differently you can run it by opening a terminal and typing `bash`.  There is no need to install anything.

### Git and a GitHub account
Git is a version control system that lets you track who made changes to what when and has options for easily updating a shared or public version of your code on https://github.com/. You will need a [supported](https://help.github.com/articles/supported-browsers/) web browser (current versions of Chrome, Firefox or Safari, or Internet Explorer version 9 or above).

You will need an account at https://github.com/ for this workshop. Basic GitHub accounts are free. We encourage you to create a GitHub account if you don't have one already. Please consider what personal information you'd like to reveal. For example, you may want to review these [instructions for keeping your email address private](https://help.github.com/articles/keeping-your-email-address-private/) provided at GitHub.

#### Windows
Git should be installed on your computer as part of your Babun Windows shell install (described above).

#### Mac OS X and Linux
Git should already be installed on most Mac and Linux machines. Here are instructions for verifying that it is installed and for installing/updating: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

### Text Editor
When you're writing code, it's nice to have a text editor that is optimized for writing code, with features like automatic color-coding of key words. The default text editor on Mac OS X and Linux is usually set to Vim, which is not famous for being intuitive.  if you accidentally find yourself stuck in it, try typing the escape key, followed by `:q!` (colon, lower-case 'q', exclamation mark), then hitting Return to return to the shell.

**nano** is a basic editor and the default that instructors use in the workshop. It is pre-installed in the Babun Windows shell (described above) and on Mac/Linux machines.

Others editors that you can use are:

#### Windows
* Notepad++: http://notepad-plus-plus.org/
* Sublime Text: http://www.sublimetext.com/

#### Mac OS X
* Atom: https://atom.io
* Text Wrangler: http://www.barebones.com/products/textwrangler/
* Sublime Text: http://www.sublimetext.com/

#### Linux
* Gedit: https://wiki.gnome.org/Apps/Gedit
* Kate: http://kate-editor.org/
* Sublime Text: http://www.sublimetext.com/
