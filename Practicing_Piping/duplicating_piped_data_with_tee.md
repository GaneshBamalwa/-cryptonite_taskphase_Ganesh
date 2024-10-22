# CTF Challenge: duplicating_piped_data_with_tee

## Table of Content

- commands-executed: /challenge/pwn | tee output | /challenge/college , cat output , /challenge/pwn  --secret AqhGjH-V | /challenge/college
- flag :pwn.college{AqhGjH-VmPjEuqpjxHKXRAUhDhy.dFjM5QDLzETN0czW}  



### Output:
```console
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee output | /challenge/college 
Processing...
WARNING: you are overwriting file output with tee's output...
The input to 'college' does not contain the correct secret code! This code 
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the 
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat output 
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "AqhGjH-V"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret AqhGjH-V | /challenge/college 
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{AqhGjH-VmPjEuqpjxHKXRAUhDhy.dFjM5QDLzETN0czW}

```
