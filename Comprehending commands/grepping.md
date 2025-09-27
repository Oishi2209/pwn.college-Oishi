# Grepping 
In this challenge, I've put a hundred thousand lines of text into the /challenge/data.txt file. grep it for the flag!
## Solution
We have to use grep command to specifically search for the flag among massive lines of code. Since the flag always starts with 'pwn.college' we use it to search for the flag along with the path given.

```sh
Connected!
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{gkdLC5CgVXpBXN8nZrjljD34bFx.QX3EDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{gkdLC5CgVXpBXN8nZrjljD34bFx.QX3EDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
Sometimes, the files that you might cat out are too big. We use the grep command to search for the contents we need. It is invoked as follows hacker@dojo:~$ grep SEARCH_STRING /path/to/file.
