# CTF Challenge: fun_with_group_names

## Table of Content

- commands-executed: id , chgrp grp787 /flag , cat /flag
- flag :pwn.college{ETMqhh99rAWzosLDZmI3U6r43VJ.dJzNyUDLzETN0czW}


### Output:
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp787) groups=1000(grp787)
hacker@permissions~fun-with-groups-names:~$ chgrp grp787 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{ETMqhh99rAWzosLDZmI3U6r43VJ.dJzNyUDLzETN0czW}


