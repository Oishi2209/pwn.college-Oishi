# Multiple options for tab completion
This challenge has a /challenge/files directory with a bunch of files starting with pwncollege. Tab-complete from /challenge/files/p or so, and make your way to the flag!

## Solution
Repeatedly used /challenge/files/p<tab> to search for the flag.
```sh
Connected!
hacker@globbing~multiple-options-for-tab-completion:~$ cd /challenge/files
hacker@globbing~multiple-options-for-tab-completion:/challenge/files$ /challenge/files/pwn
pwn                    pwn-the-planet         pwncollege-flamingo    pwncollege-hacking
pwn-college            pwncollege-family      pwncollege-flyswatter
hacker@globbing~multiple-options-for-tab-completion:/challenge/files$ /challenge/files/pwn-
pwn-college     pwn-the-planet
hacker@globbing~multiple-options-for-tab-completion:/challenge/files$ /challenge/files/pwn-college
hack-the-planet        pwn-college            pwncollege-family      pwncollege-flamingo    pwncollege-hacking
pwn                    pwn-the-planet         pwncollege-flag        pwncollege-flyswatter
hacker@globbing~multiple-options-for-tab-completion:/challenge/files$ cat pwncollege-flag
pwn.college{oajJS9S9WtwNjBFA-ZE9Fi_Qzg-.0lN0EzNxwCM0AzNzEzW}
```

## Flag: 

```
pwn.college{oajJS9S9WtwNjBFA-ZE9Fi_Qzg-.0lN0EzNxwCM0AzNzEzW}
```

### References:
none

### Notes:
By default bash will auto-expand until the first point when there are multiple options (in this case, fl). When you hit tab a second time, it'll print out those options
