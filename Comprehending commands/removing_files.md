# Removing files
his challenge will create a delete_me file in your home directory! Delete it, then run /challenge/check, which will make sure you've deleted it and then give you the flag.

## Solution
Used ls command to check the files. Next used rm command to delete the mentioned file. Finally ran /challenge/check to get the flag.

```sh
Connected!
hacker@commands~removing-files:~$ ls
delete_me  g
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{Uf2DCIxO9W00WucKx-cJchOMoP9.QX2kDM1wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{Uf2DCIxO9W00WucKx-cJchOMoP9.QX2kDM1wCM0AzNzEzW}
```

### References:
none

### Notes:
In Linux, you remove files with the rm command. Example: hacker@dojo:~$ rm PWN.
