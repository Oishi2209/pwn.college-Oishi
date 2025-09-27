# Searching manuals
Find the option that will give you the flag by reading the challenge man page.

## Solution
Used man command to read the manual for challenge. Used /flag to find the flag. Used --qy argument from there to get the flag.

```sh
Connected!
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge --qy
Initializing...
Correct usage! Your flag: pwn.college{Q_REuQBHdiD_kxKvJaDCrUdDRJt.QX1EDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{Q_REuQBHdiD_kxKvJaDCrUdDRJt.QX1EDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
man is short for manual, and will display (if available) the manual of the command you pass as an argument.
