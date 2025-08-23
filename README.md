# Gym-Git-Exercise-Solutions

# boundle 1

# exercise 1

...bash

//creating new folder

mkdir folder name

//change directory

$ cd ProjectGym

//initialazing folder to a git repository

$ git init

//Cheacking if the folder is initialize to git repo

$ ls -a
./ ../ .git/

//Creating new files

$ touch index.html

//Checking status for track,stage, modify and untrack files

$ git status

//Staging a file

$ git add index.html

//Commiting file or files to the repo

$ git commit -m "First commite"

$ git commit -a -m "First commite" for multiple files

//Opening files in code editor

$ code index.html

//Creating New Branch

$ git branch master

$ git checkout -b master to creat and switch to new branch

//To know the your branches created

$ git branch

//To move from branch to branch

$ git switch master
$ git checkout master

// To change branch name to another name

$ git branch -m main master

// To connect to github repo

$ git remote add origin https://github.com/Jameszammy/Gym-Git-Exercise-Sol.git

// To pull for branch the latest changes

$ git pull origin main

Unpacking objects: 100% (6/6), 2.33 KiB | 108.00 KiB/s, done.
From https://github.com/Jameszammy/Gym-Git-Exercise-Solutions

// To push changes to github repo

$ git push -u origin main
...

## Bundle one:

## exercise 2

...bash

// Create new file

$ touch home.html

// Open new file with code editor

$ code home.html

// Staged new file

$ git add home.html

// Commiting or sending to git repo

$ git commit -m "adding home.html

// Staging multiple files
$ git add README.md home.html

// To hide your current working directory if you don't stage or commit.

$ git stash

// check for stage, mmodify and unstage

$ git status

// Created new page

$ touch about.html

// Stage new file
$ git add about.html

//Open with code editor

$ code about.html

// stash new file for later use

$ git stash

// Created new file

touch team.html

//Stage new file

$ git add team.html

// Open with code editor

$ code team.html

// Inde new file for later use

$ git stash

// To bring the 1st stage file back to the working directory

$ git stash apply stash@{0}

// To bring the second stash file to working directory and remove it.

$ git stash pop stash@{1}

// Add to stage after editing

$ git add home.html

//This undoes your last commit but keeps the changes staged—perfect if you want to tweak your commit message or add more files.

$ git reset --soft HEAD-1
Unstaged changes after reset:
M README.md

// To commit all files in the stage to git repo

$ git commit -a -m "commiting all new file"

// staged file after changes

$ git add about.html

// Commit stage file to git repo

$ git commit -m "new file"

...

# Bundle two

## Exercise 1

...bash

// Create new branch

$ git branch ft/bundle-2

// Creating new file

$ touch services.html

// Stage new file

$ git add services.html

// Adding to git repo

$ git commit -m "adding new page"

// Open file with code editor

$ code services.html

// Stage changes

$ git add services.html

// add changes to repo
$ git commit -m "make

// Switching to another branch

$ git checkout ft/bundle-2

// Creating file

$ touch services.html

// Staging file

$ git add services.html

// Adding to repo

$ git commit -m

// Opening with code editor

$ code services.html

// Staging changes

$ git add services.html

// Adding changes to repo

$ git commit -m

// Staging file

$ git add README.md

// Adding to repo

$ git commit -m

// Connecting with github repo

$ git remote add https://github.com/Jameszammy/Gym-Git-Exercise-Solutions

// Pushing to github repo

$ git push -u origin ft/bundle-2

// Creating a pull request

remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote: https://github.com/Jameszammy/Gym-Git-Exercise-Solutions/pull/new/f
t/bundle-2
remote:
To https://github.com/Jameszammy/Gym-Git-Exercise-Solutions.git

...

# Bundle two

## Exercise 2

...bash

// Switching to main branch

$ git checkout main

// pulling from main branch

$ git pull origin main

Unpacking objects: 100% (1/1), 892 bytes | 111.00 KiB/s, done.
From https://github.com/Jameszammy/Gym-Git-Exercise-Solutions

// Creating new branch

$ git branch ft/service-redesign

// See status

$ git status

// Staging multiple files

$ git add services.html README.md

// Adding multiple files to git repo

$ git commit -a -m "Updated both files with new contents"

// Connecting with github repo

$ git remote add https://github.com/Jameszammy/Gym-Git-Exercise-Solutions

j// Pushing to github repo

$ git push -u origin main

To https://github.com/Jameszammy/Gym-Git-Exercise-Solutions.git

...

# Bundle Three

## Exercise 1

...bash

// Creating new branch

$ git checkout -b ft/team

// Creating new file

$ touch team.html

// Opening with code editor

$ code team.html

// Staging file

$ git add team.html

// Adding to git repo

$ git commit -m "updating file"

// Connecting with github repo

$ git remote add https://github.com/Jameszammy/Gym-Git-Exercise-Solutions

// Pushing to github

$ git push -u origin ft/team

// Changing to main branch

$ git checkout main

// Creating a new branch

$ git checkout -b ft/contact-page

// Switching branch

$ git checkout ft/team

// Checking last commit

$ git log --oneline -1

// Switching branch

$ git checkout ft/contact-page

// To get changes from last commit on ft/team branch

$ git cherry-pick 99a862f

//Connecting to github repo

$ git remote add https://github.com/Jameszammy/Gym-Git-Exercise-Solutions

//pushing changes to github repo

$ git push -u ft/contact-page

// Creating new branch and switching to it

$ git checkout -b ft/faq-page

// Creating new file

$ touch faq.html

// Staging the new file

$ git add faq.html

// Opening file with code editor

$ code faq.html

// Staging changes in file

$ git add faq.html

// Adding file changes to git repo

$ git commit -m "Adding new file"

// Connecting to github repo

$ git remote add https://github.com/Jameszammy/Gym-Git-Exercise-Solutions

// Pushing changes to github repo

$ git push -u origin ft/faq-page

// Switching to another branch

$ git checkout ft/team

// Reverting last commit using the last commit hash to change last commit message

$ git revert 99a862f

// Pushing the changes to github repo

$ git push origin ft/team

...

# Bundle Three

## Exercise 2

...bash

//Switch to another branch

$ git checkout ft/faq-page

// Creating new branch from another branch

$ git checkout -b ft/home-page-redesign

//Going back to main branch

$ git checkout main

...
