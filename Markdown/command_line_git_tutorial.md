### What is Terminal/Command Prompt?

![Terminal](assets/img/terminal.png)

Terminal (or Command Prompt on Windows) is basically a way for us to access the Command Line. This gives us access to a wonderful variety of things that we can do. We will be spending a good amount of time this weekend in here, so let's take some time to get used to it.

Once you fire up Terminal or Command Prompt (on Windows, you'll later need to run cmd.exe by right clicking on the shortcut and clicking Run as Administrator, you'll know it's running as Admin if your path ends in `../system32`), here's how you get around:

- `ls` (`DIR` on Windows) lists all the files in the current folder
- `cd` allows you to change directory. So `cd Documents` will move into the folder Documents, if there is such a folder in the current directory. You can check this by using `ls` (`DIR` on windows). To move up a directory, say back to where you were before you went into Documents, type in `cd ../`.
- `mkdir` allows you to make a folder in the current directory. So `mkdir New` makes a folder named 'New'.
- `mv` (`move` on windows) will let you move files and folders. In Terminal you can do `mv ~/Desktop/MyFile.rtf /Volumes/Backup/MyFolder` to move MyFile.rtf. On Windows `move c:\windows\temp\*.* c:\temp` will move everything from `C:\windows\temp` to `C:\temp`. `*` works as a wildcard operator here.

### What are git and GitHub?

'git' is a command line tool used for version control. What's version control? You know when you've written the first draft of an essay, and as you're saving your second draft you use "Save As" and just tack on "v2" to the name. That's the most basic kind of version control.

![Essay Drafts](images/essay_drafts.png)

Version control is extremely useful when coding. Say you made a mistake. You can easily revert back to a previous version of your work. Then, maybe you decide that change actually wasn't a mistake. Well, git is still keeping track of the code you thought you discarded, and you can go back to that. Git keeps track of everything, making working on a project much better.

[Install Git](http://git-scm.com/download)

Here are some of the basics of git. Anywhere I have brackets ([]), that means you should replace that bracketed portion with your own stuff (e.g. ["commit message"] should be replaced with something like "initial commit"):
- 'git init [project-name]' initializes a git repository called "project-name"
- 'git status' shows the status of the working directory
- 'git add [file(s)]' adds the respective file(s) to staging (a temporary place for holding until all of the staged files are committed)
- 'git commit -m ["commit message"]' commits the files in staging (i.e. the staged files are now permanently in your commit tree)


- 'git clone [project-url]' initializes that git repository locally
- 'git config global user.name ["Your Name"]' sets your name
- 'git config --global user.email ["your_email@whatever.com"]' sets your GitHub email