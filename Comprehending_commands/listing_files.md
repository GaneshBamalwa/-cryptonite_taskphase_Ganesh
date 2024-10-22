# CTF Challenge: Listing Files

## Table of Content

- commands-executed: cd ../ , cd challenge , ls , ./21022-renamed-run-24068
- flag :pwn.college{4PZsCuczDm67i214ws1z4ObaYFi.dhjM4QDLzETN0czW}




### Output:
```console
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


```
