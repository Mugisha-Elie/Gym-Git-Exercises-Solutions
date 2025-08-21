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