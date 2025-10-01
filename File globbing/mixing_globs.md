# Mixing globs
We put a few happy, but diversely-named files in /challenge/files. Go cd there and, using the globbing you've learned, write a single, short (6 characters or less) glob that (when passed as an argument to /challenge/run) will match the files "challenging", "educational", and "pwning"!

## Solution
Used cd /challenge/files to change directories. Next, ran /challenge/run [cep]* to get the flag.
```sh
Connected!
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{kIednUqAQ3CIGxbm1SEnbnY9OCx.QX1IDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{kIednUqAQ3CIGxbm1SEnbnY9OCx.QX1IDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
none
