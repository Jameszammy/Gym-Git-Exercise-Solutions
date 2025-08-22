# Gym-Git-Exercise-Solutions

# boundle 1

# exercise 1

...bash

jzamm@DESKTOP-96E9C5V MINGW64 ~
$ cd ProjectGym

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym
$ git init
Initialized empty Git repository in C:/Users/jzamm/ProjectGym/.git/

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ ls -a
./ ../ .git/

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ touch index.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main

No commits yet

Untracked files:
(use "git add <file>..." to include in what will be committed)
index.html

nothing added to commit but untracked files present (use "git add" to track)

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git add index.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main

No commits yet

Changes to be committed:
(use "git rm --cached <file>..." to unstage)
new file: index.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git commit -m "First commite"
[main (root-commit) bfc7e5a] First commite
1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 index.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ code index.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: index.html

no changes added to commit (use "git add" and/or "git commit -a")

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git add index.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
Changes to be committed:
(use "git restore --staged <file>..." to unstage)
modified: index.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git commit -m "I added new content to the index.html file"
[main 7caa264] I added new content to the index.html file
1 file changed, 11 insertions(+)

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
nothing to commit, working tree clean

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git branch

- main

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git branch -m main master

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (master)
$ git branch

- master

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (master)
$ git branch -m master main

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git branch

- main

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git remote add origin https://github.com/Jameszammy/Gym-Git-Exercise-Sol.git

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git pull origin main --allow-unrelated-histories
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (6/6), 2.33 KiB | 108.00 KiB/s, done.
From https://github.com/Jameszammy/Gym-Git-Exercise-Solutions

- branch main -> FETCH_HEAD
- [new branch] main -> origin/main
  Merge made by the 'ort' strategy.
  README.md | 108 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++
  +++++
  1 file changed, 108 insertions(+)
  create mode 100644 README.md

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git push -u origin main
...

##bundle one: exercise 2
...bash
jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ touch home.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ code home.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git add home.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git commit -m "adding home.html file"
[main cfba84f] adding home.html file
1 file changed, 11 insertions(+)
create mode 100644 home.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
(use "git push" to publish your local commits)

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: README.md
modified: home.html

no changes added to commit (use "git add" and/or "git commit -a")

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git stash
Saved working directory and index state WIP on main: cfba84f adding home.html fi
le

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
(use "git push" to publish your local commits)

nothing to commit, working tree clean

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ touch about.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git add about.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ code about.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
(use "git push" to publish your local commits)

Changes to be committed:
(use "git restore --staged <file>..." to unstage)
new file: about.html

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: about.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git stash\

> Saved working directory and index state WIP on main: cfba84f adding home.html fi
> le

touch team.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git add team.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ code team.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git stash
Saved working directory and index state WIP on main: cfba84f adding home.html fi
le

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git stash
No local changes to save

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
(use "git push" to publish your local commits)

Untracked files:
(use "git add <file>..." to include in what will be committed)
about.html

nothing added to commit but untracked files present (use "git add" to track)

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git stash
No local changes to save

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
(use "git push" to publish your local commits)

Untracked files:
(use "git add <file>..." to include in what will be committed)
about.html
team.html

nothing added to commit but untracked files present (use "git add" to track)

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git stash
No local changes to save

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git add team.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git stash
Saved working directory and index state WIP on main: cfba84f adding home.html fi
le

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git stash apply stash@{0}
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
(use "git push" to publish your local commits)

Changes to be committed:
(use "git restore --staged <file>..." to unstage)
new file: team.html

Untracked files:
(use "git add <file>..." to include in what will be committed)
about.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
(use "git push" to publish your local commits)

Changes to be committed:
(use "git restore --staged <file>..." to unstage)
new file: team.html

Untracked files:
(use "git add <file>..." to include in what will be committed)
about.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git stash pop stash@{1}
Auto-merging team.html
CONFLICT (add/add): Merge conflict in team.html
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
(use "git push" to publish your local commits)

