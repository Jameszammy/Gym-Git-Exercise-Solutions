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
$ git push -u origin main
To https://github.com/Jameszammy/Gym-Git-Exercise-Solutions.git
! [rejected] main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Jameszammy/Gym-Git-
se-Solutions.git'
hint: Updates were rejected because the remote contains work that you do n
hint: have locally. This is usually caused by another repository pushing t
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ ^C

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
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (8/8), 948 bytes | 474.00 KiB/s, done.
Total 8 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Jameszammy/Gym-Git-Exercise-Solutions.git
447cc50..19b5086 main -> main
branch 'main' set up to track 'origin/main'.

% bundle one: exercise 2

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
