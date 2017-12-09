## Setup

  To participate in this workshop, you will need access to the software described below.
  In addition, you will need an up-to-date web browser.

  We maintain a list of common issues that occur during installation as a reference for instructors
  that may be useful on the

## The Bash Shell    

Bash is a commonly-used shell that gives you the power to do simple tasks more quickly.

  <div class="row">
    <div class="col-md-4">
      <h4 id="shell-windows">Windows</h4>
      <ol>
        <li>Download the Babun Windows shell (<a href="http://babun.github.io">http://babun.github.io</a>).</li>
        <li>Run the installer using the steps bellow:
          <ol>
            <li>Unzip the downloaded file and double-click the `install.bat` file to install the program.</li>
            <li>This will open a shell window and begin installation.</li>
            <li>When install is complete, you will see a message that your program has installed successfully :)</li>
          </ol>
        </li>
      </ol>
      <p><strong>Optional: Set your HOME directory in Babun to your Windows user home folder</strong></p>
      <p>The default <strong>HOME</strong> directory for Babun is set to a sub-folder in your Windows Home directory - something like: <code>C:\Users\[username]\.babun\cygwin\home\[username]</code></p>
      <p>To set your Babun HOME directory to <code>C:\Users\[username]</code>, follow these steps:</p>
        <ol>
          <li>From your Babun shell, execute <code>rundll32 sysdm.cpl,EditEnvironmentVariables</code> or search in the Start menu for `env` and select "Select Edit environment variables for your account”</li>
          <li>Select “New”
            <ol>
              <li>Name: HOME</li>
              <li>Value: C:\Users\[username]</li>
              <li>Click on “OK”</li>
            </ol>
          </li>
          <li>Click on “OK” again</li>
          <li>In Babun, run `babun install`</li>
          <li>Restart Babun. Your HOME directory should now be you Windows user directory.</li>
        </ol>
      <p>Babun will provide you with both Bash and Git already installed.</p>
    </div>
    <div class="col-md-4">
      <h4 id="shell-macosx">Mac OS X</h4>
      <p>
        The default shell in all versions of Mac OS X is Bash, so no
        need to install anything.  You access Bash from the Terminal
        (found in
        <code>/Applications/Utilities</code>).
        See the Git installation <a href="https://www.youtube.com/watch?v=9LQhwETCdwY ">video tutorial</a>
        for an example on how to open the Terminal.
        You may want to keep
        Terminal in your dock for this workshop.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="shell-linux">Linux</h4>
      <p>
        The default shell is usually Bash, but if your
        machine is set up differently you can run it by opening a
        terminal and typing <code>bash</code>.  There is no need to
        install anything.
      </p>
    </div>
  </div>
</div> <!-- End of 'shell' section. -->

<div id="git"> <!-- Start of 'Git' section. GitHub browser compatability
           is given at https://help.github.com/articles/supported-browsers/-->
  <h3>Git</h3>
  <p>
    Git is a version control system that lets you track who made changes
    to what when and has options for easily updating a shared or public
    version of your code
    on <a href="https://github.com/">github.com</a>. You will need a
    <a href="https://help.github.com/articles/supported-browsers/">supported</a>
    web browser (current versions of Chrome, Firefox or Safari,
    or Internet Explorer version 9 or above).
  </p>
  <p>
    You will need an account at <a href="https://github.com/">github.com</a>
    for parts of the Git lesson. Basic GitHub accounts are free. We encourage
    you to create a GitHub account if you don't have one already.
    Please consider what personal information you'd like to reveal. For
    example, you may want to review these
    <a href="https://help.github.com/articles/keeping-your-email-address-private/">instructions
    for keeping your email address private</a> provided at GitHub.
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="git-windows">Windows</h4>
      <p>
        Git should be installed on your computer as part of your Babun Windows shell
        install (described above).
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="git-macosx">Mac OS X</h4>
      <a href="https://www.youtube.com/watch?v=9LQhwETCdwY ">Video Tutorial</a>
      <p>
        <strong>For OS X 10.9 and higher</strong>, install Git for Mac
        by downloading and running the most recent "mavericks" installer from
        <a href="http://sourceforge.net/projects/git-osx-installer/files/">this list</a>.
        After installing Git, there will not be anything in your <code>/Applications</code> folder,
        as Git is a command line program.
        <strong>For older versions of OS X (10.5-10.8)</strong> use the
        most recent available installer labelled "snow-leopard"
        <a href="http://sourceforge.net/projects/git-osx-installer/files/">available here</a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="git-linux">Linux</h4>
      <p>
        If Git is not already available on your machine you can try to
        install it via your distro's package manager. For Debian/Ubuntu run
        <code>sudo apt-get install git</code> and for Fedora run
        <code>sudo yum install git</code>.
      </p>
    </div>
  </div>
</div> <!-- End of 'Git' section. -->

<div id="editor"> <!-- Start of 'editor' section. -->
  <h3>Text Editor</h3>

  <p>
    When you're writing code, it's nice to have a text editor that is
    optimized for writing code, with features like automatic
    color-coding of key words.  The default text editor on Mac OS X and
    Linux is usually set to Vim, which is not famous for being
    intuitive.  if you accidentally find yourself stuck in it, try
    typing the escape key, followed by <code>:q!</code> (colon, lower-case 'q',
    exclamation mark), then hitting Return to return to the shell.
  </p>

  <div class="row">
    <div class="col-md-4">
      <h4 id="editor-windows">Windows</h4>
      <p>nano is a basic editor and the default that instructors use in the workshop. It is pre-installed in the Babun Windows shell (described above).
      </p>
      <p>
        Others editors that you can use are
        <a href="http://notepad-plus-plus.org/">Notepad++</a> or
        <a href="http://www.sublimetext.com/">Sublime Text</a>.
        <strong>Be aware that you must
          add its installation directory to your system path.</strong>
        Please ask your instructor to help you do this.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="editor-macosx">Mac OS X</h4>
      <p>
        nano is a basic editor and the default that instructors use in the workshop.
        See the Git installation <a href="https://www.youtube.com/watch?v=9LQhwETCdwY ">video tutorial</a>
        for an example on how to open nano.
        It should be pre-installed.
      </p>
      <p>
        Others editors that you can use are
        <a href="http://www.barebones.com/products/textwrangler/">Text Wrangler</a> or
        <a href="http://www.sublimetext.com/">Sublime Text</a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="editor-linux">Linux</h4>
      <p>
        nano is a basic editor and the default that instructors use in the workshop.
        It should be pre-installed.
      </p>
      <p>
        Others editors that you can use are
        <a href="https://wiki.gnome.org/Apps/Gedit">Gedit</a>,
        <a href="http://kate-editor.org/">Kate</a> or
        <a href="http://www.sublimetext.com/">Sublime Text</a>.
      </p>
    </div>
  </div>
</div>
