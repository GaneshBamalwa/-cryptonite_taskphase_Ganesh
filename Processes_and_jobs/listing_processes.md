# CTF Challenge: Listing Processes 

## Table of Content

- commands-executed: ps -ef
- flag :pwn.college{MqnK_7K9V8KnhbFZJ_B-GWQgYc1.dhzM4QDLzETN0czW}


### Output:
hacker@processes~listing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 04:40 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bin/dojo-init /run/dojo/bin/sleep 6h
root           7       1  0 04:40 ?        00:00:00 /run/dojo/bin/sleep 6h
root          68       1  0 04:40 ?        00:00:00 /challenge/1061-run-10844
root          72      68  0 04:40 ?        00:00:00 sleep 6h
hacker        95       1  1 04:40 ?        00:00:00 /nix/store/g53lqy8w86jkp2g98rz3dd9dpvmvab12-tigervnc-1.13.1/bin/Xvnc :0 -localhost 0 -rfbunixpath 
hacker       100       1  0 04:40 ?        00:00:00 /nix/store/1xhds5s320nfp2022yjah1h7dpv8qqns-bash-5.2p32/bin/bash /nix/store/w3brwhxn0nfn8kh7l8kgi3
hacker       109     100  1 04:40 ?        00:00:00 /nix/store/3wb0055984n2whn449hywsl4ag9gcjir-python3-3.11.9/bin/python3.11 /nix/store/pma5sqhyxm2zq
hacker       119       1  0 04:40 ?        00:00:00 /nix/store/jnz1wdn463qilzhc8nj1kwccshk65pc9-xfce4-session-4.18.3/bin/xfce4-session
hacker       122       1  0 04:40 ?        00:00:00 /nix/store/rvr416z148cjcxh2bmf5anxpsdvmcvrk-dbus-1.14.10/bin/dbus-launch --sh-syntax --exit-with-s
hacker       123       1  0 04:40 ?        00:00:00 /run/current-system/sw/bin/dbus-daemon --syslog --fork --print-pid 5 --print-address 7 --config-fi
hacker       128       1  0 04:40 ?        00:00:00 /nix/store/3zi7zn2bbz3jpx8ds4nharz67j6ajp9k-xfconf-4.18.3/lib/xfce4/xfconf/xfconfd
hacker       137       1  0 04:40 ?        00:00:00 /run/workspace/bin/ssh-agent -s
hacker       139     119  1 04:40 ?        00:00:00 xfwm4
hacker       144     119  0 04:40 ?        00:00:00 xfsettingsd
hacker       149     119  3 04:40 ?        00:00:00 xfce4-panel
hacker       154     119  0 04:40 ?        00:00:00 Thunar --daemon
hacker       161     119  2 04:40 ?        00:00:00 xfdesktop
hacker       178     149  0 04:40 ?        00:00:00 /nix/store/xpgf309sv9w5majf26zg50fpd9vqk1x3-xfce4-panel-4.18.6/lib/xfce4/panel/wrapper-2.0 /run/cu
hacker       182     149  0 04:40 ?        00:00:00 /nix/store/xpgf309sv9w5majf26zg50fpd9vqk1x3-xfce4-panel-4.18.6/lib/xfce4/panel/wrapper-2.0 /run/cu
hacker       274     109  1 04:40 ?        00:00:00 /nix/store/3wb0055984n2whn449hywsl4ag9gcjir-python3-3.11.9/bin/python3.11 /nix/store/pma5sqhyxm2zq
hacker       299       1  0 04:40 ?        00:00:00 /run/workspace/bin/xfce4-mime-helper --launch TerminalEmulator
hacker       300     299  3 04:40 ?        00:00:00 /run/workspace/bin/xfce4-terminal
hacker       306     300  0 04:40 pts/0    00:00:00 bash
hacker       328     306  0 04:40 pts/0    00:00:00 ps -ef
hacker@processes~listing-processes:~$ /challenge/1061-run-10844
Yahaha, you found me! Here is your flag:
pwn.college{MqnK_7K9V8KnhbFZJ_B-GWQgYc1.dhzM4QDLzETN0czW}
Now I will sleep for a while (so that you could find me with 'ps').
