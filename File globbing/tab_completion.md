# Tab completion
This challenge has copied the flag into /challenge/pwncollege, and you can freely cat that file. But you can't type the filename

## Solution
Used cd/challenge/pwn<TAB> to complete the file path and get the flag.

```sh
Connected!
hacker@globbing~tab-completion:~$ cat /challenge/pwncollege​
pwn.college{Ed4BlR9S_aioLks-XGFiPN8PBrC.0FN0EzNxwCM0AzNzEzW}
```

## Flag: 

```
pwn.college{Ed4BlR9S_aioLks-XGFiPN8PBrC.0FN0EzNxwCM0AzNzEzW}
```

### References:
none

### Notes:
If you hit tab in the shell, it'll try to figure out what you're going to type and automatically complete it.
