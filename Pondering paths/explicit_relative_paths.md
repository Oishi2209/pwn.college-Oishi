# Explicit relative paths

This challenge will get you using . in your relative paths.

## Solution
First I tried to change directories to challenge. Next I tried ./run to get the flag. That told me I need to be in the / directory so I used cd to change directory. Next i ran ./challenge/run to get the flag.

```sh
Connected!
hacker@paths~explicit-relative-paths-from-:/$ cd /challenge
hacker@paths~explicit-relative-paths-from-:/challenge$ ./run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:/challenge$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{wgw0gS3Q57Mg_Mfol1PhZ480BvH.QXwUTN0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{wgw0gS3Q57Mg_Mfol1PhZ480BvH.QXwUTN0wCM0AzNzEzW}
```

### References:
none

### Notes:
Every directory has two implicit entries that you can reference in paths: . and ... The first, ., refers right to the same directory, so the following absolute paths are all identical to each other:
/challenge
/challenge/.
/challenge/./././././././././
/./././challenge/././

The following relative paths are also all identical to each other:
challenge
./challenge
./././challenge
challenge/.
