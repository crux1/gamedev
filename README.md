
gamedev
=======

Please, if you have any questions, send me a message. Do not try and commit anything if you are unsure.

DO NOT USE THE GITHUB APP. IF YOU FOLLOW STEP-BY-STEP ON HOW TO COMMIT WE WILL NOT HAVE ANY ERRORS.

AFTER EVERY COMMAND HIT "ENTER"

IF YOU HAVE AN ERROR THAT SAYS THATS NOT A VALID COMMAND, CHECK YOUR SPELLING (it fixes 90% of my problems)


===========================USING GITHUB====================================

first things first, make sure you are using the development branch.


-in git bash navigate to your file you wish to commit/clone to. for example, on my computer its:

cd Documents/gameDev

-you will now see that you are in that directory

if you need to go up a level (back) type:

cd ../

anytime you need to go a little further start the line with 

cd

navigate to the root directory of where you put the game. and type 

 git checkout -b development

 You will see the change on the line above in bash from master to development.

 Only I will edit the master branch. It is where we will put our final build.


 				========cloning=====

Clones a repository into a newly created directory, creates remote-tracking branches for each branch in the cloned repository

in order to clone in git bash navigate to the folder you have set up, and type 

git clone https://github.com/crux1/gamedev.git


That will download the files to your computer


				========commit========

Commiting is when you want to push the new build up to the site

Navigate to the file you want to commit and type

git commit -m "type in the change here, this is where we will see your new changes"

git pull

git push



=======================extra================

if you want to see the files that are in that directory, basically everything you are about to commit type

ls


if you want to see what you have staged type

git status


please, if you make a change, try to commit that one file by navigating to it. No need to keep putting up every file.



========================CREATE SSH KEY IF NEEDED=======================================

Github git bash help---

--Making a public ssh key-
-login to github.com
-click on your username in the top right.
-go to edit profile
-on the side nav, click on SSH keys
-click add SSH KEY

NOW OPEN GIT BASH

first check if you have an existing key
in the git bash type-

 $ls -al ~/.ssh

if you do not have a key type 

$ssh-keygen -t rsa -C "your_email@example.com"

it will ask you where you want to save it. Just hit enter
Then create a password

create a password - hit enter
type password in again - hit enter

It will then tell you identification. Where it is a long string of numbers and colons.

type into git bash-

$ clip < ~/.ssh/id_rsa.pub

That copies your key to clipboard
and now paste the key into your profile on github.com

You now have just made your new key!
