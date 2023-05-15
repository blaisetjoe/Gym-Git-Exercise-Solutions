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
