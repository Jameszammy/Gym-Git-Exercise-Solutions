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

...
