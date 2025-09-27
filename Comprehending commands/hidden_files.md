# Hidden files
Find the flag, hidden as a dot-prepended file in /s.

## Solution
First used cd command to position myself inside the / directory. Next used ls -a command to see all files including the .flag-116382324127795 file. Used cat command to get the flag.

```sh
Connected!
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-116382324127795  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-116382324127795
pwn.college{wyIhwmKBS4tS84wTwOFZ1neSILB.QXwUDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{wyIhwmKBS4tS84wTwOFZ1neSILB.QXwUDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
ls doesn't list all the files by default. Linux has a convention where files that start with a . don't show up by default in ls and in a few other contexts. To view them with ls, you need to invoke ls with the -a flag.
