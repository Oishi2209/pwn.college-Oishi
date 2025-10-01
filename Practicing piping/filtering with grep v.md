# Filtering with grep v
Use grep -v to filter out all the lines containing "DECOY" and reveal the real flag!

## Solution
Used //challenge/run | grep -v DECOY to get the flag.

```sh
Connected!
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{gJSq5io6qn1dil2zaZo206UgsZB.0FOxEzNxwCM0AzNzEzW}
```

## Flag: 

```
pwn.college{gJSq5io6qn1dil2zaZo206UgsZB.0FOxEzNxwCM0AzNzEzW}
```

### References:
none

### Notes:
The grep command has a very useful option: -v (invert match). While normal grep shows lines that MATCH a pattern, grep -v shows lines that do NOT match a pattern:
