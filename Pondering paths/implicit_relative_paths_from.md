# Implicit relative paths

You'll need to run /challenge/run using a relative path while having a current working directory of /.

## Solution
Since current working directory is given as '/' and we need to run /challenge/run; we need to remove / to get relative path which is challenge/run.

```sh
Connected!
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{con2-PeTuyaNZ0BnEeh_sJ-hYse.QX5QTN0wCM0AzNzEzW}
```

## Flag: 

```
pwn.college{con2-PeTuyaNZ0BnEeh_sJ-hYse.QX5QTN0wCM0AzNzEzW}
```

### References:
none

### Notes:
The current working directory matters for relative paths.
A relative path is any path that does not start at root (i.e., it does not start with /).
A relative path is interpreted relative to your current working directory (cwd).
Your cwd is the directory that your prompt is currently located at.
