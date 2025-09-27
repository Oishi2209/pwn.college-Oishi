# Comparing files
Now for your challenge! There are two files in /challenge:

/challenge/decoys_only.txt contains 100 fake flags
/challenge/decoys_and_real.txt contains all 100 fake flags plus the one real flag
Use diff to find what's different between these files and get your flag!

## Solution
We must use diff command to find the real flag between the two directories. I simply use diff command to find out the difference between the two files i.e. the flag.
```sh
Connected!
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
47a48
> pwn.college{AxfwmXAglVws5SBA883zdNdJOBr.01MwMDOxwCM0AzNzEzW}
```

## Flag: 

```
pwn.college{AxfwmXAglVws5SBA883zdNdJOBr.01MwMDOxwCM0AzNzEzW}
```

### References:
none

### Notes:
diff compares two files line by line and shows you exactly what's different between them.
