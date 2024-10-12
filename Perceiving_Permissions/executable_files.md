# CTF Challenge: executable_files

## Table of Content

- commands-executed: chmod +x /challenge/run , ls -l /challenge/run  , /challenge/run
- flag :pwn.college{kZcP4n6kUV1mznYDlCnJpGPWJEo.dJTM2QDLzETN0czW}


### Output:
hacker@permissions~executable-files:~$ ls -l /challenge/run 
-r--r--r-- 1 hacker hacker 32 Jul  4 06:37 /challenge/run
hacker@permissions~executable-files:~$ chmod go-wrx /challenge/run 
hacker@permissions~executable-files:~$ /challenge/run
bash: /challenge/run: Permission denied
hacker@permissions~executable-files:~$ chmod +x /challenge/run 
hacker@permissions~executable-files:~$ /challenge/run 
Successful execution! Here is your flag:
pwn.college{kZcP4n6kUV1mznYDlCnJpGPWJEo.dJTM2QDLzETN0czW}

