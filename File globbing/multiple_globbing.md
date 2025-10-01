# Multiple globs
We put a few happy, but diversely-named files in /challenge/files. Go cd there and run /challenge/run, providing a single argument: a short (3 characters or less) globbed word with two * globs in it that covers every word that contains the letter p

## Solution
Used cd /challenge/files to access directory. Then ran /challenge/run *p* to search for any files containing p.
```sh
Connected!
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{Uhs7DQYxvpnW3OQB2Hdc8UiSSmK.0lM3kjNxwCM0AzNzEzW}
```

## Flag: 

```
pwn.college{Uhs7DQYxvpnW3OQB2Hdc8UiSSmK.0lM3kjNxwCM0AzNzEzW}
```

### References:
none

### Notes:
ash supports the expansion of multiple globs in a single word.
