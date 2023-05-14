# Gym-Git-Exercise-Solutions

## Bundle 1

### Exercise 1
```bash
User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises (master)
$ mkdir NewProject

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises (master)
$ cd NewProject

User@DESKTOP-I1ARRFM MINGW64 ~/Documents/Project/The Gym/Git Exercises/NewProject (master)
$ git init
Initialized empty Git repository in C:/Users/User/Documents/Project/The Gym/Git Exercises/


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
