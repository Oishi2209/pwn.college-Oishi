# Help for builtins
In this challenge, we'll practice using help to look up help for builtins. This challenge's challenge command is a shell builtin, rather than a program. Like before, you need to lookup its help to figure out the secret value to pass to it.

## Solution
Used the help challenge command since it is builtin. This gave me a list of arguments including -- secret VALUE along with said value "4jcCjCV4". Finally used the challenge --secret 4jcCjCV4 command to get the flag.

```sh
Connected!
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "4jcCjCV4".
hacker@man~help-for-builtins:~$ challenge --secret 4jcCjCV4
Correct! Here is your flag!
pwn.college{4jcCjCV4QxGPlePUv9kK7Tm-qXo.QX0ETO0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{4jcCjCV4QxGPlePUv9kK7Tm-qXo.QX0ETO0wCM0AzNzEzW}
```

### References:
none

### Notes:
Some commands, rather than being programs with man pages and help options, are built into the shell itself. These are called builtins. Builtins are invoked just like commands, but the shell handles them internally instead of launching other programs. You can get a list of shell builtins by running the builtin help.
