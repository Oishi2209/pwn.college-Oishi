# Writing to multiple programs
In this challenge, we have /challenge/hack, /challenge/the, and /challenge/planet. Run the /challenge/hack command, and duplicate its output as input to both the /challenge/the and the /challenge/planet commands!

## Solution
Used /challenge/hack | tee >(/challenge/the) >(/challenge/planet) to get the flag.

```sh
Connected!
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
23431565631820677
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{IpbIDccXGnE7eKefYUH7guZCwLT.QXwgDN1wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{IpbIDccXGnE7eKefYUH7guZCwLT.QXwgDN1wCM0AzNzEzW}
```

### References:
none

### Notes:
none
