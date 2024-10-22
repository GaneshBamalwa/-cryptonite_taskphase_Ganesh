# CTF Challenge: more catting practice

## Table of Content

- commands-executed: cat /usr/share/games/flag
- flag :pwn.college{gaYoO9LSBefeXidDlpze6cF8sUt.dBjM5QDLzETN0czW}



### Output:
```console
You cannot use the 'cd' command in this level, and must retrieve the flag by 
absolute path. Plus, I hid the flag in a different directory! You can find it 
in the file /usr/share/games/flag. Go cat it out **without** cding into that 
directory!
hacker@commands~more-catting-practice:~$ cd /usr/share/games/flag
You used 'cd'! In this level, I don't allow you to change the working directory 
--- you MUST chase pass 'cat' the absolute path of where I put it on the 
filesystem (which is /usr/share/games/flag).
hacker@commands~more-catting-practice:~$ cat /usr/share/games/flag
pwn.college{gaYoO9LSBefeXidDlpze6cF8sUt.dBjM5QDLzETN0czW}
hacker@commands~more-catting-practice:~$ 
```

