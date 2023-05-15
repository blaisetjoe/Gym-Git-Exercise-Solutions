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
### Exercise 2
```bash

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git add home.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 62c4374 added changes to readme

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git add about.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 62c4374 added changes to readme

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash list
stash@{0}: WIP on dev: 62c4374 added changes to readme
stash@{1}: WIP on dev: 62c4374 added changes to readme

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git add team.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 62c4374 added changes to readme

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash list
stash@{0}: WIP on dev: 62c4374 added changes to readme
stash@{1}: WIP on dev: 62c4374 added changes to readme
stash@{2}: WIP on dev: 62c4374 added changes to readme

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (3e1b4b55f9abee059a1b5275bc7d8238c4c4cf5a)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash list
stash@{0}: WIP on dev: 62c4374 added changes to readme
stash@{1}: WIP on dev: 62c4374 added changes to readme

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (acc15ec79a60085f96a61259e8efdfcb6e878714)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git add about.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git add home.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git commit -m "updated home and about pages"
[dev 89133d8] updated home and about pages
 2 files changed, 24 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash list
stash@{0}: WIP on dev: 62c4374 added changes to readme

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash pop stash@{0}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (ea583ed2ed07538eb2a3c497abd694985fab6d05)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 89133d8 updated home and about pages

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash list
stash@{0}: WIP on dev: 89133d8 updated home and about pages

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git status
On branch dev
nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git push --set-upstream origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 539 bytes | 269.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
git stash list
git status
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/blaisetjoe/Bundle-1/pull/new/dev
remote:
To https://github.com/blaisetjoe/Bundle-1.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash list
stash@{0}: WIP on dev: 89133d8 updated home and about pages

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ t status
bash: t: command not found

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (eb2f178a93718dec5c27f83504667b2f5db37cd1)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git reset --hard
HEAD is now at 89133d8 updated home and about pages

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$
```
## Bundle 2
## Exercise 1

```bash

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (dev)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html
        modified:   home.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

no changes added to commit (use "git add" and/or "git commit -a")

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/bundle-2)
$ git add --all

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   about.html
        modified:   home.html
        new file:   services.html


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/bundle-2)
$ git commit -m "added changes at bundle-2 exercise-1"
[ft/bundle-2 1f1d341] added changes at bundle-2 exercise-1
 3 files changed, 14 insertions(+)
 create mode 100644 services.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/bundle-2)
$  git push --set-upstream origin ft/bundle-2
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 550 bytes | 110.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/blaisetjoe/Bundle-1/pull/new/ft/bundle-2
remote:
To https://github.com/blaisetjoe/Bundle-1.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/bundle-2)
$
```
