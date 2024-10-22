# CTF Challenge: Position Yet Elsewhere

## Table of Contents

- commands-executed: /challenge/run,  cd proc/346/fd , /challenge/run
- flag :pwn.college{cDcF1mSjmUJgIeWaCVjUgUY2eiF.dhDN1QDLzETN0czW}



### Output:
```console
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /proc/346/fd directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd proc/346/fd
bash: cd: proc/346/fd: No such file or directory
hacker@paths~position-yet-elsewhere:~$ cd /proc/346/fd
hacker@paths~position-yet-elsewhere:/proc/346/fd$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{cDcF1mSjmUJgIeWaCVjUgUY2eiF.dhDN1QDLzETN0czW}
```


