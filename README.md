# Upload from local computer

This is an attempt at uploading files from my local computer to the github server via my terminal in the text editor

### Process

- create required directory, navigate into it in terminal
- create files
- write your code,
- use the git add command to convert it to a repository
- use git commit -m to commit changes to git still within the local computer
- for modified files it is possible to both add and commit at the same time using the git commit -am command
- use git push command to push said changes to github

### branching
- check for all available branches using the git branch command
- create a new branch using the git checkout -b <branch name> command
- switch branch using the git checkout <branch name> command
- rename a branch using the git branch -m <newBranchName> command
- to save a new branch on github from terminal use git push -u origin <branchName> command
- use the git diff <branch name> command to check the differences between a branch and the branch that is currently active. If the get diff is used on the same branch it will show changes such as those committed and those that haven't been.
- type q to exit the difference prompt

### merging
- merge a branch to the main using the git merge command.
- normally merging is not done from local computer especially as git is used in collaboration work with others, on github you ought to make a pull request and have the code reviewed before it is merged. However, while working on a branch of master with others, you will likely want to or need to merge master to your branch so that your branch can be up to date with all the extant changes on master.
- merge conflict can arise when main is being merged by multiple people working on different branches such that git cannot decide which codes to keep and which to delete
- merging master to a branch is a common source for merging conflict as you might be changing a code in your branch that has previously been changed by another person working in the team since you last merged with master.
- delete a branch using the git branch -d <branch name> command
- import changes made from github to the local machine using the git pull command


### Undo
- undo a change that has been made but not yet committed with the git reset command. when this is done it is known as unstaging
- undo a commit using the HEAD~1 command. the ~1 tells the system to revert the last commit made
- undoing multiple commits isn't straightforward but one can see a log of all commits made using the git log command. It displays the commit as well as the commit messages which can help to identify what was done and when and also aid the reversal of commits, it also displays a commit id with which you can reset the commit using the git reset <commitId> command.
- it is important to note that uncommitting does not undo changes i.e delete the changes but rather as the name implies uncommit those changes. To actually remove those changes you use git reset --hard <commitId> command

### Forking
- this allows us to create a branch off other peoples repositories that we likely do not have access to copying it to our local computer for local consumption. E.g. copying somebody else's project so we can have a better look at it and make our own tweaks and changes.
- forking is normally done on the github platform and not on the local terminal
