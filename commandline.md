# CSE 15L LAB REPORTS SPRING 24

---
## Week 7
---
 
## Step 4 : Log into ieng6

Screen Shot:
![Image](https://raw.githubusercontent.com/VolumeZer0/cse15L-lab-reports-fa24/main/4.png)

Keys Pressed:
```ssh<space>kht002@ieng6.ucsd.edu<enter>``` : To log into ssh server

---

## Step 5 : Clone your fork of the repository from your Github account (using the SSH URL)

Screen Shot:
![Image](https://raw.githubusercontent.com/VolumeZer0/cse15L-lab-reports-fa24/main/5.png)

Keys Pressed:
```Git<space>clone<space><control><v><enter>``` : to clone the repo from copy and paste

```yes<enter>``` : to agree to the terms and conditions

---

## Step 6 : Run the tests, demonstrating that they fail

Screen Shot:
![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/6.png?raw=true)

Keys Pressed:

```ls<enter>``` : to list the directories

```cd<space>lab7<enter>``` : to go into the "lab7" directory

```bash<space>test.sh<enter>``` : to run the test.sh file

---

## Step 7 : Edit the code file to fix the failing test

Screen Shot:
![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/7.png?raw=true)
![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/7.1.png?raw=true)

Keys Pressed:

```vim<space>test.sh<enter>``` : to start the vim enviorment on test.sh

```:set<space>number<enter>``` : to show the line numbers

```:44<enter>``` : to go to line 44 where the bugged line is

```LLLLLXI2<esc>``` : to edit the file by going to the right 5 times, deleting the character that the cursor is on, going into insert mode, inserting 2, and then returning to command mode

```:wq<space><enter> ``` : to save and quit

---

## Step 8 : Run the tests, demonstrating that they now succeed

Screen Shot:
![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/8.png?raw=true)

Keys Pressed:

```<up arrow><up arrow><enter>``` :  run the tests fromn the history

---

## Step 9: Commit and push the resulting change to your Github account (you can pick any commit message!)

Screen Shot:
![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/9.png?raw=true)

Keys Pressed:

```git<space>status<enter>``` : to check the status of the files

```git<space>add<space>L<space><tab><enter>``` : to auto fill and add the file

```git<space>commit<space>-m<space>“fixed”<enter>``` : to commit added files

```git<space>push<enter>``` : to push the committed changes to the repository




