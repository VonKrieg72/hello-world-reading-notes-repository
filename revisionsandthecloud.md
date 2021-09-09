# Revisions-and-the-Cloud

## Version Control

**Version Control** is a system that enables you to revisit various versions of a file, or set of files by making a record of changes. Through Version Control, you can change a file back to a previous version of itself, track modifications and modifying individuals and compare changes. 

**Local Version Control System** (Local VCS) was created many years ago by programmers, and it has one database on your hard disk, that stores changes to files.

**Centralized Version Control System** (CVCS) was created due to multiple people on development teams needing to collaborate on a single file or set of files. 

However, CVS had many drawbacks. For example, If a CVS were to go down, collaborators wouldn't be able to work with each other on a file, or save changes and new versions. Also, if the central database's hard disk were to be corrupted without any backups, all work would be lost, with the exception of portions on a local machine. 

In response to these short comings, **Distributed Version Control Systems** (DVCS) was created. In DVCS, programmers working together on a team were able to prevent the loss of data, by enabling them to create mirrored repositories, which served as data backups, that could be easily placed on the server to replae any lost information. 

## So What is Git

Git is a DVCS that stores data in a file system made up of snapshots. Snapshots of files are created by Git, and the references are stored. Whenever you make changes to a project and change it, it's called a commit. Because a project's hstory resides on a local disk, Git relies on local operations, which enables it to process things with expedience. Git tracks every single change made to a file, and always detects file corruption or loss of information in transit, because of this, permanent damage to files is greatly minimized. Git has three main states:

-Committed- Data is securely stored in a local databse. 

-Modified- File has been changed, but not committed to the database.

-Staged- Flagged a file's changed version to be committed in the next snapshot. 

## Getting Started

There are three ways to install Git on your computer:

-Install it as a package

-Install it via another installer

-Download and compile the source code

On Windows, Mac, Linux Os you can download from the Git Website 

[(http://git-scm.com/download/windows)]   /mac  /linux

You can download from Github on Mac and Windows 

[(http://mac.github.com)]. [(http://windows.github.com)]

## Initial Customizations

After installing Git, it's recommended to perform customization steps, which should only need to be completed once. There's a tool called "Git Config" which allows the setting of configuration variables that control Git's operation and look. You're going to have to set up your user name and email in order to use Git Commit. In order to do so, type the following into your terminal or command line:

git config --global user.name "your name here"

git config --global user.email "example@email.com"

To confirm that the setting are correct, enter the following commands:

git config --global user.name (should return your name)

git config --global user.email (should return example@email.com)

Git will use the system's default text editor, unless you choose to configure a different text editor. For example, if you choose to use emacs as a text editor you have to install it. Enter the following command into the terminal command line:

git config --global core.editor emacs

In the event that you need help, there's three commands you can enter:

-git help command

-git command --help

-man git-command

## Setting up a Git Repository

In order to import an existing project or directory into Git type these commands:

cd test (cd = change directory)

git init

At this point a new subdirectory named **.git** has been created that has the repository files. In order to track these repository files, you have to type an initial commit.

git add *.c

git add LICENSE

git commit -m “any message here”

After typing in these commands, your files will be tracked, and there is an initial commit

## Cloning

If you wish to create a copy of an existing Git repository from a particular server, you can do so with the clone command.

git clone https://github.com/test

By cloning, you have copied all versions of all files for a project. This leads to the creation of a directory called **Test.** If your wish to clone a repository into another directory, with another name, you can do so by entering:

git clone https://github.com/test mydirectory

## Workflow

The local Git repository has three componenets:

-Working directory: The actual files reside here

-Index: The area used for staging

-Head: Points to the most recent commit

If you wish to check a file status, enter:

git status

If you wish to track and stage a new file, you can do so by entering:

git add filename *(for single files)*

git add * *(for all files)*

After these two command files are tracked and staged for commiting.

After staging one or more multiple files, you should commit the changes, and record what you did within the commit message.

git commit -m “made change x,y,z”

After this step, you have committed changes for the file or files

If you wish to push changes to a remote repository, you would enter:

git push origin master

This command pushes changes from the local master branch, to the remote repository named origin. 

## Stashing Changes

In the event that you're not ready to commit changes, but don't want to lose them either, you can hide them by enterig the command:

git stash 

This command will temporarily remove changes and hide them. When you're ready later on to commit the changes or continue working on them enter:

git stash apply

This command will retreive the hidden changes

## Remote Repositories

Remote repositories are important, because in order to collaborate on Git, you must interact with them. Remote repositories are versions of a project residing online or on a network. You're able to work on multiple repositories. On some of them, you may have read/write privileges and some you'll have read only privileges. Remote repositories will be used by your team to push information and pull data from. 

## Cloned Repositories

In the event that you decide to clone a repository, Git will automatically give the name *origin* to the server from which you cloned it from, and it will give the name *master* to your local branch.

## Seeing Your Remotes

When you run the ***git remote*** command, you are able to view the short names such as ***origin*** of all specified remote handles. By entering the command ***git remote -v*** you are able to review all the remote URLs, next to their corresponding short names. Here are a couple of examples:

cd example

git remote -v

remote1 https://github.com/remote1/example (fetch)

remote1 https://github.com/remote1/example (push)

remote2 https://github.com/remote2/example (fetch)

remote2 https://github.com/remote2/example (push)

remote3 https://github.com/remote3/example (fetch)

remote3 https://github.com/remote3/example (push)




[<== Back](README.md) 
