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
### Exercise 2

```bash

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git branch -b ft/service-redesign
error: unknown switch `b'
usage: git branch [<options>] [-r | -a] [--merged] [--no-merged]
   or: git branch [<options>] [-f] [--recurse-submodules] <branch-name> [<start-point>]
   or: git branch [<options>] [-l] [<pattern>...]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --verbose         show hash and subject, give twice for upstream branch
    -q, --quiet           suppress informational messages
    -t, --track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --set-upstream-to <upstream>
                          change the upstream info
    --unset-upstream      unset the upstream info
    --color[=<when>]      use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --abbrev[=<n>]        use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --delete          delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --move            move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    -c, --copy            copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --list            list branch names
    --show-current        show current branch name
    --create-reflog       create the branch's reflog
    --edit-description    edit the description for the branch
    -f, --force           force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --column[=<style>]    list branches in columns
    --sort <key>          field name to sort on
    --points-at <object>  print only branches of the object
    -i, --ignore-case     sorting and filtering are case insensitive
    --recurse-submodules  recurse through submodules
    --format <format>     format to use for the output


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git status
On branch ft/service-redesign
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

nothing added to commit but untracked files present (use "git add" to track)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git add services.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git commit -m "added changes to services page"
[ft/service-redesign 48f5336] added changes to services page
 1 file changed, 13 insertions(+)
 create mode 100644 services.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
git reset --hard
fatal: unable to access 'https://github.com/blaisetjoe/Bundle-1.git/': Recv failure: Connection was reset

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git reset --hard
HEAD is now at 48f5336 added changes to services page

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 658 bytes | 2.00 KiB/s, done.
From https://github.com/blaisetjoe/Bundle-1
   62c4374..db23dc0  main       -> origin/main
Updating 62c4374..db23dc0
Fast-forward
 about.html    | 13 +++++++++++++
 home.html     | 13 +++++++++++++
 services.html | 12 ++++++++++++
 3 files changed, 38 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git add services.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git commit -m "added changes to services html"
[ft/service-redesign fa2819e] added changes to services html
 1 file changed, 1 insertion(+)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 799 bytes | 133.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/blaisetjoe/Bundle-1/pull/new/ft/service-redesign
remote:
To https://github.com/blaisetjoe/Bundle-1.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git add services.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git commit -m "added other changes to services"
[main e6cb009] added other changes to services
 1 file changed, 1 insertion(+), 1 deletion(-)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 333 bytes | 111.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/blaisetjoe/Bundle-1.git
   db23dc0..e6cb009  main -> main

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git checkout
Your branch is up to date with 'origin/main'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git diff

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git merge ft/service-redesign
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main|MERGING)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git merge ft/service-redesign
Already up to date.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git push
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 946 bytes | 236.00 KiB/s, done.
Total 9 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
To https://github.com/blaisetjoe/Bundle-1.git
   e6cb009..f46e164  main -> main

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$
```
## Bunlde 3
### Exercise 1

```bash


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/team-page)
$ git status
On branch ft/team-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/team-page)
$ git add team.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/team-page)
$ git commit -m "added team page"
[ft/team-page d2bb990] added team page
 1 file changed, 12 insertions(+)
 create mode 100644 team.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 4 threads
Compressing objects: 100% (16/16), done.
Writing objects: 100% (16/16), 2.11 KiB | 45.00 KiB/s, done.
Total 16 (delta 8), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (8/8), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/blaisetjoe/Bundle-1/pull/new/ft/team-page
remote:
To https://github.com/blaisetjoe/Bundle-1.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/team-page)
$ git log
commit d2bb99038a7c998a20b247c07fcaafdb23c11366 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Tue May 16 09:40:46 2023 +0200

    added team page

commit f46e164294fe7b0c66eff7061a32c385977483f3 (origin/main, main, ft/contact-page)
Merge: e6cb009 fa2819e
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:38:53 2023 +0200

    Merge branch 'ft/service-redesign'

commit e6cb009c515c62829a015038a6ff7ab484bb6b4f
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:30:12 2023 +0200

    added other changes to services

commit fa2819ee422d5a4d39affefcd901cc20ad0b58d0 (origin/ft/service-redesign, ft/service-redesign)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:18:33 2023 +0200

    added changes to services html

