# Position elsewhere

This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program

## Solution
We essentially need to execute /challenge/run program from a specific path. First I typed /challenge/run and got the path. Then I used the cd (change directory) command with the directory provided and finally ran the /challenge/run program.

```sh
Connected!
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /var/lib/apt/lists directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /var/lib/apt/lists
hacker@paths~position-elsewhere:/var/lib/apt/lists$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{sMKSQFU2BJCMTgmJNXcpe7-oFl4.QX3QTN0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{sMKSQFU2BJCMTgmJNXcpe7-oFl4.QX3QTN0wCM0AzNzEzW}
```

### References:
none

### Notes:
-You can navigate around directories by using the cd (change directory) command and passing a path to it as an argument.
- '~' shows the current path that your shell is located at.
