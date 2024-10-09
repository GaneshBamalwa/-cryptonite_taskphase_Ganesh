# CTF Challenge: Catting Absolute Paths

## Table of Content


- commands-executed: ls , cat flag ,cd flag
- flag :pwn.college{4-SxuGpQfhiDbbQzS8AFG8qXQlU.dFzN1QDLzETN0czW}



### Objective:
In the last level, you did cat flag to read the flag out of your home directory! You can, of course, specify cat's arguments as absolute paths:

hacker@dojo:~$ cat /challenge/DESCRIPTION.md
In the last level, you did `cat flag` to read the flag out of your home directory!
You can, of course, specify `cat`'s arguments as absolute paths:
...
In this directory, I will not copy it to your home directory, but I will make it readable. You can read it with cat at its absolute path: /flag.

FUN FACT: /flag is where the flag always lives in pwn.college, but unlike in this challenge, you typically can't access that file directly.

### Output:
lshacker@commands~catting-absolute-paths:~/flag$ ls
apache2         firefox-restart-required  mount            shm      utmp
challenge       flag                      mysqld           sudo     workspace
current-system  lock                      screen           systemd
dojo            log                       sendsigs.omit.d  user
hacker@commands~catting-absolute-paths:~/flag$ cat flagh
cat: flagh: No such file or directory
hacker@commands~catting-absolute-paths:~/flag$ cat flag
pwn.college{4-SxuGpQfhiDbbQzS8AFG8qXQlU.dFzN1QDLzETN0czW}
hacker@commands~catting-absolute-paths:~/flag$ 





