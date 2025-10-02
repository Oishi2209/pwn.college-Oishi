# Split piping for stderr & stdout
In this challenge, you have:

/challenge/hack: this produces data on stdout and stderr
/challenge/the: you must redirect hack's stderr to this program
/challenge/planet: you must redirect hack's stdout to this program
Go get the flag!

## Solution
Used /challenge/hack 2> >( /challenge/the ) | /challenge/planet to get the flag.

```sh
Connected!
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >( /challenge/the ) | /challenge/planet
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{oVkVi8OUZkGk3wAsOuZgxt557Oj.QXxQDM2wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{oVkVi8OUZkGk3wAsOuZgxt557Oj.QXxQDM2wCM0AzNzEzW}
```

### References:
none

### Notes:
none
