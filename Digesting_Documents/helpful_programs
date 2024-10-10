# CTF Challenge: helpful_programs

## Table of Content

- commands-executed: cd ../../ , ./challenge --help , ./challenge -p , ./challenge -g 87
- flag :pwn.college{0kYROjX8pg7_yVkXcjy7IvbVQ9e.ddjM4QDLzETN0czW}

### Objective:
Some programs don't have a man page, but might tell you how to run them if invoked with a special argument. Usually, this argument is --help, but it can often be -h or, in rare cases, -?, help, or other esoteric values like /? (though that latter is more frequently encountered on Windows).

In this level, you will practice reading a program's documentation with --help. Try it out!

### Output:
hacker@man~helpful-programs:~$ cd ../../
hacker@man~helpful-programs:/$ ls
bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr
boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var
hacker@man~helpful-programs:/$ cd /challenge/
hacker@man~helpful-programs:/challenge$ ls
DESCRIPTION.md  challenge
hacker@man~helpful-programs:/challenge$ challenge --help
bash: challenge: command not found
hacker@man~helpful-programs:/challenge$ ./challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v]
                                            [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give
                        you the flag
hacker@man~helpful-programs:/challenge$ ./challenge -g -p 
You passed -p as an argument to -g! Please read the usage
carefully: -g takes *its own* numerical argument.
hacker@man~helpful-programs:/challenge$ ./challenge -p
The secret value is: 87
hacker@man~helpful-programs:/challenge$ ./challenge -g 87
Correct usage! Your flag: pwn.college{0kYROjX8pg7_yVkXcjy7IvbVQ9e.ddjM4QDLzETN0czW}