Changes to be committed:
(use "git restore --staged <file>..." to unstage)
modified: README.md

Unmerged paths:
(use "git restore --staged <file>..." to unstage)
(use "git add <file>..." to mark resolution)
both added: team.html

Untracked files:
(use "git add <file>..." to include in what will be committed)
about.html

The stash entry is kept in case you need it again.

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git add home.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ status
bash: status: command not found

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
(use "git push" to publish your local commits)

Changes to be committed:
(use "git restore --staged <file>..." to unstage)
modified: README.md

Unmerged paths:
(use "git restore --staged <file>..." to unstage)
(use "git add <file>..." to mark resolution)
both added: team.html

Untracked files:
(use "git add <file>..." to include in what will be committed)
about.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git reset
Unstaged changes after reset:
M README.md

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git commit -a -m "commiting all new file"
[main 8d9a43d] commiting all new file
1 file changed, 74 insertions(+)

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status\

> On branch main
> Your branch is ahead of 'origin/main' by 3 commits.
> (use "git push" to publish your local commits)

Untracked files:
(use "git add <file>..." to include in what will be committed)
about.html
team.html

nothing added to commit but untracked files present (use "git add" to track)

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git add about.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
(use "git push" to publish your local commits)

Changes to be committed:
(use "git restore --staged <file>..." to unstage)
new file: about.html

Untracked files:
(use "git add <file>..." to include in what will be committed)
team.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git commit -m "new file"
[main 7faffea] new file
1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 about.htm
...

#Bundle two

##Exercise 1

...bash
jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git branch ft/bundle-2
jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ touch services.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git add services.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git commit -m "adding new page"
[main 5136c5b] adding new page
1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 services.html
jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ code services.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git add services.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git commit -m "make some changes in services.html file"
[main 4b5775e] make some changes in services.html file
1 file changed, 15 insertions(+)

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git checkout ft/bundle-2

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/bundle-2)
$ touch services.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/bundle-2)
$ git add services.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/bundle-2)
$ git commit -m "adding new file"
[ft/bundle-2 998b23d] adding new file
1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 services.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/bundle-2)
$ code services.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/bundle-2)
$ git add services.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/bundle-2)
$ git commit -m "make some update in this file"
[ft/bundle-2 a23cde6] make some update in this file
1 file changed, 11 insertions(+)

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/bundle-2)
$ git add README.md

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/bundle-2)
$ git commit -m "added new content to this file"
[ft/bundle-2 3d584ea] added new content to this file
1 file changed, 55 insertions(+)

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/bundle-2)
$ git remote add https://github.com/Jameszammy/Gym-Git-Exercise-Solutions
usage: git remote add [<options>] <name> <url>

    -f, --[no-]fetch      fetch the remote branches
    --[no-]tags           import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --[no-]track <branch>
                          branch(es) to track
    -m, --[no-]master <branch>
                          master branch
    --[no-]mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/bundle-2)
$ git push -u origin ft/bundle-2
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 4 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 1.29 KiB | 147.00 KiB/s, done.
Total 8 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote: https://github.com/Jameszammy/Gym-Git-Exercise-Solutions/pull/new/f
t/bundle-2
remote:
To https://github.com/Jameszammy/Gym-Git-Exercise-Solutions.git

- [new branch] ft/bundle-2 -> ft/bundle-2
  branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
  ...

#Bundle two
##Exercise 2

...bash
jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
(use "git push" to publish your local commits)

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git pull origin main
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 892 bytes | 111.00 KiB/s, done.
From https://github.com/Jameszammy/Gym-Git-Exercise-Solutions

- branch main -> FETCH_HEAD
  f8078db..9a9c0f1 main -> origin/main
  Auto-merging services.html
  CONFLICT (add/add): Merge conflict in services.html
  Automatic merge failed; fix conflicts and then commit the result.
jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 321 bytes | 321.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Jameszammy/Gym-Git-Exercise-Solutions/pull/new/f
t/service-redesign
remote:
To https://github.com/Jameszammy/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

...
