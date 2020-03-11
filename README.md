# Git Bash First Repository

Git Bash is a tool used by developers and teams to establish version control. This repository will show users how to create a repository using Git Bash. In addition, This repository will keep track of useful commands used throughout the repository. Keep in mind, Git Bash uses Unix commands. 

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
 
 An example using the Username "Bob Chavis" and email "BobChavis@gmail" has been provided below. Use this reference to input your Username and Email.
 
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

**Example:**
```
git config user.email
git config core.fscache
git config core.symlinks
```

Each one of these commands will display their respective stored variable. More commands can be found near the bottom of the repository with the title named "Command List".

## Initiating Repositories

When creating a repository using git, It is important to choose or create a folder to control. 

<img src="Git Pictures/First Repository Folder.JPG" Width="650" height="420">

using simple change directory commands, we navigate into the "First Repository" folder. Once selected, we initiate a git repository using the following line.
**note:** we use a backslash because there is a space in "First Repository"

**To Initiate a new Repository, type:**

```
git init
```

To verify, we can use our file explor to see turn on and see hidden files have been added to create a repository. we can see that git successfully initiated the git repository if you also now see master next to the folder name. Congratulations you have successfully created a repository!

## Committing

Committing is a way to update files into the repository keeping track of all files. When a file is edited, it is not updated immediately in the repository. We must prepare the file first, then commit and update it on the repository. 

Since we started our first repository, we have not added any files inside. For our next step we will add a simple picture and text document with some unique usernames. Feel free to add anything you wish!

<img src="Git Pictures/First Text Doccument.JPG">

Now that we added files into our folder, our repository is officially outdated. To update our repository, we will need to prepare all file that were either added or edited. 

<img src ="Git Pictures/Git first commit.JPG" Width="650" height="320">

To prepare files we have to first prepare what files we are about to update. In this situation we will update all files. 

**Add files to commit:**
```
git add .
```

This will add all files found within the folder and prepare to commit them. 

**Committing files to update the repository**
```
git commit -m "Any message to explain what you are doing or updating."
```

This will actually update the repository of all files. The Note is extremly important because it will not what changes have been made since the last version. We can see all commits through the log.

<img src="Git Pictures/Git log.JPG" Width="650" height="320">

**Log Information:**
```
git log
```
In the log, We can see all of the times we have committed and by who. In addition, it is possible to search the log using authors names.

## Committing a Single File

To commit a single file it does not differ much. For This example, we will create a new password text file and add some new names to our previous name text file. 

<img src="Git Pictures/git single commit.JPG">

**Git Status:**
```
git status
```

The git status shows us that the repository has indicated that two files are either new or edited and need to be committed. From here, we must prepare the files and commit them to update the repository. However, in this situation we will commit only one file.

<img src ="Git Pictures/stage area.JPG" Width="650" height="320">

We are going to add the "Names List" text file to prepare to commit. 

**Adding a Single file to commit:**
```
git add Names\ List.txt
```

You can add any file by just listing it after add. Now when we check the status, "Names List.txt" will be green indicating that it is a modified file ready to commit while preventing anything in red from following. 

Once we commit the file and check status once more, the repository will see that "Names List.txt" is up to date and the same that it will not list it. Only "Passwords.txt" should remain.

<img src="Git Pictures/git commit updating text file.JPG" Width="650" height="320">

Now we will add the remaining files with previous techniques.

<img src="Git Pictures/updating passwords.JPG" Width="650" height="320">

Once all files are committed and the repository is updated, we can use git status one last time. The status will indicate that no files are different than the repository, meaning eveything is up to date. You can check log to see all of the commits as reference  or to go back in case something bad happens. This is called version control and an essential for developers.

## Git Flowchart


<img src="Git Pictures/GitHub_Flow_steps.png"> 

## Command List

### Git Information Commands-

|                commands  $                   |                   Explanation                              |
|----------------------------------------------|------------------------------------------------------------|
|git help                                      |    Shows the entire help index                             |
|git -- version                                |    Displays what Git Bash Version you have installed       |
|whoami                                        |    Displays what user you are logged into                  |
|git config user.name                          |    Shows what username is currently set                    |
|git config user.name                          |    Shows what username is currently set                    |

### Git Commit Commands-
|                commands  $                   |                   Explanation                              |
|----------------------------------------------|------------------------------------------------------------|
|git init                                      |    Initiates a git repository in selected folder           |
|git add .                                     |    Prepares Files to commit                                |
|git add Example.txt                           |    Prepares a specific file to commit.                     |
|git status                                    |    Shows what files are ready to commit                    |
|git commit -m "your message here"             |    Commits files to the new branch and adds a message      |
|git commit -am "your message here"            |    Directly Adds and Commits all files with one command    | 
|git diff                                      |    Shows difference between repository and work files      |
|git diff --staged                             |    Shows difference between stage and work files           |
|git log                                       |    Shows all of the commits submitted by author and date   | 
|git log --author="author's name"              |    Shows all the commits submitted by a certain author     | 
|git checkout Example.txt                      |    Sets the named file on the work space to the last version found in the repository|

### Git Editing Files-
|                commands  $                   |                   Explanation                              |
|----------------------------------------------|------------------------------------------------------------|
|mkdir "Example_Folder"                        |    Creates a new directory or folder                       |
|rmdir Example_Folder                          |    Deletes an exsisting directory or folder                |
|git rm Exmaple.txt                            |    Deletes file from the work space                        |
|git mv Example.txt New_Name.txt               |    Renames file name into a new name                       |


### Navigation-

|                commands  $                   |                   Explanation                              |
|----------------------------------------------|------------------------------------------------------------|
|pwd                                           |    Shows what directory you are currently in               |
|ls                                            |    Shows all folders within current directory              |
|cd ~                                          |    Changes directory to set home directory.                |
|cd "desired directory"                        |    changes directory to desired directory                  |
|cd ..                                         |    Changes directory back one                              |

