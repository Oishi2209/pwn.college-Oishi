# Redirecting input
You can do interesting things with a lot of different programs using input redirection! In this level, we will practice using /challenge/run, which will require you to redirect the PWN file to it and have the PWN file contain the value COLLEGE!

## Solution
Used echo COLLEGE>PWN and /challenge/run < PWN to get the flag.

```sh
Connected!
hacker@piping~redirecting-input:~$ echo COLLEGE>PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{8vzS0s1nGPG0UU9RtxmWVxxR7W4.QXwcTN0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{8vzS0s1nGPG0UU9RtxmWVxxR7W4.QXwcTN0wCM0AzNzEzW}
```

### References:
none

### Notes:
Just like you can redirect output from programs, you can redirect input to programs! This is done using <, as so:

hacker@dojo:~$ echo yo > message
hacker@dojo:~$ cat message
yo
hacker@dojo:~$ rev < message
oy
