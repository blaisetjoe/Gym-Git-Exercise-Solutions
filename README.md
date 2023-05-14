# Gym-Git-Exercise-Solutions

## Bundle 1
### Exercise 1

```bash

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1
$ git init
Initialized empty Git repository in D:/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1/.git/

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (master)
$ git branch -m main

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git add --all

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git commit -m "added change to readme"
[main (root-commit) afa7e6d] added change to readme
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git remote add origin https://github.com/blaisetjoe/Bundle-1.git

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git push --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 241 bytes | 80.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/blaisetjoe/Bundle-1.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git branch dev

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git checkout dev
Switched to branch 'dev'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git branch test

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git branch
* dev
  main
  test

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git branch -d test
Deleted branch test (was afa7e6d).

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$
```
