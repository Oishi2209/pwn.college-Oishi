# Multi-word variables
In this level, you'll need to set the variable PWN to COLLEGE YEAH.

## Solution
Set PWN="COLLEGE YEAH" to print the flag.

```sh
Connected!
hacker@variables~multi-word-variables:~$ PWN="COLLEGE YEAH"
You've set the PWN variable properly! As promised, here is the flag:
pwn.college{0MtA1pnx7B1vSy1-qOXEKDwvsDW.QXwYTN0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{0MtA1pnx7B1vSy1-qOXEKDwvsDW.QXwYTN0wCM0AzNzEzW}
```

### References:
none

### Notes:
When the shell sees a space, it ends the variable assignment and interprets the next word (SAUCE in this case) as a command. To set VAR to 1337 SAUCE, you need to quote it:

hacker@dojo:~$ VAR="1337 SAUCE"
