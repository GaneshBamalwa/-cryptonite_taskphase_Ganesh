# CTF Challenge: implicit_relative_path

## Table of Contents

- commands-executed: cd ../, cd /challenge , run , ./run
- flag :pwn.college{w2h7r2FiDck4UZnBK_J48rqw9qO.dFTN1QDLzETN0czW}


### Output:
```console
hacker@paths~implicit-relative-path:~$ cd ../
hacker@paths~implicit-relative-path:/home$ cd ../
hacker@paths~implicit-relative-path:/$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ run
bash: run: command not found
hacker@paths~implicit-relative-path:/challenge$ ,/run
bash: ,/run: No such file or directory
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{w2h7r2FiDck4UZnBK_J48rqw9qO.dFTN1QDLzETN0czW}

```
