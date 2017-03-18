#Working with Git

1. Staging and Committing Changes

In a Git repository, changes to your code are marked by *commits*, snapshots of the changes to your code since your previous commit. You need to manually specify which files will have their changes marked in the next commit. This is known as *staging* your files. Continuing off the Project 1 example, all of the test files are not tracked yet. If we wanted to stage all of them we could do the following command

`$ git add -A`

to stage all of the relevant files. To commit the changes, we do

`$ git commit`

and type in a message to go along with the commit, documenting the changes made for the current commit. You can also stage files one by one by adding the file as an argument when staging. Committing has an option to quickly write a commit message when making the commit.

`$ nano grades.c`

`...`

`$ git add grades.c`

`$ git commit -m "created grades.c file"`

In a normal Git workflow, you want to stage any files that you have made changes to (git add) and then commit the changes when you reach a small milestone (git commit). Remember to commit early and often. Commits are inexpensive to make and are an excellent example of incremental code development. If you make commits that track small, isolated changes, fixing bugs can be easier since you have a good reference to locate possible bug locations.

2. Branching and Merging

Git has a feature called *branching* where you can have a version of your code diverge from your main code in order to try out new features or experiment with your project without the risk of breaking functionality in the main code. If you like the changes made to the divergent branch, you can always merge the two branches back together. In order to support good incremental code development, you should create a new branch for every new feature, and code on the respective branch. Once you have verified that the branch has working code, you merge it back to the master branch. That way, your main code branch will always have clean, working code.

If we wanted to create a feature in the grades calculator that calculates the mean and standard deviation, we might want to create a branch called "statistics." To create that branch we want the command

`$ git branch statistics`

to generate the branch with the name "statistics." To move into that branch, we use the command

`$ git checkout statistics`

and continue coding normally. One we are done implementing and verifying the feature, we move back to our master branch and merge the branches.

`$ git checkout master`

`$ git merge statistics`

After the merge, any changes you made in the statistics branch will be present in your master branch.

