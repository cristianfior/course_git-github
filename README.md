## README please!
*This is a cheatsheet I've made to learn and remember git commands*
- git init: initialize the git repository on the specified archive
- git clone *LinkToRemoteRepositorySSH*: creates a clone of an existing repository
- git config --local help.autocorrect 1: authorize git to correct commands when it's misswrited
- git config --local user.name "username": define collaborator username
- git config --local user.email "useremail": define collaborator useremail
- git config --local core.editor "editor": define the default editor to the files of the project
- git config --local alias.aliasname gitcommand: create an alias for a git command
- git status: see the status of the project and its files
- git add *filename or param*: stage the files (it's possible to add a specific filename or add all by using the param: *.* or *--all* or *-A*)
- git mv *path/oldfilename* *path/newfilename*: renames a file
- git mv *oldpath/filename* *newpath/filename*: moves a file to another folder
- git rm *filename*: remove a file from the project
- git checkout *filename*: reset a modified file if not staged
- git commit -m "message": creates a local snapshot of the staged files
- git commit -am "message": stage and creates a snapshot, if you already made the first commit of the file
- git remote add origin *LinkToRemoteRepository*: link the local repository to the remote one
- git push -u origin main: in the very first push, is necessary to track to where changes goes and from where it comes
- git push origin *branchname*: pushes the commits to remote repository
- git pull: pull changes from the remote repository
- :question:git log *param*: see a timeline of the commits. **Params**: *--decorate*, give back info about the branch | *--author="name"*, filter the log by author | *--oneline*, show only a part of commit hash and its name | *--all*, show the log including all existing branches | *--graph*, show a graph with a tree of merges and rebases | *--pretty=oneline*, show the complete commit hash and its name | *--since='month day year'*, return commits after the date excluding the set day | *--until='month day year'*, return commits before the date excluding the set day
- :question:git shortlog *param*: a simplified log that return the authors, its commits quantity and names. **Params**: *-sn*, simplify even more and return only the commits quantity and author username
- git reflog: return a log with commits references
- git branch: list all existing local branches
- git branch branchname: creates a new branch
- :question:git checkout *param* branchname: change between branches. **Params**: *-b* creates and checkout automatically to a new branch | *-* switches back to the previous branch | *-d* deletes the branch
- git branch --set-upstream-to=origin/main branch: set the branch to pull the changes from main
- git merge branchname: the current branch will inherit all features from the branch passed in the command
- :question:git stash *param*: save and hide the features uncommited of a branch. **Params**: *save "stashname"*, creates a named stash | *apply stash@{index}*, apply the features saved before in the current branch | *list*, return a list with all existing stashes | *clear*, cleans features saved in the stash | *drop stash@{index}*, deletes a stash | *pop*, removes the first stash in the list and applys in the current branch | *branch branchname*, creates a new branch and applys the features of first stash in the list
---
