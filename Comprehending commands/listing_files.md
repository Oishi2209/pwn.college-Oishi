# Listing files
In this challenge, we've named /challenge/run with some random name! List the files in /challenge to find it.

## Solution
We have to use ls command to find the contents of the current directory. There we see the file names. We simply have to find it in the challenge directory next.

```sh
Connected!
hacker@commands~listing-files:~$ ls /challenge
2085-renamed-run-15071  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/2085-renamed-run-15071
Yahaha, you found me! Here is your flag:
pwn.college{w77hjkXOSMWb0vI8Q0Z6grrRM_3.QX4IDO0wCM0AzNzEzW}
hacker@commands~listing-files:~$
```

## Flag: 

```
pwn.college{w77hjkXOSMWb0vI8Q0Z6grrRM_3.QX4IDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
Directories can have lots of files (and other directories) inside them. We list their contents using the ls command. ls will list files in all the directories provided to it as arguments, and in the current directory if no arguments are provided
