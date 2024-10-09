# CTF Challenge: making directories

## Table of Content

- commands-executed: mkdir /tmp/pwn, touch /tmp/pwn/college, /challenge/run
- flag : pwn.college{4BST3rZ_pkV54eNLmbv_5SUhodG.dFzM4QDLzETN0czW}


### Objective:

We can create files. How about directories? You make directories using the mkdir command. Then you can stick files in there!

Watch:

hacker@dojo:~$ cd /tmp
hacker@dojo:/tmp$ ls
hacker@dojo:/tmp$ ls
hacker@dojo:/tmp$ mkdir my_directory
hacker@dojo:/tmp$ ls
my_directory
hacker@dojo:/tmp$ cd my_directory
hacker@dojo:/tmp/my_directory$ touch my_file
hacker@dojo:/tmp/my_directory$ ls
my_file
hacker@dojo:/tmp/my_directory$ ls /tmp/my_directory/my_file
/tmp/my_directory/my_file
hacker@dojo:/tmp/my_directory$
Now, go forth and create a /tmp/pwn directory and make a college file in it! Then run /challenge/run, which will check your solution and give you the flag!


### Output:
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ touch college
hacker@commands~making-directories:~$ /challenge/run
Uh oh! /tmp/pwn/college does not exist. Please use the 'touch' command to 
create it!
hacker@commands~making-directories:~$ touch /tmp/pwn/college
hacker@commands~making-directories:~$ /challenge/run
Success! Here is your flag:
pwn.college{4BST3rZ_pkV54eNLmbv_5SUhodG.dFzM4QDLzETN0czW}


