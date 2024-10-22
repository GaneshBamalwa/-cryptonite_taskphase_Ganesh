# CTF Challenge: using_sudo

## Table of Content

- commands-executed: sudo cat /flag
- flag :pwn.college{whXdKssfoQntRoiUJeC8Dx3d47t.dhTN0UDLzETN0czW}


### Output:
```console
hacker@users~using-sudo:~$ ls
1        PWN         college  flag1         leap          not-the-flah
COLLEGE  a           f        instructions  myflag        output
Desktop  actualfile  flag     intructions   not-the-flag  the-flag
hacker@users~using-sudo:~$ ls -a
.              .cache    .profile  actualfile    intructions   the-flag
..             .config   1         college       leap
.ICEauthority  .dbus     COLLEGE   f             myflag
.bash_history  .john     Desktop   flag          not-the-flag
.bash_logout   .lesshst  PWN       flag1         not-the-flah
.bashrc        .local    a         instructions  output
hacker@users~using-sudo:~$ cat /flag
cat: /flag: Permission denied
hacker@users~using-sudo:~$ sudo cat /flag
pwn.college{whXdKssfoQntRoiUJeC8Dx3d47t.dhTN0UDLzETN0czW}
```
