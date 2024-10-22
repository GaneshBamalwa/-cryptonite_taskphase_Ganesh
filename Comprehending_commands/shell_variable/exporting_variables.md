# CTF Challenge: exporting_variables

## Table of Content

- commands-executed:COLLEGE=PWN , PWN=COLLEGE, export PWN , sh ,/challenge/run
- flag :pwn.college{QVhwALd0QnMTf5hFUzXjNRv55rO.dJjN1QDLzETN0czW


### Output:
```console

hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ PWN=COLLEGE
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ export PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ sh
sh-5.2$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great 
job! Here is your flag:
pwn.college{QVhwALd0QnMTf5hFUzXjNRv55rO.dJjN1QDLzETN0czW}
```
