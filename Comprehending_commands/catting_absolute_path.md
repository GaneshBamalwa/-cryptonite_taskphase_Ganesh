# CTF Challenge: Catting Absolute Paths

## Table of Content


- commands-executed: ls , cat flag ,cd flag
- flag :pwn.college{4-SxuGpQfhiDbbQzS8AFG8qXQlU.dFzN1QDLzETN0czW}



### Output:
```console
lshacker@commands~catting-absolute-paths:~/flag$ ls
apache2         firefox-restart-required  mount            shm      utmp
challenge       flag                      mysqld           sudo     workspace
current-system  lock                      screen           systemd
dojo            log                       sendsigs.omit.d  user
hacker@commands~catting-absolute-paths:~/flag$ cat flagh
cat: flagh: No such file or directory
hacker@commands~catting-absolute-paths:~/flag$ cat flag
pwn.college{4-SxuGpQfhiDbbQzS8AFG8qXQlU.dFzN1QDLzETN0czW}
hacker@commands~catting-absolute-paths:~/flag$ 
```




