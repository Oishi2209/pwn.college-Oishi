# The root
In this challenge, you'll be giving the exact path, starting from /, so the path would be /pwn. 

## Solution

**Flag:** `pwn.college{At3OV5mFWdwuRF7fJt4yMex8LK6.QX4cTO0wCM0AzNzEzW}`

```bash
Connected!
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{At3OV5mFWdwuRF7fJt4yMex8LK6.QX4cTO0wCM0AzNzEzW}
```
### References 
None

### Notes
File system starts at '/'.
You can invoke a program by providing its path on the command line.
A path from the root of the filesystem starts with / and describes the set of directories that must be descended into to find the file. 
Every piece of the path is demarcated with another /.



