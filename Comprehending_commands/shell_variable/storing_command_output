# CTF Challenge: storing_command_output

## Table of Content

- commands-executed: PWN=$(/challenge/run) , echo $PWN
- flag :pwn.college{saX3LYIsgvYEmqbrH9N_8sAgxu1.dVzN0UDLzETN0czW}



### Objective:

In the course of working with the shell, you will often want to store the output of some command into a variable. Luckily, the shell makes this quite easy using something called Command Substitution! Observe:

hacker@dojo:~$ FLAG=$(cat /flag)
hacker@dojo:~$ echo "$FLAG"
pwn.college{blahblahblah}
hacker@dojo:~$
Neat! Now, you practice. Read the output of the /challenge/run command directly into a variable called PWN, and it will contain the flag!

Trivia: You can also backticks instead of $(): FLAG=`cat /flag` instead of FLAG=$(cat /flag) in the example above. This is an older format, and has some disadvantages (for example, imagine if you wanted to nest command substitutions. How would you do $(cat $(find / -name flag)) with backticks? The official stance of pwn.college is that you should use $(blah) instead of `blah`.

### Output:
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out 
and submit it!
hacker@variables~storing-command-output:~$ echo PWN
PWN
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{saX3LYIsgvYEmqbrH9N_8sAgxu1.dVzN0UDLzETN0czW}
