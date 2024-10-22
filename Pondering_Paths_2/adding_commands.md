# CTF Challenge: adding_commands

## Table of Content

- commands-executed: nano win , export PATH="/home/hacker/:$PATH" , /challenge/run
- flag :pwn.college{M-Nwz6EUkc4Mgblz6OB8E6LJzln.dZzNyUDLzETN0czW}


### Output:
```console
hacker@path~adding-commands:~$ nano win.sh
hacker@path~adding-commands:~$ chmod +x win.sh
hacker@path~adding-commands:~$ ./win.sh
cat: /flag: Permission denied
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
/challenge/run: line 4: win: command not found
It looks like that did not work... Did you set PATH correctly?
hacker@path~adding-commands:~$ echo $PATH
/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~adding-commands:~$ export PATH="/home/hacker/win.sh:$PATH"
hacker@path~adding-commands:~$ echo $PATH
/home/hacker/win.sh:/run/challenge/bin:/run/workspace/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
hacker@path~adding-commands:~$ /challenge/run 
Invoking 'win'....
/challenge/run: line 4: win: command not found
It looks like that did not work... Did you set PATH correctly?
hacker@path~adding-commands:~$ export PATH="/home/hacker/win:$PATH"
hacker@path~adding-commands:~$ /challenge/run 
Invoking 'win'....
/challenge/run: line 4: win: command not found
It looks like that did not work... Did you set PATH correctly?
hacker@path~adding-commands:~$ export PATH="/home/hacker/:$PATH"
hacker@path~adding-commands:~$ /challenge/run 
Invoking 'win'....
/challenge/run: line 4: win: command not found
It looks like that did not work... Did you set PATH correctly?
hacker@path~adding-commands:~$ nano win
hacker@path~adding-commands:~$ chmod +x win
hacker@path~adding-commands:~$ bash win
cat: /flag: Permission denied
hacker@path~adding-commands:~$ /challenge/run 
Invoking 'win'....
pwn.college{M-Nwz6EUkc4Mgblz6OB8E6LJzln.dZzNyUDLzETN0czW}
```
