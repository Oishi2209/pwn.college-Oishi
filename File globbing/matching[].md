# Matching with []
We've placed a bunch of files in /challenge/files. Change your working directory to /challenge/files and run /challenge/run with a single argument that bracket-globs into file_b, file_a, file_s, and file_h!

## Solution
First used cd to change directory to challenge. Next, used /challenge/run file_[bash] to get the flag (this matches file_a, file_b, file_s and file_h).

```sh
Connected!
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[bash]
You got it! Here is your flag!
pwn.college{km6WqzDh2Q4k4IEIu42d10pXooz.QXzIDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{km6WqzDh2Q4k4IEIu42d10pXooz.QXzIDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
The square brackets are, essentially, a limited form of ?, in that instead of matching any character, [] is a wildcard for some subset of potential characters, specified within the brackets. 
