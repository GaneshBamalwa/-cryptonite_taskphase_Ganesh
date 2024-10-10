# CTF Challenge: duplicating_piped_data_with_tee

## Table of Content

- commands-executed: /challenge/pwn | tee output | /challenge/college , cat output , /challenge/pwn  --secret AqhGjH-V | /challenge/college
- flag :pwn.college{AqhGjH-VmPjEuqpjxHKXRAUhDhy.dFjM5QDLzETN0czW}  



### Objective:
  When you pipe data from one command to another, you of course no longer see it on your screen. This is not always desired: for example, you might want to see the data as it flows through between your commands to debug unintended outcomes (e.g., "why did that second command not work???").

Luckily, there is a solution! The tee command, named after a "T-splitter" from plumbing pipes, duplicates data flowing through your pipes to any number of files provided on the command line. For example:

hacker@dojo:~$ echo hi | tee pwn college
hi
hacker@dojo:~$ cat pwn
hi
hacker@dojo:~$ cat college
hi
hacker@dojo:~$
As you can see, by providing two files to tee, we ended up with three copies of the piped-in data: one to stdout, one to the pwn file, and one to the college file. You can imagine how you might use this to debug things going haywire:

hacker@dojo:~$ command_1 | command_2
Command 2 failed!
hacker@dojo:~$ command_1 | tee cmd1_output | command_2
Command 2 failed!
hacker@dojo:~$ cat cmd1_output
Command 1 failed: must pass --succeed!
hacker@dojo:~$ command_1 --succeed | command_2
Commands succeeded!
Now, you try it! This process' /challenge/pwn must be piped into /challenge/college, but you'll need to intercept the data to see what pwn needs from you!

### Output:
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

