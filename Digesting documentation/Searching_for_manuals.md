# Searching for manuals
This challenge hides the manpage for the challenge by randomizing its name. Luckily, all of the manpages are gathered in a searchable database, so you'll be able to search the man page database to find the hidden challenge man page! To figure out how to search for the right manpage, read the man page manpage by doing: man man!

## Solution
First I used man man to see the manual page. There it was mentioned that man -k keyword searches the manual page for the specified keyword. So I searched for man -k challenge. Terminal showed nwyuzhdzvk (1) -- print the flag. Hence I used the man nwyuzhdzvk command. The manual showed me the correct argument to get the flag.

```sh
Connected!
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -l
What manual page do you want?
For example, try 'man man'.
hacker@man~searching-for-manuals:~$ /challenge/challenge --l
Incorrect usage! Please read the hidden challenge man page!
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k flag
hacker@man~searching-for-manuals:~$ man -k challenge
nwyuzhdzvk (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man nwyuzhdzvk
hacker@man~searching-for-manuals:~$ /challenge/challenge --nwyuzh 486
Correct usage! Your flag: pwn.college{AJnwyLOYuB4NzhdzvVWIkOoFQ86.QX2EDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{AJnwyLOYuB4NzhdzvVWIkOoFQ86.QX2EDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
none