commit 48f53360a97856da589ffd4598e88dcf2a736b4f
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:10:39 2023 +0200

    added changes to services page

commit db23dc055cc0a59c80e4345933603f5eed8cc410
commit db23dc055cc0a59c80e4345933603f5eed8cc410
commit d2bb99038a7c998a20b247c07fcaafdb23c11366 (HEAD -> ft/team-page,
 origin/ft/team-page)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Tue May 16 09:40:46 2023 +0200

    added team page

commit f46e164294fe7b0c66eff7061a32c385977483f3 (origin/main, main, ft
/contact-page)
Merge: e6cb009 fa2819e
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:38:53 2023 +0200

    Merge branch 'ft/service-redesign'

commit e6cb009c515c62829a015038a6ff7ab484bb6b4f
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:30:12 2023 +0200

    added other changes to services

commit fa2819ee422d5a4d39affefcd901cc20ad0b58d0 (origin/ft/service-red
esign, ft/service-redesign)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:18:33 2023 +0200

    added changes to services html

commit 48f53360a97856da589ffd4598e88dcf2a736b4f
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:10:39 2023 +0200

    added changes to services page

commit db23dc055cc0a59c80e4345933603f5eed8cc410
Merge: 62c4374 1f1d341
Author: Annette <74765874+Annette-Bwemere-Salama@users.noreply.github.com>
Date:   Mon May 15 12:00:53 2023 +0200

    Merge pull request #1 from blaisetjoe/ft/bundle-2

    added changes to project and created new

commit 1f1d34183d34afbf718100989e922510845be860 (origin/ft/bundle-2, ft/bundle-2)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:53:23 2023 +0200

    added changes at bundle-2 exercise-1

commit 89133d819551ec15e36f60062766f42c6a61d5d3 (origin/dev, dev)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:34:30 2023 +0200

    updated home and about pages

commit 62c437434dec0621b0c74d24d31071f36a2ebc11
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:18:48 2023 +0200

    added changes to readme

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/contact-page)
$ git cherry-pick d2bb99038a7c998a20b247c07fcaafdb23c11366
[ft/contact-page 4f24979] added team page
 Date: Tue May 16 09:40:46 2023 +0200
 1 file changed, 12 insertions(+)
 create mode 100644 team.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/contact-page)
$ git git status
git: 'git' is not a git command. See 'git --help'.

The most similar command is
        init

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/contact-page)
$ git status
On branch ft/contact-page
nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/contact-page)
$ git status
On branch ft/contact-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/contact-page)
$ git add team.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/contact-page)
$ git commit -m "added changes on contact>team page"
[ft/contact-page 71c30df] added changes on contact>team page
 1 file changed, 1 insertion(+)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/contact-page)
$  git push --set-upstream origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 734 bytes | 244.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/blaisetjoe/Bundle-1/pull/new/ft/contact-page
remote:
To https://github.com/blaisetjoe/Bundle-1.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page)
$ git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page)
$ git add faq.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page)
$ git commit -m "added faq page"
[ft/faq-page 6c12c33] added faq page
 1 file changed, 12 insertions(+)
 create mode 100644 faq.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 470 bytes | 156.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/blaisetjoe/Bundle-1/pull/new/ft/faq-page
remote:
To https://github.com/blaisetjoe/Bundle-1.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
CONFLICT (modify/delete): team.html deleted in parent of d2bb990 (added team page) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert d2bb990... added team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
CONFLICT (modify/delete): team.html deleted in parent of d2bb990 (added team page) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert d2bb990... added team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
CONFLICT (modify/delete): team.html deleted in parent of d2bb990 (added team page) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert d2bb990... added team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
CONFLICT (modify/delete): team.html deleted in parent of d2bb990 (added team page) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert d2bb990... added team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

