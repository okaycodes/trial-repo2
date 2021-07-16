# Upload from local computer

This is an attempt at uploading files from my local computer to the github
server via my terminal in the text editor

### Process

- create required directory, navigate into it in terminal
- create files
- write your code,
- use the git add command to convert it to a repository
- use git commit -m to commit changes to git still within the local computer
- for modified files it is possible to both add and commit at the same time using
the git commit -am command
- use git push command to push said changes to github

### branching
- check for all available branches using the git branch command
- create a new branch using the git checkout -b <branch name> command
- switch branch using the git checkout <branch name> command
- use the git diff <branch name> command to check the differences between a branch
and the branch that is currently active. If the get diff is used on the same branch
it will show changes such as those committed and those that haven't been.
- type q to exit the difference prompt
- merge a branch to the main using the git merge command.
- normally merging is not done from local computer especially as git is used in
collaboration work with others, on github you ought to make a pull request and
have the code reviewed before it is merged. However, while working on a branch of
master with others, you will likely want to or need to merge master to your branch
so that your branch can be up to date with all the extant changes on master.
- merge conflict can arise when main is being merged by multiple people working on
different branches such that git cannot decide which codes to keep and which to delete
- merging master to a branch is a common source for merging conflict as you might be
changing a code in your branch that has previously been changed by another person working
in the team since you last merged with master.
- delete a branch using the git branch -d <branch name> command
- import changes made from github to the local machine using the git pull command
