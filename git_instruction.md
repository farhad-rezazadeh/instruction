### git instruction for beginners

git is distributed version control system ===> VCS



`git init` ===> start the git in a direct

`git status`====> show situation

standard file =====modify====> Stage ====commit===> standard file

`git add nameOFfile` ===> add file to git space(tracked by git) or staged modified file

or use `-A` for all of file or `*.extension` for specefic file type

`git commit -m "massage"` -===> commit file

each commit take a uniqe code

`HEAD` point to position that working on

`git diff HEAD` show changes

`git diff --staged` show changes which in stage

`git reset nameOFfile` unstage change

`git checkout -- nameOFfile` undo modified file to last commit

`git branch` show branchs

`git branch nameOFbranch` create a branch

`git checkout nameOFbranch` go to branch

`git merge nameOFbranch` merge nameOFbranch with branch A when you are on branch A

`git rm nameOFfile` delete from both git and file system

`git branch -d nameOFbranch` delete nameOFbranch

`git clone url` clone a repository

`git push origin master` push

`git pull origin maste` pull