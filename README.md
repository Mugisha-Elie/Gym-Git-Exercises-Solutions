# Gym-Git-Exercises-Solutions

## Bundle 1

### Exercise 1

```bash
hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises
$ git init
Initialized empty Git repository in C:/Users/hp/Desktop/Git Exercises/.git/

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git branch -M master

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (master)
$ git branch -M main

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git add index.html

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git remote add origin "https://github.com/Mugisha-Elie/Git-Exercises"

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git commit -m "initial exercise"
[main (root-commit) 9ae8a2e] initial exercise
 1 file changed, 11 insertions(+)
 create mode 100644 index.html

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 387 bytes | 129.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Mugisha-Elie/Git-Exercises
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git checkout -b dev
Switched to a new branch 'dev'

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (dev)
$ git checkout -b test
Switched to a new branch 'test'

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (test)
$ git checkout dev
Switched to branch 'dev'
gi
hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (dev)
$ git branch -d test
Deleted branch test (was 9ae8a2e)
```

### Exercise 2

```bash
hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git add home.html

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 9ae8a2e initial exercise

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git add team.html

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 9ae8a2e initial exercise

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)
g
hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git add about.html

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git stash
Saved working directory and index state WIP on main: 9ae8a2e initial exercise

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git stash list
stash@{0}: WIP on main: 9ae8a2e initial exercise
stash@{1}: WIP on main: 9ae8a2e initial exercise
stash@{2}: WIP on main: 9ae8a2e initial exercise

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git stash pop stash@{2}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped stash@{2} (864e7ee8ea820576edd93b68c15416f47cc25fed)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped refs/stash@{0} (90aa22ec0cea81505cc9f8a32171115c1bd902e7)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git commit -m "exercise2 commit"
[main 4fe50fe] exercise2 commit
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 521 bytes | 74.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Mugisha-Elie/Git-Exercises
   9ae8a2e..4fe50fe  main -> main

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (5290a0b5be1813f3950d8bf3f26c9bace764b382)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git reset
```