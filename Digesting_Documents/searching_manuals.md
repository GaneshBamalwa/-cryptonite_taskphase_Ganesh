# CTF Challenge: searching_manuals

## Table of Content

- commands-executed:  man challenge, /challenge/challenge --sj
- flag :pwn.college{c-V_Xm_DxC0ntR_wM6J_VxRxa7l.dVTM4QDLzETN0czW}



### Objective:
You can scroll man pages with the arrow keys (and PgUp/PgDn) and search with /. After searching, you can hit n to go to the next result and N to go to the previous result. Instead of /, you can use ? to search backwards!

Find the option that will give you the flag by reading the challenge man page.

### Output:
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge --xj
Initializing...
Incorrect usage! Please read the challenge man page!
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge --sj
Initializing...
Correct usage! Your flag: pwn.college{c-V_Xm_DxC0ntR_wM6J_VxRxa7l.dVTM4QDLzETN0czW}

