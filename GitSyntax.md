working directory , stage area , local directory

git init = make a repository

git status = show the situation of our file

git add <file> = add our file to stage area (directory -> stage)
we can use . for all the files

git commit -m "" = add our files to local with a comment that we'll say (stage -> local)

git commit -a -m "" = add our files to stage area (directory -> stage) then add our files to local with a comment that we'll say (stage -> local)
"we can not use this command before add our file , so our file must add then we can use this command ."

git rm --cached <file> = unsatge our files (stage -> directory)

git diff = show changes in files

git diff --help = show all commands


----> Commit syntax
git log = show commits (detail of commit like num of commit, author, date of commit)

git log --help = show some infos of commits related to log command

git log --oneline = show each commits in a line

git log -2 --oneline = show last two commits in a line

git log -p = show commits with all their changes

git checkout -- <file> = unmodified file (change modified file to last form of itself)

git reset HEAD . = remove files form stage area (stage -> directory)

git reset <commit> = return our activity before that commit but keep the folder and file even empty (soft)

git reset --hard <commit> = return our activity and delete created files and folders before that commit

git log --graph : list our commits like a tree and show detail of commits dedicated to branches and merges


---->Branch and Merge syntax
git branch <branch-name> = create a new branch

git branch -a = list our branches

git branch -d <branch-name> = delete a branch

git switch <brance-name> = switch between branches
git checkout <brance-name> = switch between branches

git switch -c <branch-name> = create a branch and switch to created branch
git checkout -b <branch-name> = create a branch and switch to created branch
"before switch between branches we must check status and we will add and commit if needed ."

git merge <branch-name> = merge(add) changes of another branch to branch we're in it
