# CTF Challenge: explicit relative path

## Table of Content

- commands-executed:  cd ../ , ./challenge/run
- flag :pwn.college{wKiOg1eSajo3075bLHIvpoMN9mp.dBTN1QDLzETN0czW}

### Objective:
Previously, your relative path was "naked": it directly specified the directory to descend into from the current directory. In this level, we're going to explore more explicit relative paths.

In most operating systems, including Linux, every directory has two implicit entries that you can reference in paths: . and ... The first, ., refers right to the same directory, so the following absolute paths are all identical to each other:

/challenge
/challenge/.
/challenge/./././././././././
/./././challenge/././
The following relative paths are also all identical to each other:

challenge
./challenge
./././challenge
challenge/.
Of course, if your current working directory is /, the above relative paths are equivalent to the above absolute paths.

This challenge will get you using . in your relative paths. Get ready!

### Output:

hacker@paths~explicit-relative-paths-from-:~$ cd ../
hacker@paths~explicit-relative-paths-from-:/home$ cd ../
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{wKiOg1eSajo3075bLHIvpoMN9mp.dBTN1QDLzETN0czW}




