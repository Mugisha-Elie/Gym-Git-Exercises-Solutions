# Gym-Git-Exercises-Solutions

## Bundle 1

### Exercise 1

```bash
- Command for initialize git in a local repo
git init

- Command to rename a branch
$ git branch -M master

- Command to check staged or unstaged status
$ git status

- Command for staging
$ git add index.html

- Command for referencing a remote and creating origin
$ git remote add origin "https://github.com/Mugisha-Elie/Git-Exercises"

- Command for committing with an inline message
$ git commit -m "initial exercise"

- Command for pushing on a new origin
$ git push -u origin main

- Command for creating a new branch and directly working on it
$ git checkout -b dev
Switched to a new branch 'dev'

- Command for deleting a branch locally
$ git branch -d test
Deleted branch test (was 9ae8a2e)
```

### Exercise 2

```bash
- Command for stashing / saving uncommitted changes
$ git stash
Saved working directory and index state WIP on main: 9ae8a2e initial exercise

- Command for checking the list of stashed items
$ git stash list
stash@{0}: WIP on main: 9ae8a2e initial exercise
stash@{1}: WIP on main: 9ae8a2e initial exercise
stash@{2}: WIP on main: 9ae8a2e initial exercise

- Command for popping a stash at a specific index
$ git stash pop stash@{2}

- Command for popping the previously stashed change
$ git stash pop

- Command for pushing on an already existing branch
$ git push

- Command for reseting to the previous change
$ git reset
```

## Bundle 2

### Exercise 1

```bash
- Command for staging all files in the current directory and sub directories
$ git add .
```

### Exercise 2

```bash
- Command for changing to an already existing branch
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

- Command for pulling new commits into local working repo
$ git pull

- The git fetch command downloads remote changes to the local repo without intergrating them to your local files while git pull downloaads and automatically merges the changes into your local files

- Command to do a remote fetch
$ git fetch

- Command to do a remote pull
$ git pull

- Command to check the differences between two branches
$ git diff ft/service-redesign main

- Command to perforom a merge on the local repository
⚠ It merges the specified branch to the branch you are currently on
$ git merge ft/service-redesign

$ git merge main
Updating 599754a..979ef8e
Fast-forward
 services.html | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

```

## Bundle 3

### Exercise 1

```bash
- Command to check commit history and view commit hashes, branch and author
$ git log

- Command to minimize the size of the output from the commit history
$ git log --oneline

- Command to move a commit from one branch to another without merging
$ git cherry-pick cb06e4e612e8b2dd7ec3a003a219b228ce891af9

- Command to to revert to a specific commit
$ git revert cb06e4e612e8b2dd7ec3a003a219b228ce891af9            

```