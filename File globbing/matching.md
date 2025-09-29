# Matching with *
Starting from your home directory, change your directory to /challenge, but use globbing to keep the argument you pass to cd to at most four characters! Once you're there, run /challenge/run for the flag.

## Solution
Used cd /ch* command to change directories and ran /challenge/run to get the flag.

```sh
Connected!
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{QfU2y3qOjCB9juIgQD4elNqx3Yw.QXxIDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{QfU2y3qOjCB9juIgQD4elNqx3Yw.QXxIDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
When it encounters a * character in any argument, the shell will treat it as a "wildcard" and try to replace that argument with any files that match the pattern. The * matches any part of the filename except for / or a leading . character. 
