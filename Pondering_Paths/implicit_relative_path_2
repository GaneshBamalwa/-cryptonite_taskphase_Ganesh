# CTF Challenge: implicit_relative_path

## Table of Contents

- commands-executed: cd ../, cd /challenge , run , ./run
- flag :pwn.college{w2h7r2FiDck4UZnBK_J48rqw9qO.dFTN1QDLzETN0czW}

### Objective:
In this level, we'll practice refering to paths using . a bit more. This challenge will need you to run it from the /challenge directory. Here, things get slightly tricky.

Linux explicitly avoids automatically looking in the current directory when you provide a "naked" path. Consider the following:

hacker@dojo:~$ cd /challenge
hacker@dojo:/challenge$ run
This will not invoke /challenge/run. This is actually a safety measure: if Linux searched the current directory for programs every time you entered a naked path, you could accidentally execute programs in your current directory that happened to have the same names as core system utilities! As a result, the above commands will yield the following error:

bash: run: command not found
We'll explore the mechanisms behind this concept later, but in this challenge, will learn how to explicitly use relative paths to launch run in this scenario. The way to do this is to tell Linux that you explicitly want to execute a program in the current directory, using . like in the previous levels. Give it a try now!



### Output:
hacker@paths~implicit-relative-path:~$ cd ../
hacker@paths~implicit-relative-path:/home$ cd ../
hacker@paths~implicit-relative-path:/$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ run
bash: run: command not found
hacker@paths~implicit-relative-path:/challenge$ ,/run
bash: ,/run: No such file or directory
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{w2h7r2FiDck4UZnBK_J48rqw9qO.dFTN1QDLzETN0czW}


