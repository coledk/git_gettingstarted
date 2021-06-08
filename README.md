# git_gettingstarted
# This is commands sequence how to create new repository from command line
#
#--------------------------------------------------------------------------------------------------------
# git init - this command turns any folder into a git repository.
# This command creates hidden folder called .git. That folder stores all
# of the objects and refs that Git uses and creates as a part of my project's
# history. This hidden folder is what separates a regular folder from a Git
# repository.
#
#--------------------------------------------------------------------------------------------------------
# git add README.md - this command adds new or changed files in my working
# directory to the Git staging area. Without this command no git commit would ever do anything.
# git add [filename] selects that file, and moves it to the staging area, marking it for inclusion 
# in the next commit. I can select all files, a directory, specific files, or even specific parts
# of a file for staging and commit.
# Staging area - it is a file which contains information what shouuld be included in the next commit.
# This means  if I git add a deleted file the DELETION is staged for commit.
# git add <path> - stages a specific directory or file
# git add . - stages all files (that are not listed in .gitignore) in the entire repository
# git add -p - interactively stages hunks of changed
#
#--------------------------------------------------------------------------------------------------------
# git commit -m "first commit" - this command creates a commit. The commit is like a snapshot of a
# repository. They are snapshots of entire repository at specific moment. 
# It is a good idea to run git status to find out where am I currently checked out (which branch)
#
# git commit - starts the commit process, but since it doesn't inclua a -m flag fore the messahe,
# my default text editor will be opened for me to creatr the commit message.
#
# git commit -m "my awesome comment" - starts commit processm and allows me to include the commit message
# at the same time
#
# git commit -am "my awesome comment" - in addition ti including the commit message, this option allows
# me to skip the staging phase. The addition of -a will automatically stage any files that are already
# being tracked by Git (changes to files tha i've commited before)
# 
# git commit --amend - replaces the most recent commit with a new commit.
#
# There are many of options which I can find on thi link: https://git-scm.com/docs/git-commit
#
#--------------------------------------------------------------------------------------------------------
# git branch -M main - this shows the existing branches in my local repository.
# I can also use git branch [branch-name] to create a branch from my current location,
# or git branch --all to see all branches, both the local ones on my machinem and remote trackong branches
# stores from the last git pull or git fetch from remote.
#
#--------------------------------------------------------------------------------------------------------
# git remote add origin https://github.com/coledk/git_gettingstarted.git
# 
# git remote -v - shows a list of current remotes associated with the local repository. The output of
# this comman probably can be like origin. The origin - is where repository is stored (an URL)
# git remote add [name] [URL] - adds a remote
# git remote remove [name] - removes a remote
#
#--------------------------------------------------------------------------------------------------------
# git push -u origin main - uploads all local branch commits to the corresponding remote branch.
# It updates the remote branch with local commits. As bets practice, it is important to run the git pull
# command before I push any new changes to the remote branch.
#
# git push -f - forece push that would otherwise be blockedm usually it will delete or overwrite existing
# commits.
#
# git push -u origin [branch] - it is useful when pushing a new branch, this creates an upstream tracking
# branch wit lasting relationship to my local branch.
#
# git push --all - pushes all branches
#
# git push --tags - publishes tags that are not yet in the remote repository.
#
# There are many other options I can find on following link: htpps://git-scm.com/docs/git-push
#--------------------------------------------------------------------------------------------------------
#
# To make my first commit on existing repository on GitHub:
# 1. git init - to turn current folder into repository
# 2. git add README.md - to add changed file into staging area.
# 3. git commit -m "My first commit. Added README.md with eplanation of command sequence."
# 4. git branch -M main - to show an existing branches in my local repository
# 5. git remote add origin https://github.com/coledk/git_gettingstarted.git - to add a remote
# 6. git push -u origin main - to publish my cnahges into the branch main.
#
#
