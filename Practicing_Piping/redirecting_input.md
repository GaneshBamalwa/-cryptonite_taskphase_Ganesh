# CTF Challenge: redirecting_input

## Table of Content

- commands-executed: echo COLLEGE > PWN , /challenge/run < PWN
- flag :pwn.college{8qHz_-4AtowtTDjvRjiL0gBpmiU.dBzN1QDLzETN0czW}


### Output:
```console
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN 
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read 
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{8qHz_-4AtowtTDjvRjiL0gBpmiU.dBzN1QDLzETN0czW}
```
