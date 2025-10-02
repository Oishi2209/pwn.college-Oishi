# Exporting variables
In this challenge, you must invoke /challenge/run with the PWN variable exported and set to the value COLLEGE, and the COLLEGE variable set to the value PWN but not exported (e.g., not inherited by /challenge/run).
## Solution
Set PWN=COLLEGE. Exported PWN. Next set COLLEGE=PWN and finally ran /challenge/run PWN to get the flag.

```sh
Connected!
hacker@variables~exporting-variables:~$ PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ export PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ /challenge/run PWN
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{E8GzBnTMv_y1AzTkEe_M7reziIY.QXyYTN0wCM0AzNzEzW}
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
```

## Flag: 

```
pwn.college{E8GzBnTMv_y1AzTkEe_M7reziIY.QXyYTN0wCM0AzNzEzW}
```

### References:
none

### Notes:
In the output above, the $ prompt is the prompt of sh, a minimal shell implementation that is invoked as a child of the main shell process. And it does not receive the VAR variable.
