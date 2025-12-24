working directory , stage area , local directory

git init = makes a repository

git status = shows the situation of our file

git add <file> = adds our file to stage area (directory -> stage)
we can use . for all the files

git commit -m "" = adds our files to local with a comment that we'll say (stage -> local)

git commit -a -m "" = adds our files to stage area (directory -> stage) then add our files to local with a comment that we'll say (stage -> local)
"we can not use this command before add our file , so our file must add then we can use this command ."

git rm --cached <file> = unsatges our files (stage -> directory)

git diff = shows changes in files

git diff --help = shows all commands

git push <repository> = sends (push) your local commits to a remote repository (local -> remote)

git pull <repository> = updates your local branch with the latest changes from a remote repository (remote -> local)

git clone <HTTPS,SSH> = creates a local copy of an existing Git repository
"after we make a remote repository in githup we must clone it ."

git remote = lists our remote repository

touch .gitignore = creates gitignore file

git config --global user.name "your name" = save user name as global setting

git config --global user.email "your email" = save user email as global setting

----> Commit syntax
git log = shows commits (detail of commit like num of commit, author, date of commit)

git log --help = shows some infos of commits related to log command

git log --oneline = shows each commits in a line

git log -2 --oneline = shows last two commits in a line

git log -p = shows commits with all their changes

git checkout -- <file> = unmodified file (changes modified file to last form of itself)

git reset HEAD . = removes files form stage area (stage -> directory)

git reset <commit> = returns our activity before that commit but keep the folder and file even empty (soft)

git reset --hard <commit> = returns our activity and delete created files and folders before that commit

git log --graph : list our commits like a tree and show detail of commits dedicated to branches and merges


---->Branch and Merge syntax
git branch <branch-name> = creates a new branch

git branch -a = lists our both local and remote branches

git branch -r = lists our remote branches

git branch -l = lists our local branches

git branch -d <branch-name> = deletes a branch

git switch <brance-name> = switches between branches
git checkout <brance-name> = switches between branches

git switch -c <branch-name> = creates a branch and switch to created branch
git checkout -b <branch-name> = creates a branch and switch to created branch
"before switch between branches we must check status and we will add and commit if needed ."

git merge <branch-name> = merges(add) changes of another branch to branch we're in it


---->Stash
git stash = adds our changes in temporary location(stash) with random id and commit

git stash save "commit" = adds our changes in temporary location with our commit
git stash push -m "commit" = adds our changes in temporary location with our commit

git stash list = lists our stashes

git stash drop <stash@{stash-number}> = deletes changes from the specified stash

git stash show <stash@{stash-number}> = shows changes in stash in summary form

git stash show -p <stash@{stash-number}> = shows changes in stash accurately

git stash pop <stash@{stash-number}> = applies changes in specified branch and delete that stash

git stash apply <stash@{stash-number}> = applies changes in specified branch and keep that stash



'fork' is a personal copy of someone else's repository under your github account
'pull request' is a request to merge changes from one branch/repository to another 
