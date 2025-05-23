# Gym-Git-Exercise-Solutions-Part1
## Bundle 1
### Exercie 1
```bash
PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT (main)
$ mkdir git-exercise-1

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT (main)
$ 

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT (main)
$ cd git-exercise-1

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git init
Initialized empty Git repository in C:/Users/PC/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1/.git/

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (master)
$ touch index.html

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (master)
$ git branch -m master main

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git add --all

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git commit -m"Part 1"
[main (root-commit) f77537b] Part 1
 1 file changed, 11 insertions(+)
 create mode 100644 index.html

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git remote add origin https://github.com/Adiiaa/Gym-Git-Exercise-Solutions-Part1.git

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git pull origin main --allow-unrelated-histories
fatal: couldn't find remote ref main

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 382 bytes | 9.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Adiiaa/Gym-Git-Exercise-Solutions-Part1.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git checkout -b dev
Switched to a new branch 'dev'

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git checkout -b test
Switched to a new branch 'test'

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (test)
$ git checkout dev
Switched to branch 'dev'

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git branch -D test
Deleted branch test (was f77537b).

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git add --all

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git commit -m"switching branches"
On branch dev
nothing to commit, working tree clean

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$  git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Adiiaa/Gym-Git-Exercise-Solutions-Part1/pull/new/dev
remote:
To https://github.com/Adiiaa/Gym-Git-Exercise-Solutions-Part1.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.
```


## Bundle 1
### Exercise 2
```bash
PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ touch home.html

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git add --all

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git stash
Saved working directory and index state WIP on dev: f77537b Part 1

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ touch about.html

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git add --all

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git stash
Saved working directory and index state WIP on dev: f77537b Part 1

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ touch team.html

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git add --all

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git stash
Saved working directory and index state WIP on dev: f77537b Part 1

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git stash list
stash@{0}: WIP on dev: f77537b Part 1
stash@{1}: WIP on dev: f77537b Part 1
stash@{2}: WIP on dev: f77537b Part 1

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (2e1224013641ae71151181dd650c25a9d1610f76)

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (991c5a1c555052c63657654a283e3bab8c386581)

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git add --all

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git commit -m "Restoring about.html and home.html from stash"
[dev 054f1e4] Restoring about.html and home.html from stash
 2 files changed, 5 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 373 bytes | 124.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Adiiaa/Gym-Git-Exercise-Solutions-Part1.git
   f77537b..054f1e4  dev -> dev

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (e7e8d1af8422fbf6bf58b5c5400536dc7fd9a295)

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (dev)
$ git reset --hard
HEAD is now at 054f1e4 Restoring about.html and home.html from stash
```
