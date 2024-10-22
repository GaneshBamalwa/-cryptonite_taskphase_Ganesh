# CTF Challenge:help_for_builtins

## Table of Content

- commands-executed: help challenge , challenge --secret A6nG14qo
- flag :pwn.college{A6nG14qopwxNgU8c103qEec3-sE.dRTM5QDLzETN0czW}



### Output:
```console
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!
    
    Options:
      --fortune		display a fortune
      --version		display the version
      --secret VALUE	prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "A6nG14qo".
hacker@man~help-for-builtins:~$ challenge --secret A6nG14qo
Correct! Here is your flag!
pwn.college{A6nG14qopwxNgU8c103qEec3-sE.dRTM5QDLzETN0czW}
```
