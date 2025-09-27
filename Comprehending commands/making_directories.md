# Making directories 
Create a /tmp/pwn directory and make a college file in it! Then run /challenge/run, which will check your solution and give you the flag.

## Solution
First I used the mkdir /tmp/pwn command to create the required directory. Next I used cd to insert myself in the tmp directory. Used ls to check contents. Finally used touch command to create college file and run /challenge/run.

```sh
Connected!
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ cd /tmp
hacker@commands~making-directories:/tmp$ ls
bin  hsperfdata_root  pwn  tmp.4mK6TfTSUV
hacker@commands~making-directories:/tmp$ touch /tmp/pwn/college
hacker@commands~making-directories:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{IjWsBnPqewqQIVY9KJxNnmo3rb-.QXxMDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{IjWsBnPqewqQIVY9KJxNnmo3rb-.QXxMDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
You make directories using the mkdir command. Then use touch command to create files there.
