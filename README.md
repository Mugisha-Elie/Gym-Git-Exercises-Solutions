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

## Bundle 2

### Exercise 1

```bash
hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/bundle-2)
$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html
        team.html

nothing added to commit but untracked files present (use "git add" to track)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/bundle-2)
$ git add .

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/bundle-2)
$ git commit -m "bundle2-exercise1 commit"
[ft/bundle-2 445ddf5] bundle2-exercise1 commit
 2 files changed, 22 insertions(+)
 create mode 100644 services.html
 create mode 100644 team.html

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/bundle-2)
$ git push -u origin ft/bundle-2
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 595 bytes | 297.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Mugisha-Elie/Git-Exercises/pull/new/ft/bundle-2
remote:
To https://github.com/Mugisha-Elie/Git-Exercises
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```

### Exercise 2

```bash
hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 917 bytes | 91.00 KiB/s, done.
From https://github.com/Mugisha-Elie/Git-Exercises
   4fe50fe..a818854  main       -> origin/main
Updating 4fe50fe..a818854
Fast-forward
 services.html | 11 +++++++++++
 team.html     | 11 +++++++++++
 2 files changed, 22 insertions(+)
 create mode 100644 services.html
 create mode 100644 team.html

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/service-redesign)
$ git add .

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/service-redesign)
$ git commit -m "add new changes to service"
[ft/service-redesign 599754a] add new changes to service
 1 file changed, 2 insertions(+)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/service-redesign)
$ git push -u origin ft/service-redesign
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 705 bytes | 176.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Mugisha-Elie/Git-Exercises/pull/new/ft/service-r
edesign
remote:
To https://github.com/Mugisha-Elie/Git-Exercises
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git add services.html

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git commit -m "modify services.html"
[main 15819c7] modify services.html
 1 file changed, 2 insertions(+)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git fetch
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 909 bytes | 60.00 KiB/s, done.
From https://github.com/Mugisha-Elie/Git-Exercises
   4e591d4..2d1797d  main       -> origin/main

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git pull
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main|MERGING)
$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 1 and 2 different commits each, respectively.
  (use "git pull" if you want to integrate the remote branch with yours)

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
        modified:   services.html


hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main|MERGING)
$ git commit -m "services from main"
[main 979ef8e] services from main

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/service-redesign)
$ git diff ft/service-redesign main
diff --git a/services.html b/services.html
index 8153429..8c08d63 100644
--- a/services.html
+++ b/services.html
@@ -19,6 +19,6 @@
         <li>Tourism</li>
     </ul>

-    <p>Contact us: Email: Johndoe@example.com</p>
+
 </body>
 </html>
\ No newline at end of file

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/service-redesign)
$ git merge ft/service-redesign
Already up to date.

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/service-redesign)
$ git merge main
Updating 599754a..979ef8e
Fast-forward
 services.html | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/service-redesign)
$ git commit -m "service after merge"
On branch ft/service-redesign
Your branch is ahead of 'origin/ft/service-redesign' by 3 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

hp@Mr-DESKTOP-2LKS69K MINGW64 ~/Desktop/Git Exercises (main)
$ git push
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Mugisha-Elie/Git-Exercises
   2d1797d..979ef8e  main -> main
```