You are currently reverting commit d2bb990.
  (fix conflicts and run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add/rm <file>..." as appropriate to mark resolution)
        deleted by them: team.html

no changes added to commit (use "git add" and/or "git commit -a")

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git add team.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert --continue
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

You are currently reverting commit d2bb990.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

You are currently reverting commit d2bb990.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git push
Everything up-to-date

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

You are currently reverting commit d2bb990.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert --continue
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

You are currently reverting commit d2bb990.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git commit -m "revert"
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

You are currently reverting commit d2bb990.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
CONFLICT (modify/delete): team.html deleted in parent of d2bb990 (added team page) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert d2bb990... added team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
error: your local changes would be overwritten by revert.
hint: commit your changes or stash them to proceed.
fatal: revert failed

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
CONFLICT (modify/delete): team.html deleted in parent of d2bb990 (added team page) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert d2bb990... added team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
CONFLICT (modify/delete): team.html deleted in parent of d2bb990 (added team page) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert d2bb990... added team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
CONFLICT (modify/delete): team.html deleted in parent of d2bb990 (added team page) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert d2bb990... added team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
error: Reverting is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: revert failed

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
error: Reverting is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: revert failed

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert d2bb99038a7c998a20b247c07fcaafdb23c11366
CONFLICT (modify/delete): team.html deleted in parent of d2bb990 (added team page) and modified in HEAD.  Version HEAD of team.html left in tree.
error: could not revert d2bb990... added team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

You are currently reverting commit d2bb990.
  (fix conflicts and run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add/rm <file>..." as appropriate to mark resolution)
        deleted by them: team.html

no changes added to commit (use "git add" and/or "git commit -a")

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git add team.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

You are currently reverting commit d2bb990.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert --continue
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

You are currently reverting commit d2bb990.
  (all conflicts fixed: run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page|REVERTING)
$ git revert --skip

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page)
$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page)
$ git push
Everything up-to-date

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page)
$ git log
commit 5076f6f9656b040ae3a2f066c0adf23120e9d015 (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Tue May 16 10:16:53 2023 +0200

    Revert "added team page"

    This reverts commit d2bb99038a7c998a20b247c07fcaafdb23c11366.

commit bac37f0a97619edb3b93b98527580936b38bcdc0
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Tue May 16 10:14:39 2023 +0200

    Revert "added team page"

    This reverts commit d2bb99038a7c998a20b247c07fcaafdb23c11366.

commit 432f3d1c88ee200a179e1328ac881cd26d9ac8f2
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Tue May 16 10:13:51 2023 +0200

    Revert "added team page"

    This reverts commit d2bb99038a7c998a20b247c07fcaafdb23c11366.

commit ba36a1a3e85abe183f14b02ede698ac6d5f6e18f
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Tue May 16 10:13:19 2023 +0200

    Revert "added team page"

    This reverts commit d2bb99038a7c998a20b247c07fcaafdb23c11366.

commit 4fa62724d5cc47cf570dfc58952058f6b086e73e
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Tue May 16 10:06:16 2023 +0200

    Revert "added team page"

    This reverts commit d2bb99038a7c998a20b247c07fcaafdb23c11366.

commit 6c12c33ef910d86db13e787f3181abcca33bfc29
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Tue May 16 09:59:37 2023 +0200

    added faq page

commit 71c30dfbaf5a84b8f364c338629c8e17300929eb (origin/ft/contact-page, ft/contact-page)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Tue May 16 09:55:38 2023 +0200

    added changes on contact>team page

commit 4f249798f4dc36903409252269ed16ffbaf27bd3
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Tue May 16 09:40:46 2023 +0200

    added team page

commit f46e164294fe7b0c66eff7061a32c385977483f3 (origin/main, main)
Merge: e6cb009 fa2819e
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:38:53 2023 +0200

    Merge branch 'ft/service-redesign'

commit e6cb009c515c62829a015038a6ff7ab484bb6b4f
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:30:12 2023 +0200

    added other changes to services

commit fa2819ee422d5a4d39affefcd901cc20ad0b58d0 (origin/ft/service-redesign, ft/service-redesign)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:18:33 2023 +0200

    added changes to services html

commit 48f53360a97856da589ffd4598e88dcf2a736b4f
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 12:10:39 2023 +0200

    added changes to services page

commit db23dc055cc0a59c80e4345933603f5eed8cc410
Merge: 62c4374 1f1d341
Author: Annette <74765874+Annette-Bwemere-Salama@users.noreply.github.com>
Date:   Mon May 15 12:00:53 2023 +0200

    Merge pull request #1 from blaisetjoe/ft/bundle-2

    added changes to project and created new

commit 1f1d34183d34afbf718100989e922510845be860 (origin/ft/bundle-2, ft/bundle-2)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:53:23 2023 +0200

    added changes at bundle-2 exercise-1

commit 89133d819551ec15e36f60062766f42c6a61d5d3 (origin/dev, dev)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:34:30 2023 +0200

    updated home and about pages

commit 62c437434dec0621b0c74d24d31071f36a2ebc11
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:18:48 2023 +0200

    added changes to readme
 ESCOC



ers.noreply.github.com>


-2



igin/ft/bundle-2, ft/bundle-2)
>




