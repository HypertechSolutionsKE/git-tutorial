### Getting Started

1. Downloading Git
Grace already has Git installed. If you want Git on your local machine, you can always Google how to do so. ☺

2. Configuring Git
The first thing you'll want to do is to configure your name and email on Git. Git needs your identity to document the contributor whenever there is a change to the code. The two commands are as follows:

`$ git config --global user.name "hypertech"`
`$ git config --global user.email "hypertechsolutions.co.ke"`

3. Creating or Cloning a Git Repository
To turn a project into a Git repository, go inside the project folder and type the command

`$ git init`
to create a new Git repository. A folder to track history will be created, although there will be no other changes to your repository. If you want to clone an existing Git repository and you know the location of the respository, you can easily make a copy of the repository into your current directory:

`$ git clone @hypertechsolutions.co.ke:~/216/project1`
So if we wanted to do Project 1 under version control, we would want to simply convert it into a Git repository after copying over the files.

`$ cp -r ~/216public/projects/project1 ~/216`
`$ cd ~/216/project1`
`$ git init`
