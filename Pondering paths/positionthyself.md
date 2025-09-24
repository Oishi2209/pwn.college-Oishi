# Position thy self

This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program.

## Solution:

-We essentially need to execute /challenge/run program from a specific path. 
-First I typed /challenge/run and got me the path. 
-Then I used the cd (change directory) command with the directory provided and finally ran the /challenge/run program.

Use this blob for pasting commands you've run
```sh
Connected!
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/build-essential directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /usrr/share/build-essential directory
hacker@paths~position-thy-self:~$ cd /usr/share/build-essential
hacker@paths~position-thy-self:/usr/share/build-essential$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{84dAzsmXupQRyQv19rRV9R7PVq8.QX2QTN0wCM0AzNzEzW}
hacker@paths~position-thy-self:/usr/share/build-essential$

```

## Flag: 

```
pwn.college{84dAzsmXupQRyQv19rRV9R7PVq8.QX2QTN0wCM0AzNzEzW}
```

### References:
none

### Notes:
-You can navigate around directories by using the cd (change directory) command and passing a path to it as an argument.
- '~' shows the current path that your shell is located at.


