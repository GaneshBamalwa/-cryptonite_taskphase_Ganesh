# CTF Challenge: Resuming_processes

## Table of Content

- commands-executed: /challenge/run , fg /challenge/run
- flag :pwn.college{wvfil02Ddh5xX0aJ3bdIFbuf8Mp.dZDN4QDLzETN0czW}


### Output:
```console
hacker@processes~resuming-processes:~$ /challenge/run 
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with 
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg /challenge/run 
/challenge/run
I'm back! Here's your flag:
pwn.college{wvfil02Ddh5xX0aJ3bdIFbuf8Mp.dZDN4QDLzETN0czW}
Don't forget to press Enter to quit me!
```
