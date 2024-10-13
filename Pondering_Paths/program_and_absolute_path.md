# CTF Challenge: Program and absolute path

## Table of Contents

- commands-executed : /challenge/run
- flag : pwn.college{A6jUGK4DjWeAtez3C-cQXgd0bFs.dVDN1QDLzETN0czW}

### Objective:
Let's explore a slightly more complicated path! Except for in the previous level, challenges in pwn.college are in the challenge directory and the challenge directory is, in turn, right in the root directory (/). The path to the challenge the directory is, thus, /challenge. The name of the challenge program in this level is run, and it lives in the /challenge directory. Thus, the path to the run challenge program is /challenge/run.

This challenge again requires you to execute it by invoking its absolute path. You'll want to execute the run file that is in the challenge directory that is, in turn, in the / directory. If you invoke the challenge correctly, it will give you the flag. Good luck!

### Output:
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{A6jUGK4DjWeAtez3C-cQXgd0bFs.dVDN1QDLzETN0czW}
hacker@paths~program-and-absolute-paths:~$ 


