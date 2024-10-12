# CTF Challenge: Becoming_root_with_su

## Table of Content

- commands-executed: su , cd flag , ls , cat flag 
- flag :pwn.college{4-SxuGpQfhiDbbQzS8AFG8qXQlU.dFzN1QDLzETN0czW}


### Output:

hacker@users~becoming-root-with-su:~$ su
Password: 
root@users~becoming-root-with-su:/home/hacker# 
root@users~becoming-root-with-su:/home/hacker# cd flag
root@users~becoming-root-with-su:/home/hacker/flag# ls
apache2         firefox-restart-required  mount            shm      utmp
challenge       flag                      mysqld           sudo     workspace
current-system  lock                      screen           systemd
dojo            log                       sendsigs.omit.d  user
root@users~becoming-root-with-su:/home/hacker/flag# cat flag 
pwn.college{4-SxuGpQfhiDbbQzS8AFG8qXQlU.dFzN1QDLzETN0czW}