igin/dev, dev)
>





>



 ESCOD

commit db23dc055cc0a59c80e4345933603f5eed8cc410
Merge: 62c4374 1f1d341
Author: Annette <74765874+Annette-Bwemere-Salama@users.noreply.github.com>
Date:   Mon May 15 12:00:53 2023 +0200

    Merge pull request #1 from blaisetjoe/ft/bundle-2

    added changes to project and created new

commit 1f1d34183d34afbf718100989e922510845be860 (origin/ft/bundle-2, ft/bundle-2)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:53:23 2023 +0200

    added changes at bundle-2 exercise-1

commit 89133d819551ec15e36f60062766f42c6a61d5d3 (origin/dev, dev)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:34:30 2023 +0200

    updated home and about pages

commit 62c437434dec0621b0c74d24d31071f36a2ebc11
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:18:48 2023 +0200

    added changes to readme
 ESCOD

commit db23dc055cc0a59c80e4345933603f5eed8cc410
Merge: 62c4374 1f1d341
Author: Annette <74765874+Annette-Bwemere-Salama@users.noreply.github.com>
Date:   Mon May 15 12:00:53 2023 +0200

    Merge pull request #1 from blaisetjoe/ft/bundle-2

    added changes to project and created new

commit 1f1d34183d34afbf718100989e922510845be860 (origin/ft/bundle-2, ft/bundle-2)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:53:23 2023 +0200

    added changes at bundle-2 exercise-1

commit 89133d819551ec15e36f60062766f42c6a61d5d3 (origin/dev, dev)
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:34:30 2023 +0200

    updated home and about pages

commit 62c437434dec0621b0c74d24d31071f36a2ebc11
Author: Blaise Igiraneza <blaiseigiraneza@gmail.com>
Date:   Mon May 15 10:18:48 2023 +0200

    added changes to readme

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page)
$
```

### Exercise 2

```bash 

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git add home.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git commit -m "added redesign to homepage"
[main 636af94] added redesign to homepage
 1 file changed, 1 insertion(+)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 330 bytes | 165.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/blaisetjoe/Bundle-1.git
   29393c3..636af94  main -> main

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/home-page-redesign)
$ git add home.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/home-page-redesign)
$ git commit -m "changes after rebase"
[ft/home-page-redesign 0519148] changes after rebase
 1 file changed, 1 insertion(+)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 720 bytes | 240.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/blaisetjoe/Bundle-1/pull/new/ft/home-page-redesign
remote:
To https://github.com/blaisetjoe/Bundle-1.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/home-page-redesign)
$
```

## Bundle 4
### Exercise 1

```bash

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git remote add git-copy https://github.com/blaisetjoe/exercise-clone-repo.git

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git remote
git-copy
origin

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git add home.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git commit -m "changes to home page after git-copy remote"
[main 610406c] changes to home page after git-copy remote
 1 file changed, 1 insertion(+)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git push origin
To https://github.com/blaisetjoe/Bundle-1.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/blaisetjoe/Bundle-1.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git push git-copy
Enumerating objects: 71, done.
Counting objects: 100% (71/71), done.
Delta compression using up to 4 threads
Compressing objects: 100% (67/67), done.
Writing objects: 100% (71/71), 10.83 KiB | 616.00 KiB/s, done.
Total 71 (delta 38), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (38/38), done.
To https://github.com/blaisetjoe/exercise-clone-repo.git
 * [new branch]      main -> main

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git push origin
To https://github.com/blaisetjoe/Bundle-1.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/blaisetjoe/Bundle-1.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git pull origin
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 640 bytes | 91.00 KiB/s, done.
From https://github.com/blaisetjoe/Bundle-1
   636af94..00d549b  main       -> origin/main
Auto-merging home.html
CONFLICT (content): Merge conflict in home.html
Automatic merge failed; fix conflicts and then commit the result.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main|MERGING)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git push origin
Everything up-to-date

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$
```
### Exercise 2

```bash 

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/footer)
$ git status
On branch ft/footer
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        footer.html

