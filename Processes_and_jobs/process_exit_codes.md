# CTF Challenge: process_exit_codes

## Table of Content

- commands-executed: /challenge/get-code, echo $?, /challenge/submit-code 149
- flag :pwn.college{osvV3RFN6-f77C_4BbSa5c4GkmH.dljN4UDLzETN0czW}


### Output:
```console
hacker@processes~process-exit-codes:~$ /challenge/get-code 
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
149
hacker@processes~process-exit-codes:~$ /challenge/submit-code 
You must run /challenge/submit-code with the exit code you retrieved from 
/challenge/get-code as the first argument:

Usage: /challenge/submit-code [EXIT_CODE]
hacker@processes~process-exit-codes:~$ /challenge/submit-code 149
CORRECT! Here is your flag:
pwn.college{osvV3RFN6-f77C_4BbSa5c4GkmH.dljN4UDLzETN0czW}
```
