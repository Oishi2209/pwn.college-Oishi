# Matching with ?
Starting from your home directory, change your directory to /challenge, but use the ? character instead of c and l in the argument to cd! Once you're there, run /challenge/run for the flag!

## Solution
Used cd /?ha??enge command to change directories and ran /challenge/run to get the flag.
```sh
Connected!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{MINUtFvtZo9bIf5UR3fKT7i0BnC.QXyIDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{MINUtFvtZo9bIf5UR3fKT7i0BnC.QXyIDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
When it encounters a ? character in any argument, the shell will treat it as a single-character wildcard. This works like *, but only matches one character.
