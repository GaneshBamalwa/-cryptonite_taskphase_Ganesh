# CTF Challenge: finding files

## Table of Content

- commands-executed: cd , cat , find -name flag
- flag : pwn.college{kFpca_sMHlI9sxhJ-M06748zgmG.dJzM4QDLzETN0czW}



### Output:
```console

hacker@commands~finding-files:~$ find -name flag
./flag
./flag/flag
hacker@commands~finding-files:~$ cd ../ 
hacker@commands~finding-files:/home$ cd ../
hacker@commands~finding-files:/$ find -name flag
find: ‘./root’: Permission denied
find: ‘./proc/1/task/1/fd’: Permission denied
find: ‘./proc/1/task/1/fdinfo’: Permission denied
find: ‘./proc/1/task/1/ns’: Permission denied
find: ‘./proc/1/fd’: Permission denied
find: ‘./proc/1/map_files’: Permission denied
find: ‘./proc/1/fdinfo’: Permission denied
find: ‘./proc/1/ns’: Permission denied
find: ‘./proc/7/task/7/fd’: Permission denied
find: ‘./proc/7/task/7/fdinfo’: Permission denied
find: ‘./proc/7/task/7/ns’: Permission denied
find: ‘./proc/7/fd’: Permission denied
find: ‘./proc/7/map_files’: Permission denied
find: ‘./proc/7/fdinfo’: Permission denied
find: ‘./proc/7/ns’: Permission denied
find: ‘./proc/132/task/132/fd’: Permission denied
find: ‘./proc/132/task/132/fdinfo’: Permission denied
find: ‘./proc/132/task/132/ns’: Permission denied
find: ‘./proc/132/fd’: Permission denied
find: ‘./proc/132/map_files’: Permission denied
find: ‘./proc/132/fdinfo’: Permission denied
find: ‘./proc/132/ns’: Permission denied
./home/hacker/flag
./home/hacker/flag/flag
find: ‘./var/log/private’: Permission denied
find: ‘./var/log/apache2’: Permission denied
find: ‘./var/log/mysql’: Permission denied
find: ‘./var/cache/ldconfig’: Permission denied
find: ‘./var/cache/apt/archives/partial’: Permission denied
find: ‘./var/cache/private’: Permission denied
find: ‘./var/lib/apt/lists/partial’: Permission denied
find: ‘./var/lib/php/sessions’: Permission denied
find: ‘./var/lib/mysql-files’: Permission denied
find: ‘./var/lib/private’: Permission denied
find: ‘./var/lib/mysql-keyring’: Permission denied
find: ‘./var/lib/mysql’: Permission denied
find: ‘./tmp/tmp.XvrUsDZh8M’: Permission denied
find: ‘./run/mysqld’: Permission denied
find: ‘./run/sudo’: Permission denied
find: ‘./etc/ssl/private’: Permission denied
./usr/local/lib/python3.8/dist-packages/pwnlib/flag
./usr/local/share/radare2/5.9.5/flag
./opt/busybox/busybox-1.33.2/include/config/hush/mode/flag
./opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/flag
./opt/radare2/libr/flag
./nix/store/pmvk2bk4p550w182rjfm529kfqddnvh3-python3.11-pwntools-4.12.0/lib/python3.11/site-packages/pwnlib/flag
./nix/store/1yagn5s8sf7kcs2hkccgf8d0wxlrv5sz-radare2-5.9.0/share/radare2/5.9.0/flag
hacker@commands~finding-files:/$ cat ./nix/store/1yagn5s8sf7kcs2hkccgf8d0wxlrv5sz-radare2-5.9.0/share/radare2/5.9.0/flag
cat: ./nix/store/1yagn5s8sf7kcs2hkccgf8d0wxlrv5sz-radare2-5.9.0/share/radare2/5.9.0/flag: Is a directory
hacker@commands~finding-files:/$ cd ./nix/store/1yagn5s8sf7kcs2hkccgf8d0wxlrv5sz-radare2-5.9.0/share/radare2/5.9.0/flag
hacker@commands~finding-files:/nix/store/1yagn5s8sf7kcs2hkccgf8d0wxlrv5sz-radare2-5.9.0/share/radare2/5.9.0/flag$ ls
tags.r2
hacker@commands~finding-files:/nix/store/1yagn5s8sf7kcs2hkccgf8d0wxlrv5sz-radare2-5.9.0/share/radare2/5.9.0/flag$ cd /
hacker@commands~finding-files:/$ cd ./nix/store/pmvk2bk4p550w182rjfm529kfqddnvh3-python3.11-pwntools-4.12.0/lib/python3.11/site-packages/pwnlib/flag
hacker@commands~finding-files:/nix/store/pmvk2bk4p550w182rjfm529kfqddnvh3-python3.11-pwntools-4.12.0/lib/python3.11/site-packages/pwnlib/flag$ 
hacker@commands~finding-files:/nix/store/pmvk2bk4p550w182rjfm529kfqddnvh3-python3.11-pwntools-4.12.0/lib/python3.11/site-packages/pwnlib/flag$ ls
__init__.py  __pycache__  flag.py
hacker@commands~finding-files:/nix/store/pmvk2bk4p550w182rjfm529kfqddnvh3-python3.11-pwntools-4.12.0/lib/python3.11/site-packages/pwnlib/flag$ python flag.py
hacker@commands~finding-files:/nix/store/pmvk2bk4p550w182rjfm529kfqddnvh3-python3.11-pwntools-4.12.0/lib/python3.11/site-packages/pwnlib/flag$ cd /
hacker@commands~finding-files:/$ cd ./opt/radare2/libr/flag
hacker@commands~finding-files:/opt/radare2/libr/flag$ ls
Makefile  flag.c  flag.o        meson.build  tags.d  zones.c  zones.o
d         flag.d  libr_flag.so  tags.c       tags.o  zones.d
hacker@commands~finding-files:/opt/radare2/libr/flag$ cd /
hacker@commands~finding-files:/$ cd ./opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/flag
hacker@commands~finding-files:/opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/flag$ ls
__init__.py  __pycache__  flag.py
hacker@commands~finding-files:/opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/flag$ python3 flag.py
hacker@commands~finding-files:/opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/flag$ cd /
hacker@commands~finding-files:/$ cd ./opt/busybox/busybox-1.33.2/include/config/hush/mode/flag
bash: cd: ./opt/busybox/busybox-1.33.2/include/config/hush/mode/flag: Not a directory
hacker@commands~finding-files:/$ cat ./opt/busybox/busybox-1.33.2/include/config/hush/mode/flag
pwn.college{kFpca_sMHlI9sxhJ-M06748zgmG.dJzM4QDLzETN0czW}
```
