# Matching paths with [] 
We've placed a bunch of files in /challenge/files. Starting from your home directory, run /challenge/run with a single argument that bracket-globs into the absolute paths to the file_b, file_a, file_s, and file_h files!

## Solution
Used /challenge/run /challenge/files/file_[bash] to get the flag.
```sh
Connected!
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[bash]
You got it! Here is your flag!
pwn.college{wD00si_f31Pjm9Twgs-LdC1sE0l.QX0IDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{wD00si_f31Pjm9Twgs-LdC1sE0l.QX0IDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
Globbing happens on a path basis, so you can expand entire paths with your globbed arguments
