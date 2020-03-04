# Git Bash First Repository

This repository will show users how to create a repository using Git Bash. In addition, This repository will keep track of useful commands used throughout the repository. Keep in mind, Git Bash uses Unix commands. 

## Getting Started

**Prerequisites -**

**Software**
- [Git Download for Windows](https://gitforwindows.org/)
- [Git Alternative Downloads for Mac /Linux /Unix](https://git-scm.com/downloads)

For Windows, A setup wizard should install git bash within your system. During the installation, all options should be kept as default. Any additional options will fall outside of the scope of this repository. The installation wizard should look like the image below.

<img src = "Git Pictures/Git Installing window.JPG" Width="600" height="420">

Once installed, launch Git Bash. 

<img src = "Git Pictures/Git Bash Command Line.JPG" Width="650" height="320">
 
## Setting Username and Email

While using Git Bash with multiple contributors, it is important to set a local Username and Email. This task can be accomplished by using the command line in Git Bash. 

**To configure your username, type and alter the following command then press enter:**
```
 git config -- global user.name "Your Full Name"
```
**To configure your Email, type and alter the following command then press enter:**

```
 git config -- global user.email "Your Email"
 ```
 
 An example using the Username "Bob Chavis" and email "BobChavis@gmail" has been provided below. Use this refrence to input your Username and Email.
 
<img src="Git Pictures/Username and Email.JPG" Width="650" height="320">

**To ensure that a Username and Email has been set, type:**

```
git config -- list
```

<img src="Git Pictures/config Settings.JPG" Width="650" height="320">

A list of many variables will be listed. Among the few, the user.name and user.email should display your newly entered data. You can always change Username or Email using the commands listed previously. 

**To quickly search specific config data, type:**

```
git config user.email
```

<img src="Git Pictures/config shortcuts.JPG" Width="650" height="320">

This command will only display the variable you listed. You can also alter "user.email" with any other variable found within the config list to display said variable. below are some examples.

```
git config user.email
git config core.fscache
git config core.symlinks
```

Each one of these commands will display their respective stored variable. More commands can be found near the bottom of the repository with the title named "Command List".

## Initiating Repositories

When creating a repositroy using git, It is important to choose or create a folder to control. 

<img src="Git Pictures/First Repository Folder.JPG" Width="650" height="320">

using simple change directory commands, we navigate into the "First Repository" folder. Once selected, we initiate a git repository using the following line.

```
git init
```

we can see that git successfully initiated the git repository if you now see master next to the folder name. Congratulations you have successfully created a repository!


## Command List

### Git Information Commands

|                commands  $                   |                   Explanation                              |
|----------------------------------------------|------------------------------------------------------------|
|git help                                      |    Shows the entire help index                             |
|git -- version                                |    Displays what Git Bash Version you have installed       |
|whoami                                        |    Displays what user you are logged into                  |
|git config user.name                          |    Shows what username is currently set                    |
|git config user.name                          |    Shows what username is currently set                    |

### Git Commit Commands
|                commands  $                   |                   Explanation                              |
|----------------------------------------------|------------------------------------------------------------|
|git init                                      |    Initiates a git repository in selected folder           |
|git add .                                     |    Sets a version point to commit onto the master branch   |
|git commit -m "you message here"              |    Commits files to the new branch and adds a message      |
|git log                                       |    Shows all of the commits submitted by author and date   | 

### Navigation

|                commands  $                   |                   Explanation                              |
|----------------------------------------------|------------------------------------------------------------|
|pwd                                           |    Shows what directory you are currently in               |
|ls                                            |    Shows all folders within current directory              |
|cd ~                                          |    Changes directory to set home directory.                |
|cd "desired directory"                        |    changes directory to desired directory                  |
|cd ..                                         |    Changes directory back one                              |

