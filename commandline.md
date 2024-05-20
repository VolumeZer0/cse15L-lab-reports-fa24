![image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/assets/71284679/89e0bc73-8572-43ce-a694-ca4bd79499f9)# CSE 15L LAB REPORTS SPRING 24

---
## Week 7
---
 
## Step 4 : Log into ieng6

Screen Shot:
![Image](https://raw.githubusercontent.com/VolumeZer0/cse15L-lab-reports-fa24/main/4.png)

Keys Pressed:
```ssh kht002@ieng6.ucsd.edu <enter>``` : To log into ssh server

Explantion:

---

## Step 5 : Clone your fork of the repository from your Github account (using the SSH URL)

Screen Shot:
![Image](https://raw.githubusercontent.com/VolumeZer0/cse15L-lab-reports-fa24/main/5.png)

Keys Pressed:
```Git clone <control><v> yes <enter>``` : to clone the repo from copy and paste and agree to terms

---

## Step 6 : Run the tests, demonstrating that they fail

Screen Shot:
![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/6.png?raw=true)

Keys Pressed:

```ls <enter>``` : to list the directories

```cd lab7 <enter>``` : to go into the "lab7" directory

```bash test.sh <enter>``` : to run the test.sh file

---

## Step 7 : Edit the code file to fix the failing test

Screen Shot:
![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/7.png?raw=true)
![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/7.1.png?raw=true)

Keys Pressed:

```vim test.sh``` : to start the vim enviorment on test.sh

```:set number <enter>``` : to show the line numbers

```:44 <enter>``` : to go to line 44 where the bugged line is

```<L> <L> <L> <L> <L> <X> <I> <2> <esc>``` : to edit the file by going to the right 5 times, deleting the character that the cursor is on, going into insert mode, inserting 2, and then returning to command mode

```:wq <enter> ``` : to save and quit

---

## Step 8 : Run the tests, demonstrating that they now succeed

Screen Shot:
![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/8.png?raw=true)

Keys Pressed:

```<up arrow> <up arrow> <enter>``` :  run the tests 

---

## Step 9: Commit and push the resulting change to your Github account (you can pick any commit message!)

Screen Shot:
![Image](https://github.com/VolumeZer0/cse15L-lab-reports-fa24/blob/main/9.png?raw=true)

Keys Pressed:

```Git status <enter>``` : to check the status of the files
```Git add L <tab> <enter>``` : to auto fill and add the file
```Git commit -m “fixed” <enter>``` : to commit added files
```Git push <enter>``` : to push the committed changes to the repository



