# CTF Challenge: Listing Files

## Table of Content

- commands-executed: cd ../ , cd challenge , ls , ./21022-renamed-run-24068
- flag :pwn.college{4PZsCuczDm67i214ws1z4ObaYFi.dhjM4QDLzETN0czW}



### Objective:
So far, we've told you which files to interact with. But directories can have lots of files (and other directories) inside them, and we won't always be here to tell you their names. You'll need to learn to list their contents using the ls command!

ls will list files in all the directories provided to it as arguments, and in the current directory if no arguments are provided. Observe:

hacker@dojo:~$ ls /challenge
run
hacker@dojo:~$ ls
Desktop    Downloads  Pictures  Templates
Documents  Music      Public    Videos
hacker@dojo:~$ ls /home/hacker
Desktop    Downloads  Pictures  Templates
Documents  Music      Public    Videos
hacker@dojo:~$
In this challenge, we've named /challenge/run with some random name! List the files in /challenge to find it.

### Output:
hacker@commands~listing-files:~$ ls
Desktop  a  actualfile  f  flag  flag1  leap  not-the-flag
hacker@commands~listing-files:~$ cd ../
hacker@commands~listing-files:/home$ cd ../
hacker@commands~listing-files:/$ ls
bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@commands~listing-files:/$ cd challenge/
hacker@commands~listing-files:/challenge$ ls
21022-renamed-run-24068  DESCRIPTION.md
hacker@commands~listing-files:/challenge$ ./21022-renamed-run-24068
Yahaha, you found me! Here is your flag:
pwn.college{4PZsCuczDm67i214ws1z4ObaYFi.dhjM4QDLzETN0czW}


