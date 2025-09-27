# More catting practise 
I'll put the flag in some crazy directory, and I will not allow you to change directories with cd, so no cat flag for you. You must retrieve the flag by absolute path, wherever it is.

## Solution
The challenge says to use cat to read the flag wherever it has been put. File has been mentioned in the prompt file /lib/cmake/flag. So I used the absolute path of the flag to retrieve it.

```sh
Connected!
You cannot use the 'cd' command in this level, and must retrieve the flag by
absolute path. Plus, I hid the flag in a different directory! You can find it
in the file /lib/cmake/flag. Go cat it out **without** cding into that
directory!
hacker@commands~more-catting-practice:~$ cat /lib/cmake/flag
pwn.college{Y1KoTIQ-7jU_oTjRq2R67b062CG.QXwITO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{Y1KoTIQ-7jU_oTjRq2R67b062CG.QXwITO0wCM0AzNzEzW}
```

### References:
none

### Notes:
We can specify cat's arguments as absolute paths.
