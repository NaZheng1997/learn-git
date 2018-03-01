Git is a version control system.
Git is free software.

init: 
git init

add files: 
git add <file> //many files <file1 file2 etc.>
git commit -m "explain"

know the status:
git status

know the difference:
git diff

view the last three changes:
git log

view the last and future changes:
git reflog

back to the previous version:
git reset --hard commit-id

remove files:
git rm

restore flies:
git checkout

Push the latest changes:
git push origin master


-------------------------------------


$ git checkout -b dev//$ git branch dev   +   $ git checkout dev
Switched to a new branch 'dev'
$ git branch
* dev
  master
  
$ git add readme.txt 
$ git commit -m "branch test"
[dev fec145a] branch test
 1 file changed, 1 insertion(+)
 
$ git checkout master
Switched to branch 'master'

$ git merge dev
Updating d17efd8..fec145a
Fast-forward
 readme.txt |    1 +
 1 file changed, 1 insertion(+)
 
$ git branch -d dev
Deleted branch dev (was fec145a).

$ git branch
* master


-------------------------------------


$ git merge dev//Save the history branch
$ git merge --no-ff -m "merge with no-ff" dev