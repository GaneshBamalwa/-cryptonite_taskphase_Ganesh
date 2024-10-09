# CTF Challenge: Hidden Files

## Table of Content

- commands-executed: cd ../ , ls -a , cat .flag-243191644928680
- flag :pwn.college{QasznEBa7dja1KGu78zqMSXZIOG.dBTN4QDLzETN0czW}



### Objective:

Interestingly, ls doesn't list all the files by default. Linux has a convention where files that start with a . don't show up by default in ls and in a few other contexts. To view them with ls, you need to invoke ls with the -a flag, as so:

hacker@dojo:~$ touch pwn
hacker@dojo:~$ touch .college
hacker@dojo:~$ ls
pwn
hacker@dojo:~$ ls -a
.college	pwn
hacker@dojo:~$
Now, it's your turn! Go find the flag, hidden as a dot-prepended file in /.

### Output:
hacker@commands~hidden-files:~$ cd ../
hacker@commands~hidden-files:/home$ cd ../
hacker@commands~hidden-files:/$ ls -a
.                      bin        etc    lib64   nix   run   tmp
..                     boot       home   libx32  opt   sbin  usr
.dockerenv             challenge  lib    media   proc  srv   var
.flag-243191644928680  dev        lib32  mnt     root  sys
hacker@commands~hidden-files:/$ ./.flag-243191644928680
bash: ./.flag-243191644928680: Permission denied
hacker@commands~hidden-files:/$ cat .flag-243191644928680
pwn.college{QasznEBa7dja1KGu78zqMSXZIOG.dBTN4QDLzETN0czW}


