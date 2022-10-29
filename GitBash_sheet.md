title	description	created	updated
GitBash-Cheatsheet
Git Bash all necessary commands for using Github
2022-10-08
2022-10-08
GITHUB COMMANDS SHEET
Contents
SETUP
SETUP & INIT
STAGE & SNAPSHOT
BRANCH & MERGE
INSPECT & COMPARE
TRACKING PATH CHANGES
SHARE & UPDATE
RERWITE HISTORY
TEMPORARY COMMITS
Undo Changes
SETUP
set a name that is identifable for credit when review version history

  git config --global user.name "[firstname lastname]"
set an email address that will be associated with each hustory maker

  git config --global user.email "[valid-email]"
set automatic command line coloring for Git for easy reviewing

  git config --global color.ui auto
Get global config

  git config --global --list
SETUP & INIT
initialize an existing directory as a Git repository

  git clone https://link-to-project
retrieve an entire repository from a hosted location via URL

  git clone [url
STAGE & SNAPSHOT
show modified files in working directory , staged for your next commit

  git status
Clone private repository

  git clone ssh://git@github.com/[username]/[repository-name].git
Add all new and changed files to the staging area

  git add -A
Remove a file (or folder)

  git rm -r[file-name.txt]
show modified files in working directory , staged for your next commit

  git status
add a file as it looks now to your next commit (stage)

  git add [file] 
unstage a file while retaining the changes in the working directory

  git reset [file] 
commit your staged content as a new commit snapshot

  git commit -m "[descriptive message]" 
BRANCH & MERGE
list your branches. a * will appear next to the currently active branch

  git branch 
Push a branch to your remote repository

  git push origin [branch name]
Push changes to remote repository (and remember the branch)

  git push -u origin [branch name]
Delete a remote branch

  git push origin --delete [branch name]
Update local repository to the newest commit

  git pull
Pull changes from remote repository

  git pull origin [branch name]
Add a remote repository

  git remote add origin ssh://git@github.com/[username]/[repository-name].git 
Set a repository's origin branch to SSH

  git remote set-url origin ssh://git@github.com/[username]/[repository-name].git
Update local repository to the newest commit

  git pull
switch to another branch and check it out into your current working directory

  git checkout 
merge the specified branch's history into the current one

  git merge [branch] 
show all commits in the current branch history

  git log 
View changes (detailed)

  git log --summary
Switch to a branch

  git checkout [branch name
Switch to the branch last checked out

  git checkout
Discard changes to a file

  git checkout -- [file-name.txt]
List all branches (local and remote)

  git branch -a
Delete a branch

  git branch -d [branch name]
Delete a branch forcefully

  git branch -D [branch name] 
INSPECT & COMPARE
show the commits on branchA that is not in branchB

  git log branchB..branchA
show any object in Git in human-readable format

  git show [SHA]
difference between working directory and last commit

  git diff HEAD
difference between staged changes and last commit

  git diff --cached
diff of what is changed but not staged

  git diff 
diff of what is staged but not committed

  git diff --staged
TRACKING PATH CHANGES
delete the file from project and stage the removal for commit

  git rm[file] 
change an existing file path and stage the move

  git mv [existing-path] [new-path]
Show all commit logs with indication of any paths that moved

  git log --stat -M
SHARE & UPDATE
add a URL as an alias

  |git remote add [alias] [url] 
fetch down all the branches from that Git remote

  git fetch [alias]
merge a remote branch into your current branch to bring it up to date

  git merge [alias]/[branch] 
RERWITE HISTORY
apply any commmits of currents branch ahead of specified one

  git rebase [branch]
clear staging area, rewrite working tree from specified commit

  git reset --hard [commit]
TEMPORARY COMMITS
save modified and staged changes

  git stash
list stack-order of stashed file changes

  git stash list
write working from top of stash stack

  git stash drop
discard the changes from top of stash stack

  git reset --hard [commit]
Remove all stashed entries

  git stash clear
discard the changes from top of stash stack

  git reset --hard [commit]
Undo Changes
Get the previous version of a given files

  git checkout <commit> <paths> // HEAD is used implicitly if <commit> omitted
Revert certain commit by applying another one (to persist history)

  git revert <commit>
Unstage files

  git reset <paths>
Unstage all files

  git reset
Move state to specified commit

  git reset <commit>
// --hard (to remove changes) --soft (to leave changes staged)
Set specified files to state of certain revision

  git checkout <commit> <paths>