nothing added to commit but untracked files present (use "git add" to track)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/footer)
$ git add footer.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/footer)
$ git commit -m "first footer commit"
[ft/footer 6db0c73] first footer commit
 1 file changed, 12 insertions(+)
 create mode 100644 footer.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/footer)
$ git status
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   footer.html

no changes added to commit (use "git add" and/or "git commit -a")

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/footer)
$ git add footer.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/footer)
$ git commit -m "second footer commit"
[ft/footer 1059ded] second footer commit
 1 file changed, 1 insertion(+)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/footer)
$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/footer)
$ git push --set-upstream origin ft/footer
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 754 bytes | 251.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/blaisetjoe/Bundle-1/pull/new/ft/footer
remote:
To https://github.com/blaisetjoe/Bundle-1.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/footer)
$ git status
On branch ft/footer
Your branch is up to date with 'origin/ft/footer'.

nothing to commit, working tree clean

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/footer)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/squashing)
$ git merge --squash ft/footer
Updating 1f9cd8d..1059ded
Fast-forward
Squash commit -- not updating HEAD
 footer.html | 13 +++++++++++++
 1 file changed, 13 insertions(+)
 create mode 100644 footer.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/squashing)
$ git status
On branch ft/squashing
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   footer.html


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/squashing)
$ git add footer.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/squashing)
$ git commit -m "footer changes squashing"
[ft/squashing 3e6ccd2] footer changes squashing
 1 file changed, 13 insertions(+)
 create mode 100644 footer.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/squashing)
$ git push
fatal: The current branch ft/squashing has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/squashing

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/squashing)
$ git push --set-upstream origin ft/squashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 492 bytes | 28.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/blaisetjoe/Bundle-1/pull/new/ft/squashing
remote:
To https://github.com/blaisetjoe/Bundle-1.git
 * [new branch]      ft/squashing -> ft/squashing
branch 'ft/squashing' set up to track 'origin/ft/squashing'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/Bundle-1 (ft/squashing)
$

```

## Bundle 5 

### Exercise 1

link to github page: https://blaisetjoe.github.io/Bundle-1/

### Exercise 2

```bash 

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB
$ git clone https://github.com/blaisetjoe/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 100
Receiving objects: 100% (107/107), 1.95 MiB | 10.00 KiB/s, done.
Resolving deltas: 100% (5/5), done.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB
$ cd git-cafe-exercise

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (main)
$ git remote -v
origin  https://github.com/blaisetjoe/git-cafe-exercise.git (fetch)
origin  https://github.com/blaisetjoe/git-cafe-exercise.git (push)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (main)
$ git add index.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (main)
$ git commit -m "changed title"
[main 7e1ce00] changed title
 1 file changed, 1 insertion(+), 1 deletion(-)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 322 bytes | 161.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/blaisetjoe/git-cafe-exercise.git
   d1d3f9c..7e1ce00  main -> main

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (main)
$
```

## Bundle 6 

### Exercise 1

```bash

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (main)
$ git checkout -b ft/exercise1
Switched to a new branch 'ft/exercise1'

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (ft/exercise1)
$ git status
On branch ft/exercise1
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        menu.html

nothing added to commit but untracked files present (use "git add" to track)

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (ft/exercise1)
$ git add menu.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (ft/exercise1)
$ git commit -m "create new menu page"
[ft/exercise1 6569a72] create new menu page
 1 file changed, 12 insertions(+)
 create mode 100644 menu.html

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (ft/exercise1)
$ git push
fatal: The current branch ft/exercise1 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/exercise1

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (ft/exercise1)
$ git push --set-upstream origin ft/exercise1
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 474 bytes | 158.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/exercise1' on GitHub by visiting:
remote:      https://github.com/blaisetjoe/git-cafe-exercise/pull/new/ft/exercise1
remote:
To https://github.com/blaisetjoe/git-cafe-exercise.git
 * [new branch]      ft/exercise1 -> ft/exercise1
branch 'ft/exercise1' set up to track 'origin/ft/exercise1'.

pc@OPTIMUS-PRIME MINGW64 /d/LOCAL WEBSITES PROJECTS/THEGYM/GIT & GITHUB/git-cafe-exercise (ft/exercise1)
$
```



