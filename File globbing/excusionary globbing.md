# exclusionary globbing
Armed with this knowledge, go forth to /challenge/files and run /challenge/run with all files that don't start with p, w, or n

## Solution
Used cd to change directories. Used /challenge/run [!pwn]* to look for files which dont contain p, w and n and get the flag.

```sh
Connected!
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{EEAfXKTNaq-XmH5PFbLHiNm7iUI.QX2IDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{EEAfXKTNaq-XmH5PFbLHiNm7iUI.QX2IDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
 If the first character in the brackets is a ! or (in newer versions of bash) a ^, the glob inverts, and that bracket instance matches characters that aren't listed.
