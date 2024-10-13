# CTF Challenge: removing files

## Table of Content

- commands-executed: ls , rm delete_me , /challenge/check
- flag :pwn.college{4MQyHmBrro-TLda3iPxjntuVugv.dZTOwUDLzETN0czW}



### Objective:
Files are all around you. Like candy wrappers, there'll eventually be too many of them. In this level, we'll learn to clean up!

In Linux, you remove files with the rm command, as so:

hacker@dojo:~$ touch PWN
hacker@dojo:~$ touch COLLEGE
hacker@dojo:~$ ls
COLLEGE     PWN
hacker@dojo:~$ rm PWN
hacker@dojo:~$ ls
COLLEGE
hacker@dojo:~$
Let's practice. This challenge will create a delete_me file in your home directory! Delete it, then run /challenge/check, which will make sure you've deleted it and then give you the flag!


### Output:

hacker@commands~removing-files:~$ ls
Desktop  a  actualfile  delete_me  f  flag  flag1  leap  not-the-flag
hacker@commands~removing-files:~$ rm delete_me 
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{4MQyHmBrro-TLda3iPxjntuVugv.dZTOwUDLzETN0czW}

