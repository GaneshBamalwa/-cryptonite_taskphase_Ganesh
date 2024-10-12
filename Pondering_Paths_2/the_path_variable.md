# CTF Challenge: the_path_variable

## Table of Content

- commands-executed: cd /challenge/, PATH="" , ./run
- flag :pwn.college{wyxJSjohdHI3GfewOsJLg41BrZX.dZzNwUDLzETN0czW}


### Output:

hacker@path~the-path-variable:~$ cd ../../
hacker@path~the-path-variable:/$ cd /challenge/
hacker@path~the-path-variable:/challenge$ 
hacker@path~the-path-variable:/challenge$ ls
DESCRIPTION.md  run
hacker@path~the-path-variable:/challenge$ PATH=""
hacker@path~the-path-variable:/challenge$ ./run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{wyxJSjohdHI3GfewOsJLg41BrZX.dZzNwUDLzETN0czW}
