# CTF Challenge: cat not pet , but command

## Table of Content

- commands-executed: ls , cd flag , cat flag
- flag :pwn.college{4-SxuGpQfhiDbbQzS8AFG8qXQlU.dFzN1QDLzETN0czW}



### Objective:

One of the most critical Linux commands is cat. cat is most often used for reading out files, like so:

hacker@dojo:~$ cat /challenge/DESCRIPTION.md
One of the most critical Linux commands is `cat`.
`cat` is most often used for reading out files, like so:
cat will concatenate (hence the name) multiple files if provided multiple arguments. For example:

hacker@dojo:~$ cat myfile
This is my file!
hacker@dojo:~$ cat yourfile
This is your file!
hacker@dojo:~$ cat myfile yourfile
This is my file!
This is your file!
hacker@dojo:~$ cat myfile yourfile myfile
This is my file!
This is your file!
This is my file!
Finally, if you give no arguments at all, cat will read from the terminal input and output it. We'll explore that in later challenges...

In this challenge, I will copy the flag to the flag file in your home directory (where your shell starts). Go read it with cat!


### Output:
hacker@commands~cat-not-the-pet-but-the-command:~$ ls
hacker@commands~cat-not-the-pet-but-the-command:~$ cd flag
hacker@commands~cat-not-the-pet-but-the-command:~/flag$ cat flag
pwn.college{4-SxuGpQfhiDbbQzS8AFG8qXQlU.dFzN1QDLzETN0czW}