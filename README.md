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

## Bundle 2
### Exercise 2

``bash 

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git pull origin main
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 1.95 KiB | 10.00 KiB/s, done.
From https://github.com/Adiiaa/Gym-Git-Exercise-Solutions-Part1
 * branch            main       -> FETCH_HEAD
   26f5c9b..9bef488  main       -> origin/main
Updating 26f5c9b..9bef488
Fast-forward
 about.html   | 3 +++
 home.html    | 2 ++
 service.html | 4 ++++
 3 files changed, 9 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 service.html

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (ft/service-redesign)
$ git add --all

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (ft/service-redesign)
$ git commit -m "Redesigning the service heading"
[ft/service-redesign 9443e50] Redesigning the service heading
 1 file changed, 1 insertion(+), 1 deletion(-)

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (ft/service-redesign)
$ git push -u origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 358 bytes | 179.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Adiiaa/Gym-Git-Exercise-Solutions-Part1/pull/new/ft/service-redesign
remote:
To https://github.com/Adiiaa/Gym-Git-Exercise-Solutions-Part1.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git add --all

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git commit -m "Updating the service page in main"
[main 32c35b6] Updating the service page in main
 1 file changed, 1 insertion(+), 1 deletion(-)

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 362 bytes | 90.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Adiiaa/Gym-Git-Exercise-Solutions-Part1.git
   9bef488..32c35b6  main -> main

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (ft/service-redesign)
$ git fetch origin

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (ft/service-redesign)
$ git diff origin/main
diff --git a/service.html b/service.html
index 60f90a7..7347fa2 100644
--- a/service.html
+++ b/service.html
@@ -1,4 +1,4 @@


-<h1>Exploring Our Services</h1>
+<h1>Our Premium Services</h1>
 <p>We offer gym, personal training, nutrition plans, and more.</p>

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (ft/service-redesign)
$ git merge origin/main
Auto-merging service.html
CONFLICT (content): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (ft/service-redesign|MERGING)
$ git add --all

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (ft/service-redesign|MERGING)
$ git commit -m "solving the conflicts"
[ft/service-redesign e60b831] solving the conflicts

PC@DESKTOP-VBG4P66 MINGW64 ~/Desktop/codes/THE GYM PHASE 2/GIT/git-exercise-1 (ft/service-redesign)
$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 334 bytes | 334.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Adiiaa/Gym-Git-Exercise-Solutions-Part1.git
   9443e50..e60b831  ft/service-redesign -> ft/service-redesign
```
