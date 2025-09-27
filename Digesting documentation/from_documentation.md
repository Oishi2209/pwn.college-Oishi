# Digesting documentation
The program for this challenge is /challenge/challenge, and you'll need to invoke it properly in order for it to give you the flag. Let's pretend that this is its documentation:

Welcome to the documentation for /challenge/challenge! To properly run this program, you will need to pass it the argument of --giveflag. Good luck!

## Solution
First I used the /challenge/challenge --giveflag to pass the argument and get the flag.

```sh
Connected!
hacker@man~learning-from-documentation:~$ /challenge/challenge
Incorrect usage! You must pass an argument to me (read the challenge
description for details).
hacker@man~learning-from-documentation:~$ /challenge/challenge --giveflag
Correct argument! Here is your flag:
pwn.college{UbVJA8XNr2JXqPMtxQI3ChKH0t5.QX0ITO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{UbVJA8XNr2JXqPMtxQI3ChKH0t5.QX0ITO0wCM0AzNzEzW}
```

### References:
none

### Notes:
This module will mostly dig into that concept, as a proxy for figuring out how to use the programs in general. Through the rest of the module, you'll go through various ways of asking the environment for help for the programs, but first, we'll dig into the concept of reading documentation.
