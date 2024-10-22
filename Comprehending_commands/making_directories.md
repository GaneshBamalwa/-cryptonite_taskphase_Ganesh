# CTF Challenge: making directories

## Table of Content

- commands-executed: mkdir /tmp/pwn, touch /tmp/pwn/college, /challenge/run
- flag : pwn.college{4BST3rZ_pkV54eNLmbv_5SUhodG.dFzM4QDLzETN0czW}





### Output:
```console
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ touch college
hacker@commands~making-directories:~$ /challenge/run
Uh oh! /tmp/pwn/college does not exist. Please use the 'touch' command to 
create it!
hacker@commands~making-directories:~$ touch /tmp/pwn/college
hacker@commands~making-directories:~$ /challenge/run
Success! Here is your flag:
pwn.college{4BST3rZ_pkV54eNLmbv_5SUhodG.dFzM4QDLzETN0czW}

```
