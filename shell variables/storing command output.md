# Storing command output
Read the output of the /challenge/run command directly into a variable called PWN, and it will contain the fl.

## Solution
Used PWN=$(/challenge/run) to read the flag into the PWN variable and printed it using echo to view the flag.

```sh
Connected!
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echpo $PWN
bash: echpo: command not found
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{0ZBpwRazCTmFFbyJp5DRyedkGK1.QX1cDN1wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{0ZBpwRazCTmFFbyJp5DRyedkGK1.QX1cDN1wCM0AzNzEzW}
```

### References:
none

### Notes:
hacker@dojo:~$ FLAG=$(cat /flag)
hacker@dojo:~$ echo "$FLAG"
pwn.college{blahblahblah}
hacker@dojo:~$
