# Learn with Me (Vardan Tyagi)

##

some demo git code

cd folderName (to go to a folder)

pwd (to check the file path)

git --version

git status

git config --global user.email "vardantyagii@gmail.com"

git config --global user.name "vardantyagi"

config --list

ls -la (to check inside folders info)

ls (to check inside folders name)

git status

git init

git add . (to add all the files)
            or
git add fileName1 fileName2

git commit -m "message to be send"

git log

git log --oneline (give short answer)

.........................................................................

create .gitignore file

put (.env) file to .gitignore file

git add .gitignore

git commit -m 'commiting .gitignore file"

put .gitkeep file inside the folders which are empty and you do not need to track it

.........................................................................

(git behind the scenes)

git show -s --pretty=raw commitId

git ls-tree 597471debcd350b6ddfb876c95b570b720141d9c

// git internals

.........................................................................

// git branches

// "master" is a head pointer which points on the current file

git branch -> list all the branches

git branch bug-fix -> create new branch (bug-fix) name in this case

git switch bug-fix -> switch the master head to the bug-fix branch

git switch master -> will switch head to master and bug-file(fixes.txt) will be removes

git switch -c dark-mode -> create dark-mode branch and switch to it in one command only

git checkout orange-mode ->checkout the branchand switch to it (orange-mode) branch in this case

.........................................................................

// git merging

// fast forward marge

git merge bug-fix -> merge the (fixes.txt) bug-fix branch with master branch note-> you should be on that branch on which you want to merge

// not fast forward merge

// conflict merge branch

git branch -m bug-fix bug-fixNew (remame a branch)

git branch -d bug-fix (delete any branch)

..........................................................................

git diff (informational command) like git log

git diff --staged (this command shows the changes between the last commit and staging area text which is not committed yet.)

git diff 6e53954..74b1f0a
           or
git diff 6e53954..74b1f0a

git diff bug-fix master

// stash -> store your changes in temporary location

git stash 

git stash list -> show all the stash lists

git stash apply

git stash pop (Apply and drop the stash)

git stash drop (drop the stash)

..........................................................................

git tags (sticky notes)

git tag  -a mchai -m "Release 1.0" (anonated tag)

git tag chai (tag creation)

..........................................................................

// git  rebase (change the base of branch)
ensure you are on the branch you want to rebase (sub-branch)

git rebase master (on subbranch 95%)(to remove the extra commits and it changes the history means locations change) (realign the base)

..........................................................................

// git reflog

git reflog (tells the history like log)

git reset --hard ffe3a68 (will reset to the previous values data)

..........................................................................

// GitHub

git remote add origin https://github.com/vardantyagi/git-hindi.git (add remote link)

git remote -v (for fetch and push details)

git push --set-upstream origin main (put/add data to existing file on github)