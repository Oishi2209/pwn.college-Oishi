# Implicit relative paths

Explicitly use relative paths to launch run in this scenario. Tell Linux that you explicitly want to execute a program in the current directory, using . 

## Solution
It is mentioned in the problem statement that we are supposed to run the code from the challenge directory so i used cd to switch to it. Next it is mentioned that we need to explicitly tell linux to execute run program in the challenge directory hence I used ./run

```sh
Connected!
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{AOjuoAlof-8TkN3jezDS5_bhuTf.QXxUTN0wCM0AzNzEzW}
hacker@paths~implicit-relative-path:/challenge$
```

## Flag: 

```
pwn.college{AOjuoAlof-8TkN3jezDS5_bhuTf.QXxUTN0wCM0AzNzEzW}
```

### References:
none

### Notes:
Linux explicitly avoids automatically looking in the current directory when you provide a "naked" path i.e. without the use of '.' This is actually a safety measure: if Linux searched the current directory for programs every time you entered a naked path, you could accidentally execute programs in your current directory that happened to have the same names as core system utilities.
