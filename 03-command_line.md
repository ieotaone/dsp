# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

*show current working directory path: pwd**
*creating a directory: mkdir <directoryname>**
*deleting a directory: rmdir <directoryname>**
*creating a file using 'touch' command: touch <filename>
*deleting a file: rm <filename>
*renaming a file: mv <filename1> <filename2>
*listing hidden files: ls -a
*copying a file from one directory to another: cp <sourcedir> <enddir>
*listing files by file size: ls -S
*change directory: cd <directory>

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  : list files
`ls -a`  : listing hidden files
`ls -l`  :list files in long format - show permissions
`ls -lh`  : list hidden files in long format with readable file size
`ls -lah`  : list files including hidden files in long format with readable file size
`ls -t`  : list newest files first based on timestamp
`ls -Glp`: lists the detials fo the long format listing,not to display group and displayes the directories with a slash

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

ls -R: lists subdirectories
ls -x: displays files as rows across the screen
ls -1: displays each entry on a line
ls -m: displays the names as a comma separated list
ls -c: displays files by file timestamp

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

xargs - builds and executes command lines from standard input
example: printf "1\n2\n3\n" | xargs touch
ls 
1,2,3
-creates 3 files named 1, 2 and 3
 

