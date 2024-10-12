# CTF Challenge: cracking_passwords

## Table of Content

- commands-executed: john /challenge/shadow-leak --show , su zardus
- flag :pwn.college{Ig71oiuLl-fzoMtb8Vwa4A92o17.ddTN0UDLzETN0czW}


### Output:

hacker@users~cracking-passwords:~$ john /challenge/shadow-leak 
Created directory: /home/hacker/.john
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:21 100% 2/3 0.04694g/s 273.3p/s 273.3c/s 273.3C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak --show
hacker:NO PASSWORD:20000:0:99999:7:::
zardus:aardvark:20008:0:99999:7:::

2 password hashes cracked, 0 left
hacker@users~cracking-passwords:~$ su zardus
Password: 
zardus@users~cracking-passwords:/home/hacker$ /challenge/run 
Congratulations, you have become Zardus! Here is your flag:
pwn.college{Ig71oiuLl-fzoMtb8Vwa4A92o17.ddTN0UDLzETN0czW}
