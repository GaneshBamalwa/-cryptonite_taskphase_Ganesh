# CTF Challenge: Position Yet Elsewhere

## Table of Contents

- commands-executed: /challenge/run,  cd proc/346/fd , /challenge/run
- flag :pwn.college{cDcF1mSjmUJgIeWaCVjUgUY2eiF.dhDN1QDLzETN0czW}

### Objective:
The Linux filesystem has tons of directories with tons of files. You can navigate around directories by using the cd (change directory) command and passing a path to it as an argument, as so:

hacker@dojo:~$ cd /some/new/directory
hacker@dojo:/some/new/directory$ cd /some/new/directory
This affects the "current working directory" of your process (in this case, the bash shell). Each process has a directory in which it's currently hanging out. The reasons for this will become clear later in the module.

As an aside, now you can see what the ~ was in the prompt! It shows the current that your shell is located at.

This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program. Good luck!

### Output:
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



