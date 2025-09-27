# Touching files
Create two files: /tmp/pwn and /tmp/college, and run /challenge/run to get your flag.

## Solution
Using cd command first I located myself inside the tmp directory. Next used the ls command to search contents of the same. Using touch command I created two files (pwn and college). Used ls command to verify that the files have been created. Finally run /challenge/run command to get the flag.

```sh
Connected!
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ ls
bin  hsperfdata_root  tmp.4mK6TfTSUV
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.4mK6TfTSUV
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{cjS4-31q4qIS2H-Sj89m5V6y7st.QXwMDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{cjS4-31q4qIS2H-Sj89m5V6y7st.QXwMDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
You can create a new, blank file by touching it with the touch command. Example: hacker@dojo:/tmp$ touch pwnfile.
