# CTF Challenge: learning_complex_usage

## Table of Content

- commands-executed: /challenge/challenge --printfile /challenge/DESCRIPTION.md , /challenge/challenge --printfile flag , ls , cd flag
- flag :pwn.college{47yEkawanBlRn63gTDWyqTqYcub.dVjM5QDLzETN0czW}



### Objective:
While using most commands is straightforward, the usage of some commands can get quite complex. For example, the arguments to commands like sed and awk, which we're definitely not getting into right now, are entire programs in an esoteric programming language! Somewhere on the spectrum between cd and awk are commands that take arguments to their arguments...

This sounds crazy, but you've already encountered this with the find level in Basic Commands. find has a -name argument, and the -name argument itself takes an argument specifying the name to search for. Many other commands are analogous.

Here is this level's documentation for /challenge/challenge:

Welcome to the documentation for /challenge/challenge! This program allows you to print arbitrary files to the terminal, when given the --printfile argument. The argument to the --printfile argument is the path of the flag to read. For example, /challenge/challenge --printfile /challenge/DESCRIPTION.md will print out the description of the level!

Given that documentation, go get the flag!


### Output:
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /challenge/DESCRIPTION.md
Correct argument! Here is the /challenge/DESCRIPTION.md file:
While using most commands is straightforward, the usage of some commands can get quite complex.
For example, the arguments to commands like `sed` and `awk`, which we're definitely not getting into right now, are entire programs in an esoteric programming language!
Somewhere on the spectrum between `cd` and `awk` are commands that take arguments to their arguments...

This sounds crazy, but you've already encountered this with the `find` level in [Basic Commands](../commands).
`find` has a `-name` argument, and the `-name` argument itself takes an argument specifying the name to search for.
Many other commands are analogous.

Here is this level's documentation for `/challenge/challenge`:

> Welcome to the documentation for `/challenge/challenge`! This program allows you to print arbitrary files to the terminal, when given the `--printfile` argument. The argument to the `--printfile` argument is the path of the flag to read. For example, `/challenge/challenge --printfile /challenge/DESCRIPTION.md` will print out the description of the level!

Given that documentation, go get the flag!
hacker@man~learning-complex-usage:~$ /challenge/challenge
Incorrect usage! You must pass an argument to me (read the challenge 
description for details).
hacker@man~learning-complex-usage:~$ ls
Desktop  actualfile  f     flag1  not-the-flag
a        college     flag  leap   not-the-flah
hacker@man~learning-complex-usage:~$ cd flag
hacker@man~learning-complex-usage:~/flag$ ls
apache2         firefox-restart-required  mount            shm      utmp
challenge       flag                      mysqld           sudo     workspace
current-system  lock                      screen           systemd
dojo            log                       sendsigs.omit.d  user
hacker@man~learning-complex-usage:~/flag$ /challenge/challenge --printfile flag
Correct argument! Here is the flag file:
pwn.college{47yEkawanBlRn63gTDWyqTqYcub.dVjM5QDLzETN0czW}
