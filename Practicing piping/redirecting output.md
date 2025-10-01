# Redirecting output
In this challenge, you must use this output redirection to write the word PWN (all uppercase) to the filename COLLEGE (all uppercase).

## Solution
Used echo pwn>college to get the flag.
```sh
Connected!
hacker@piping~redirecting-output:~$ echo PWN>COLLEGE
Correct! You successfully redirected 'PWN' to the file 'COLLEGE'! Here is your
flag:
pwn.college{8njhCIVt-i8RK5zrNWPqu6UpNx8.QX0YTN0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{8njhCIVt-i8RK5zrNWPqu6UpNx8.QX0YTN0wCM0AzNzEzW}
```

### References:
none

### Notes:
hacker@dojo:~$ echo hi > asdf
This will redirect the output of echo hi (which will be hi) to the file asdf.
