# CTF Challenge: executable_shell_scripts

## Table of Content

- commands-executed: nano script.sh , chmod +x script.sh , ./script.sh
- flag :pwn.college{QOXkVPH5-46Et-AG-iWdUqtVnem.dRzNyUDLzETN0czW}


### Output:
```console
hacker@chaining~executable-shell-scripts:~$ nano script.sh
hacker@chaining~executable-shell-scripts:~$ ls
1        a           flag          leap          output     x.sh
COLLEGE  actualfile  flag1         myflag        run.sh
Desktop  college     instructions  not-the-flag  script.sh
PWN      f           intructions   not-the-flah  the-flag
hacker@chaining~executable-shell-scripts:~$ ./script.sh
bash: ./script.sh: Permission denied
hacker@chaining~executable-shell-scripts:~$ sudo ./script.sh
sudo: workspace is not privileged
hacker@chaining~executable-shell-scripts:~$ chmod +x script.sh 
hacker@chaining~executable-shell-scripts:~$ ./script.sh 
Congratulations on your shell script execution! Your flag:
pwn.college{QOXkVPH5-46Et-AG-iWdUqtVnem.dRzNyUDLzETN0czW}
```
