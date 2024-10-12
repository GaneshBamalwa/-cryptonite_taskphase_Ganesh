# CTF Challenge: redirecting_input

## Table of Content

- commands-executed: echo COLLEGE > PWN , /challenge/run < PWN
- flag :pwn.college{8qHz_-4AtowtTDjvRjiL0gBpmiU.dBzN1QDLzETN0czW}



### Objective:
Just like you can redirect output from programs, you can redirect input to programs! This is done using <, as so:

hacker@dojo:~$ echo yo > message
hacker@dojo:~$ cat message
yo
hacker@dojo:~$ rev < message
oy
You can do interesting things with a lot of different programs using input redirection! In this level, we will practice using /challenge/run, which will require you to redirect the PWN file to it and have the PWN file contain the value COLLEGE! To write that value to the PWN file, recall the prior challenge on output redirection from echo!

### Output:
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN 
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read 
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{8qHz_-4AtowtTDjvRjiL0gBpmiU.dBzN1QDLzETN0czW}
