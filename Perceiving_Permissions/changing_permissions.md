# CTF Challenge: changing_permissions

## Table of Content

- commands-executed: chmod u+r /flag , cat /flag , chmod go+rwx /flag , ls -l /flag
- flag :pwn.college{g6iE9W3Cgh0GBZcGf_kyDEfbTiw.dNzNyUDLzETN0czW}


### Output:
```console
hacker@permissions~changing-permissions:~$ chmod u+r /flag
hacker@permissions~changing-permissions:~$ cat /flag
cat: /flag: Permission denied
hacker@permissions~changing-permissions:~$ ls -l /flag
-r-------- 1 root root 58 Oct 12 11:00 /flag
hacker@permissions~changing-permissions:~$ chmod go+rwx /flag
hacker@permissions~changing-permissions:~$ ls -l /flag
-r--rwxrwx 1 root root 58 Oct 12 11:00 /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{g6iE9W3Cgh0GBZcGf_kyDEfbTiw.dNzNyUDLzETN0czW}
```

