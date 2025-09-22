#Intro To Arguments

Introduction to arguments, which is what we call additional data passed to the command. When you type a line of text and hit enter, the shell actually parses your input into a command and its arguments.
```sh
hacker@dojo:~$ echo Hello
Hello
hacker@dojo:~$
```
In this case, the command was echo, and the argument was Hello. echo is a simple command that "echoes" all of its arguments back out onto the terminal.
## Solution:

In this challenge, to get the flag, you must run the hello command (NOT the echo command) with a single argument of hackers.

#### Commands run: 

```sh
hello hackers
```

## Flag: 

```
pwn.college{01c0H3_9Wdgzeoz7OzeUzPBD4kn.QX4YjM1wCM0AzNzEzW}
```

### Notes:
The first word is the command, and the subsequent words are arguments.
