Ostad-Assignment02-Task03


tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK
$ gh auth status
github.com
  ✓ Logged in to github.com account shajedultonmoy (keyring)
  - Active account: true
  - Git operations protocol: https
  - Token: gho_************************************
  - Token scopes: 'gist', 'read:org', 'repo', 'workflow'

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK
$ mkdir Ostad-Assignment02-Task03

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK
$ ls
Ostad-Assignment02-Task01/  Ostad-Assignment02-Task02/  Ostad-Assignment02-Task03/

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK
$ cd Ostad-Assignment02-Task03

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03
$ git init
Initialized empty Git repository in D:/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03/.git/

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (master)
$ echo "# Task 03 - Commit History" > README.md

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (master)
$ git add .
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (master)
$ git commit -m "Initial commit"
[master (root-commit) 5580757] Initial commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (master)
$ git branch -M main

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (main)
$ git remote add origin https://github.com/shajedultonmoy/Ostad-Assignment02-Task03.git

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 244 bytes | 122.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/shajedultonmoy/Ostad-Assignment02-Task03.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (main)
$ git checkout -b feature/login
Switched to a new branch 'feature/login'

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$ git push -u origin feature/login
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'feature/login' on GitHub by visiting:
remote:      https://github.com/shajedultonmoy/Ostad-Assignment02-Task03/pull/new/feature/login
remote:
To https://github.com/shajedultonmoy/Ostad-Assignment02-Task03.git
 * [new branch]      feature/login -> feature/login
branch 'feature/login' set up to track 'origin/feature/login'.

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$ echo "Login UI" > login.txt

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$ git add .
warning: in the working copy of 'login.txt', LF will be replaced by CRLF the next time Git touches it

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$ git commit -m "Add login UI"
[feature/login 98fcfa2] Add login UI
 1 file changed, 1 insertion(+)
 create mode 100644 login.txt

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$ echo "Login backend logic" >> login.txt

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$ git add .
warning: in the working copy of 'login.txt', LF will be replaced by CRLF the next time Git touches it

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$ git commit -m "Add login backend"
[feature/login 8c2cdd0] Add login backend
 1 file changed, 1 insertion(+)

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$ echo "Validation added" >> login.txt

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$ git add .
warning: in the working copy of 'login.txt', LF will be replaced by CRLF the next time Git touches it

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)




error: could not parse 'e5'
error: invalid line 1: reword e5 Add login UI
error: could not parse 'd4'
error: invalid line 2: squash d4 Add login backend
error: could not parse 'c3'
error: invalid line 3: squash c3 Add validation
error: could not parse 'b2'
error: invalid line 4: squash b2 Fix login bug
error: could not parse 'a1'
error: invalid line 5: squash a1 Optimize login
You can fix this with 'git rebase --edit-todo' and then run 'git rebase --continue'.
Or you can abort the rebase with 'git rebase --abort'.

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login|REBASE)
$ git rebase -i HEAD~5
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login|REBASE)
$ git rebase -i HEAD~5






[detached HEAD a18f29d] feat: implement complete login system with UI, backend, validation, bug fix, optimization
 Date: Tue Apr 14 19:33:02 2026 +0600
 1 file changed, 1 insertion(+)
 create mode 100644 login.txt
[detached HEAD 5c54831] feat: implement complete login system with UI, backend, validation, bug fix, optimization
 Date: Tue Apr 14 19:33:02 2026 +0600
 1 file changed, 5 insertions(+)
 create mode 100644 login.txt
Successfully rebased and updated refs/heads/feature/login.

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$ git rebase --continue
fatal: no rebase in progress

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$ git push --force
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 437 bytes | 437.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/shajedultonmoy/Ostad-Assignment02-Task03.git
   5580757..5c54831  feature/login -> feature/login

tonmo@GHOST MINGW64 /d/DEVOPS WORKS/WORK/Ostad-Assignment02-Task03 (feature/login)
$

