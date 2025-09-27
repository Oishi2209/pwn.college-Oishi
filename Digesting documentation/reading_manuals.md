# Reading manuals
The challenge in this level has a secret option that, when you use it, will cause the challenge to print the flag. You must learn this option through the man page for challenge!

## Solution
Used the man challenge command to read the manual for challenge. There I saw the --ftxnim NUM argument which showed it would print for NUM 315. Used that to print the flag.

```sh
Connected!
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --ftnxim 315
Correct usage! Your flag: pwn.college{Eft31nZxRZiC50mgbn6mKx4I_Is.QX0EDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{Eft31nZxRZiC50mgbn6mKx4I_Is.QX0EDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
man is short for manual, and will display (if available) the manual of the command you pass as an argument.
