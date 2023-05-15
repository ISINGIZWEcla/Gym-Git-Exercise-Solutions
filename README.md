# Gym-Git-Exercise-Solutions

## Bundle 1

### Exercise 1
```bash

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises (master)
$ mkdir Exercise1

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises (master)
$ cd Exercise1

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (master) 
$ git init
Initialized empty Git repository in C:/Users/User/Documents/Project/The Gym/Git Exercises/Exercise1/.git/

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (master)
$ git branch -m main master
error: refname refs/heads/main not found
fatal: Branch rename failed

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (master)
$ git branch -m master main

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git add .

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Index.html
        new file:   README.md
        new file:   grid.css


User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git commit -m "my first commit"
[main (root-commit) e0bd1b5] my first commit
 3 files changed, 57 insertions(+)
 create mode 100644 Index.html
 create mode 100644 README.md
 create mode 100644 grid.css

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git remote add orgin https://github.com/ISINGIZWEcla/Gym-Git-Exercise-Solutions.git

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git push
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>


User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git remote add orgin https://github.com/ISINGIZWEcla/Exercise1.git
error: remote orgin already exists.

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git remote set-url origin https://github.com/ISINGIZWEcla/Exercise1.git
error: No such remote 'origin'

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git remote set-url orgin https://github.com/ISINGIZWEcla/Exercise1.git

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git push
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>


User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git push Exercise1
fatal: 'Exercise1' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git push https://github.com/ISINGIZWEcla/Exercise1.git
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 904 bytes | 150.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/ISINGIZWEcla/Exercise1.git
 * [new branch]      main -> main

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git checkout -b dev
Switched to a new branch 'dev'

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git status
On branch dev
nothing to commit, working tree clean

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git push dev
fatal: 'dev' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git push
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>


User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git push orgin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/ISINGIZWEcla/Exercise1/pull/new/dev
remote:
To https://github.com/ISINGIZWEcla/Exercise1.git
 * [new branch]      dev -> dev

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git checkout -b test
Switched to a new branch 'test'

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (test)
$ git push orgin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/ISINGIZWEcla/Exercise1/pull/new/test
remote:
To https://github.com/ISINGIZWEcla/Exercise1.git
 * [new branch]      test -> test

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (test)
$ git checkout dev
Switched to branch 'dev'

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git branch -D test
Deleted branch test (was e0bd1b5).

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git push orgin --delete test 
To https://github.com/ISINGIZWEcla/Exercise1.git
 - [deleted]         test

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$
```
### Exercise 2

```bash
User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git add home.html

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git stash save "stash saving home pahe"
Saved working directory and index state On dev: stash saving home pahe

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git add about.html

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git stash save "stash saving about page"
Saved working directory and index state On dev: stash saving about page

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git add team.html

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git stash save "stash saving team page"
Saved working directory and index state On dev: stash saving team page

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git stash list
stash@{0}: On dev: stash saving team page
stash@{1}: On dev: stash saving about page
stash@{2}: On dev: stash saving home pahe

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (92de7c90fb67737d41d820b743336c6fb9e1f58b)

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (6c138dce4e0cf8120116449d3c93ed6349878a6e)

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git commit -m "Adding home and about pages"
[dev f298e9e] Adding home and about pages
 2 files changed, 276 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git push remote dev
fatal: 'remote' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git push orgin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.81 KiB | 371.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/ISINGIZWEcla/Exercise1.git
   e0bd1b5..f298e9e  dev -> dev

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git stash list
stash@{0}: On dev: stash saving team page

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git stash pop
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (590fa05124bee8dcc173fbe68527f4b20934f97d)

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git reset --hard
HEAD is now at f298e9e Adding home and about pages

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$
```

## Bundle2

### Exercise 1

```bash
User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (dev)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/bundle-2)
$ git add .

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/bundle-2)
$ git commit -m "adding services page"                                                                                                     
[ft/bundle-2 0d1d23e] adding services page
 1 file changed, 19 insertions(+)
 create mode 100644 services.html

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/bundle-2)
$ git push orgin ft/bundle-2
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.  
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (10/10), 2.73 KiB | 103.00 KiB/s, done.
Total 10 (delta 3), reused 0 (delta 0), pack-reused 0        
remote: Resolving deltas: 100% (3/3), done.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/ISINGIZWEcla/Exercise1/pull/new/ft/bundle-2
remote:
To https://github.com/ISINGIZWEcla/Exercise1.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/bundle-2)
```

### Exercise 2

```bash
User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git pull main
fatal: 'main' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git pull orgin main
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (4/4), 2.43 KiB | 12.00 KiB/s, done.
From https://github.com/ISINGIZWEcla/Exercise1
 * branch            main       -> FETCH_HEAD
   fa62f06..4cfc43d  main       -> orgin/main
Updating fa62f06..4cfc43d
Fast-forward
 about.html    | 138 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 home.html     | 138 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 services.html |  19 ++++++++
 3 files changed, 295 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign)
$ git add servises.html
fatal: pathspec 'servises.html' did not match any files

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign)
$ git add services.html                                                                                                                    

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign)
$ git commit -m "Adding services list"
[ft/service-redesign 20cfc39] Adding services list
 1 file changed, 5 insertions(+), 5 deletions(-)  

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign)
$ git push orgin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 377 bytes | 377.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/ISINGIZWEcla/Exercise1/pull/new/ft/service-redesign
remote:
To https://github.com/ISINGIZWEcla/Exercise1.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign)
$ git checkout main
Switched to branch 'main'

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git add .

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git commit -m "Adding Service Template"
[main fedda14] Adding Service Template
 1 file changed, 5 insertions(+), 5 deletions(-)

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git push
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>


User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git push orgin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 361 bytes | 180.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/ISINGIZWEcla/Exercise1.git
   4cfc43d..fedda14  main -> main

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git checkout ft/service-redesign
error: Your local changes to the following files would be overwritten by checkout:
        services.html
Please commit your changes or stash them before you switch branches.
Aborting

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git add .

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html


User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git checkout ft/service-redesign
error: Your local changes to the following files would be overwritten by checkout:
        services.html
Please commit your changes or stash them before you switch branches.
Aborting

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git commit -m "resolving conflict"
[main 414ec93] resolving conflict
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git reset

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git status
On branch main
nothing to commit, working tree clean

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign|MERGING)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign)
$ git push ft/service-redesign
fatal: 'ft/service-redesign' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign)
$ git push orrgin ft/service-redesign
fatal: 'orrgin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign)
$ git push orgin ft/service-redesign
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 468 bytes | 234.00 KiB/s, done.
Total 4 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To https://github.com/ISINGIZWEcla/Exercise1.git
   20cfc39..b922f68  ft/service-redesign -> ft/service-redesign

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/Exercise1 (ft/service-redesign)
```