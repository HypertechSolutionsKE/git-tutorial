#A Brief Introduction to Git

##(by Andrew Liu, liu.andrew.x [AT] gmail [DOT] com)

###What is Git?

Git is an open-source version control system. It was designed and developed by Linus Torvalds (creator of the Linux kernel) and is the most popular version control system to date.

###Why use Git?

There are several reasons to use Git (or version control in general). We will just list a few reasons:

Git helps out a lot with respect to incremental code development and documentation.
..1. Git is relatively easy to pick up and learn.
..2. Git is very efficient and will not adversely affect your code.
..3. If you make a mistake with your code, Git can easily revert you back to a working version of your code.
..4. You can easily maintain multiple backups of your code that can update themselves without you needing to copy/paste your code over.
..5. You can review the history of your code.
..6. You can make multiple versions of your code.
..7. You can work on experimental changes or features without breaking your working code.
..8. You can keep track of contributions to the code when working as part of a team.
..9. Companies use version control, so you will need to learn version control eventually.

###Getting Started

####Downloading Git
Grace already has Git installed. If you want Git on your local machine, you can always Google how to do so. ☺

####Configuring Git
The first thing you'll want to do is to configure your name and email on Git. Git needs your identity to document the contributor whenever there is a change to the code. The two commands are as follows:

..1. $ git config --global user.name "Billy Programmer"
..2. $ git config --global user.email "bprogrammer123@terpmail.umd.edu"

####Creating or Cloning a Git Repository
To turn a project into a Git repository, go inside the project folder and type the command

$ git init
to create a new Git repository. A folder to track history will be created, although there will be no other changes to your repository. If you want to clone an existing Git repository and you know the location of the respository, you can easily make a copy of the repository into your current directory:

$ git clone bprogrammer@linux.grace.umd.edu:~/216/project1
So if we wanted to do Project 1 under version control, we would want to simply convert it into a Git repository after copying over the files.

$ cp -r ~/216public/projects/project1 ~/216
$ cd ~/216/project1
$ git init
