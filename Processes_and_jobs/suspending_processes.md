# CTF Challenge: suspending_processes

## Table of Content

- commands-executed: /challenge/run , ctrl+z 
- flag :pwn.college{UJyN8f8JR7ADNV_bbF-gqDAlpbF.dVDN4QDLzETN0czW}


### Output
hacker@processes~suspending-processes:~$ /challenge/run 
I'll only give you the flag if there's already another copy of me running in 
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         320     298  0 04:48 pts/0    00:00:00 bash /challenge/run
root         322     320  0 04:48 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can 
background me with Ctrl-Z or, if you're not ready to do that for whatever 
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run 
I'll only give you the flag if there's already another copy of me running in 
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         320     298  0 04:48 pts/0    00:00:00 bash /challenge/run
root         337     298  0 04:48 pts/0    00:00:00 bash /challenge/run
root         339     337  0 04:48 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{UJyN8f8JR7ADNV_bbF-gqDAlpbF.dVDN4QDLzETN0czW}
