# Helpful programs
In this level, you will practice reading a program's documentation with --help. 

## Solution
First ran /challenge/challenge --help command to get list of arguments. rank </challenge/challenge --print-value> argument to get the key value (378). Used /challenge/challenge -g 378 to get the flag.

```sh
Connected!
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge --print-value
The secret value is: 378
hacker@man~helpful-programs:~$ /challenge/challenge -g 378
Correct usage! Your flag: pwn.college{oiasQawdnEB-XN-e3D7kKJLIjr8.QX3IDO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{oiasQawdnEB-XN-e3D7kKJLIjr8.QX3IDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
Some programs don't have a man page, but might tell you how to run them if invoked with a special argument. Usually, this argument is --help, but it can often be -h.
