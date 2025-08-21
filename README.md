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
./  ../  .git/

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
        new file:   index.html


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
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git add index.html

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   index.html


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
* main

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git branch -m main master

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (master)
$ git branch
* master

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (master)
$ git branch -m master main

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$ git branch
* main

jzamm@DESKTOP-96E9C5V MINGW64 ~/ProjectGym (main)
$

...
