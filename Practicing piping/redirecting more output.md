# Redirecting more output
In this level, /challenge/run will once more give you a flag, but only if you redirect its output to the file myflag. Your flag will, of course, end up in the myflag file!

## Solution
Used challenge/run > myflag to redirect output to myflag file. Used cat myflag to get the flag. 

```sh
Connected!
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{ENqfZFRFUV0_uctYDJpCFa3lkwM.QX1YTN0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{ENqfZFRFUV0_uctYDJpCFa3lkwM.QX1YTN0wCM0AzNzEzW}
```

### References:
none

### Notes:
Aside from redirecting the output of echo, you can redirect the output of any command.
