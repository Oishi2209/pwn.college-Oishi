# Catting absolute paths
In this directory, I will not copy it to your home directory, but I will make it readable. You can read it with cat at its absolute path: /flag.

## Solution
The challenge says to use cat to read the flag which is not available in the home directory so I used the absolute path '/flag' with the cat command to get the flag.

```sh
Connected!
hacker@commands~catting-absolute-paths:~$ cat /flag
pwn.college{oFslEwkh17dSgH5Quay0OHghGjw.QX5ETO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{oFslEwkh17dSgH5Quay0OHghGjw.QX5ETO0wCM0AzNzEzW}
```

### References:
none

### Notes:
We can specify cat's arguments as absolute paths.
