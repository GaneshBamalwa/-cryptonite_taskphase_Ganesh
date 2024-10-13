# CTF Challenge: matching_with_?

## Table of Content

- commands-executed: cd /?ha??enge , /challenge/run
- flag :pwn.college{IXS-l6xMf-Q_RXt51iHREprfrxP.dJjM4QDLzETN0czW}



### Objective:
Next, let's learn about ?. When it encounters a ? character in any argument, the shell will treat it as single-character wildcard. This works like *, but only matches one character. For example:

hacker@dojo:~$ touch file_a
hacker@dojo:~$ touch file_b
hacker@dojo:~$ touch file_cc
hacker@dojo:~$ ls
file_a	file_b	file_cc
hacker@dojo:~$ echo Look: file_?
Look: file_a file_b
hacker@dojo:~$ echo Look: file_??
Look: file_cc
Now, practice this yourself! Starting from your home directory, change your directory to /challenge, but use the ? character instead of c and l in the argument to cd! Once you're there, run /challenge/run for the flag!

### Output:
This challenge resets your working directory to /home/hacker unless you change 
directory properly...
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{IXS-l6xMf-Q_RXt51iHREprfrxP.dJjM4QDLzETN0czW}
