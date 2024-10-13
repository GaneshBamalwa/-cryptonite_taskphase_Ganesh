# CTF Challenge: reading_manuals

## Table of Content

- commands-executed: /challenge/challenge --owtyse 014 ,  man challenge
- flag :pwn.college{IJowt014CyXG3Dse2bVnk76xPNr.dRTM4QDLzETN0czW}



### Objective:


### Output:
hacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)                  Challenge Commands                  CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --owtyse NUM
              print the flag if NUM is 014

AUTHOR
       Written by Zardus.
hacker@man~reading-manuals:~$ /challenge/challenge --owtyse NUM
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ /challenge/challenge --owtyse 014
Correct usage! Your flag: pwn.college{IJowt014CyXG3Dse2bVnk76xPNr.dRTM4QDLzETN0czW}
