```bash
vladt@Vlads-MacBook-Pro-2 studentManager-main % git init 
Initialized empty Git repository in /Users/vladt/Downloads/studentManager-main/.git/
vladt@Vlads-MacBook-Pro-2 studentManager-main % git remote add origin https://github.com/VladTomici14/sef-repo.git

vladt@Vlads-MacBook-Pro-2 studentManager-main % git add . 
vladt@Vlads-MacBook-Pro-2 studentManager-main % git commit -m "first commit"
[main (root-commit) accb3ad] first commit
 10 files changed, 406 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 README.md
 create mode 100644 pom.xml
 create mode 100644 src/main/java/loose/oose/fis/lab/student/manager/Main.java
 create mode 100644 src/main/java/loose/oose/fis/lab/student/manager/controllers/LoginController.java
 create mode 100644 src/main/java/loose/oose/fis/lab/student/manager/controllers/ViewStudentsController.java
 create mode 100644 src/main/java/loose/oose/fis/lab/student/manager/model/Student.java
 create mode 100644 src/main/resources/css/styles.css
 create mode 100644 src/main/resources/fxml/login.fxml
 create mode 100644 src/main/resources/fxml/view-students.fxml
vladt@Vlads-MacBook-Pro-2 studentManager-main % git push 
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

vladt@Vlads-MacBook-Pro-2 studentManager-main % git push --set-upstream origin main 
Enumerating objects: 26, done.
Counting objects: 100% (26/26), done.
Delta compression using up to 8 threads
Compressing objects: 100% (16/16), done.
Writing objects: 100% (26/26), 5.32 KiB | 5.32 MiB/s, done.
Total 26 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/VladTomici14/sef-repo.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
vladt@Vlads-MacBook-Pro-2 studentManager-main % git checkout -b new-branch
Switched to a new branch 'new-branch'
vladt@Vlads-MacBook-Pro-2 studentManager-main % git branch
  main
* new-branch
vladt@Vlads-MacBook-Pro-2 studentManager-main % idea . 
vladt@Vlads-MacBook-Pro-2 studentManager-main % idea . 
vladt@Vlads-MacBook-Pro-2 studentManager-main % git status
On branch new-branch
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   src/main/java/loose/oose/fis/lab/student/manager/Main.java

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	src/main/java/loose/oose/fis/lab/student/manager/controllers/TestController.java

no changes added to commit (use "git add" and/or "git commit -a")
vladt@Vlads-MacBook-Pro-2 studentManager-main % git add . 
vladt@Vlads-MacBook-Pro-2 studentManager-main % git commit -m "added a class comment and created a new test class"
[new-branch 52cb873] added a class comment and created a new test class
 2 files changed, 7 insertions(+)
 create mode 100644 src/main/java/loose/oose/fis/lab/student/manager/controllers/TestController.java
vladt@Vlads-MacBook-Pro-2 studentManager-main % git push 
fatal: The current branch new-branch has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin new-branch

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

vladt@Vlads-MacBook-Pro-2 studentManager-main % git branch   
  main
  new-branch
* new-new-branch
vladt@Vlads-MacBook-Pro-2 studentManager-main % git branch
  main
  new-branch
* new-new-branch
vladt@Vlads-MacBook-Pro-2 studentManager-main % git branch
  main
  new-branch
* new-new-branch
vladt@Vlads-MacBook-Pro-2 studentManager-main % git status
On branch new-new-branch
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   src/main/java/loose/oose/fis/lab/student/manager/Main.java

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	src/main/java/loose/oose/fis/lab/student/manager/controllers/ExerciseClass.java

no changes added to commit (use "git add" and/or "git commit -a")
vladt@Vlads-MacBook-Pro-2 studentManager-main % git add . 
vladt@Vlads-MacBook-Pro-2 studentManager-main % git commit -m "branch update"
[new-new-branch 2f6e3fa] branch update
 2 files changed, 15 insertions(+)
 create mode 100644 src/main/java/loose/oose/fis/lab/student/manager/controllers/ExerciseClass.java
vladt@Vlads-MacBook-Pro-2 studentManager-main % git checkout new-branch
Switched to branch 'new-branch'
vladt@Vlads-MacBook-Pro-2 studentManager-main % git merge main
Already up to date.
vladt@Vlads-MacBook-Pro-2 studentManager-main % git branch 
  main
* new-branch
  new-new-branch
vladt@Vlads-MacBook-Pro-2 studentManager-main % git status
On branch new-branch
nothing to commit, working tree clean
vladt@Vlads-MacBook-Pro-2 studentManager-main % git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
vladt@Vlads-MacBook-Pro-2 studentManager-main % git merge new-branch
Updating accb3ad..52cb873
Fast-forward
 src/main/java/loose/oose/fis/lab/student/manager/Main.java                       | 2 ++
 src/main/java/loose/oose/fis/lab/student/manager/controllers/TestController.java | 5 +++++
 2 files changed, 7 insertions(+)
 create mode 100644 src/main/java/loose/oose/fis/lab/student/manager/controllers/TestController.java
vladt@Vlads-MacBook-Pro-2 studentManager-main % git branch -d new-branch
Deleted branch new-branch (was 52cb873).
vladt@Vlads-MacBook-Pro-2 studentManager-main % git branch 
* main
  new-new-branch
vladt@Vlads-MacBook-Pro-2 studentManager-main % git push 
Enumerating objects: 52, done.
Counting objects: 100% (52/52), done.
Delta compression using up to 8 threads
Compressing objects: 100% (19/19), done.
Writing objects: 100% (40/40), 2.70 KiB | 2.70 MiB/s, done.
Total 40 (delta 8), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (8/8), completed with 2 local objects.
To https://github.com/VladTomici14/sef-repo.git
   accb3ad..67cb552  main -> main
vladt@Vlads-MacBook-Pro-2 studentManager-main % 
```
