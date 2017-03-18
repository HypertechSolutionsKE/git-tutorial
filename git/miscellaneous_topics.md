# Miscellaneous Topics

### Checking Status and History
If you want to check with files have been changed since the last commit, or if you want to see new files or files staged for commit, you can use

`$ git status`
to check the status of your repository.

To check the line-by-line changes you've made since your last commit, use the following command:

`$ git diff`
To check the commit history use

`$ git log`
Undoing Changes

### Undoing a Commit/Multiple Commits
To create a commit that undos the changes of the latest commit you can revert a commit.

`$ git revert HEAD`
You can specify how many commits to reverting by including the hash or some sort of identification of the commit to which you want to revert. For example, the following command makes a commit that undos the changes of the previous two commits:

`$ git revert HEAD^`
Undoing all Changes since the Latest Commit
To reset your repository to its state when you made your latest commit, you can do the following:

`$ git reset --hard HEAD`
Undoing the Changes to a Single File since the Latest Commit
If you want to reset only a single file to its state since the last commit without touching other modified files, you can specify the specific as an argument. The following example resets grades.c to its state since the last commit.

`$ git reset grades.c`
Unstaging a File
If you accidentally git added a file that you do not want to be staged for commit, you can easily unstage it. Note that this does not change the contents of the file. All it does it exclude it from being included in your next commit. This command is essentially the opposite of git add. In the next example, grades.c is unstaged, so when you commit, any changes made to that file will not be recorded.

`$ reset grades.c`

### Github and Remote Respositories
You may have heard of GitHub before and are wondering about its relation to Git. GitHub is an online hosting service for Git repositories. GitHub keeps the code it hosts open for the public to see, which is why this tutorial did not cover GitHub and remote repositories. However, if you are interested in working on your own projects outside of class, GitHub is a great resource use with your project.
