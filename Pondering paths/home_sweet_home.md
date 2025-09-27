# Home sweet home

In this challenge, /challenge/run will write a copy of the flag to any file you specify as an argument on the commandline, with these constraints:

Your argument must be an absolute path.
The path must be inside your home directory.
Before expansion, your argument must be three characters or less.
Again, you must specify your path as an argument to /challenge/run

## Solution
The challenge mentions that /challenge/run will write a copy of the flag to any specified file. Since we need to provide an absolute path for the argument I ran the /challenge/run ~/g command to get the flag.

```sh
Connected!
hacker@paths~home-sweet-home:~$ /challenge/run ~/g
Writing the file to /home/hacker/g!
... and reading it back to you:
pwn.college{oDgsNFY_gl198LQjNqg-Psok-76.QXzMDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{oDgsNFY_gl198LQjNqg-Psok-76.QXzMDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
The home directory is typically where users store most of their personal files. The ~ in this prompt is the current working directory, with ~ being shorthand for /home/hacker. Whenever bash sees ~ provided as the start of an argument in a way consistent with a path, it will expand it to your home directory. Note that the expansion of ~ is an absolute path, and only the leading ~ is expanded.
