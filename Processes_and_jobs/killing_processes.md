# CTF Challenge: killing_processes

## Table of Content

- commands-executed: ps -ef | grep /challenge/dont_run , kill 73 ,  /challenge/run
- flag :pwn.college{wx6H9G5d_aIL8LmsYD9Ars-NAxJ.dJDN4QDLzETN0czW}


### Output:
```console
hacker@processes~killing-processes:~$ ps -e | grep /challenge/dont_run
hacker@processes~killing-processes:~$ ps -ef | grep /challenge/dont_run
hacker        73      71  0 04:42 ?        00:00:00 /challenge/dont_run
hacker       531     486  0 04:44 pts/0    00:00:00 grep --color=auto /challenge/dont_run
hacker@processes~killing-processes:~$ kill 73
hacker@processes~killing-processes:~$ ps -ef | grep /challenge/dont_run
hacker       561     486  0 04:44 pts/0    00:00:00 grep --color=auto /challenge/dont_run
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{wx6H9G5d_aIL8LmsYD9Ars-NAxJ.dJDN4QDLzETN0czW}
```
