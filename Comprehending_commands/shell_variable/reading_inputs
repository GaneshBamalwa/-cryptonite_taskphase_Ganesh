# CTF Challenge: reading_inputs

## Table of Content

- commands-executed:read -p "Enter" PWN
- flag :pwn.college{szzWaqw5MlulU60wh2lUp7_lDtT.dhzN1QDLzETN0czW}



### Objective:

We'll start with reading input from the user (you). That's done using the aptly named read builtin, which reads input!

Here is an example using the -p argument, which lets you specify a prompt (otherwise, it would be hard for you, reading this now, to separate input from output in the example below):

hacker@dojo:~$ read -p "INPUT: " MY_VARIABLE
INPUT: Hello!
hacker@dojo:~$ echo "You entered: $MY_VARIABLE"
You entered: Hello!
Keep in mind, read reads data from your standard input! The first Hello!, above, was inputted rather than outputted. Let's try to be more explicit with that. Here, we annotated the beginning of each line with whether the line represents INPUT from the user or OUTPUT to the user:

 INPUT: hacker@dojo:~$ echo $MY_VARIABLE
OUTPUT:
 INPUT: hacker@dojo:~$ read MY_VARIABLE
 INPUT: Hello!
 INPUT: hacker@dojo:~$ echo "You entered: $MY_VARIABLE"
OUTPUT: You entered: Hello!
In this challenge, your job is to use read to set the PWN variable to the value COLLEGE. Good luc

### Output:

hacker@variables~reading-input:~$ read -p "Enter" PWN
EnterCOLLEGE
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{szzWaqw5MlulU60wh2lUp7_lDtT.dhzN1QDLzETN0czW}
