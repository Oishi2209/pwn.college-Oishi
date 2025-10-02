# Process substition for input
Now, you'll diff two sets of command outputs: /challenge/print_decoys, which will print a bunch of decoy flags, and /challenge/print_decoys_and_flag which will print those same decoys plus the real flag.
Use process substitution with diff to compare the outputs of these two programs and find your flag!

## Solution
Used diff <(/challenge/print_decoys_and_flag) <(/challenge/print_decoys) to get the flag.

```sh
Connected!
hacker@piping~process-substitution-for-input:~$ diff <( /challenge/print_decoys ) <( /challenge/print_decoys_and_flag )
75a76
> pwn.college{IQI6hIk2SVHXJBIJArNvgmzWzE5.0lNwMDOxwCM0AzNzEzW}
```

## Flag: 

```
pwn.college{IQI6hIk2SVHXJBIJArNvgmzWzE5.0lNwMDOxwCM0AzNzEzW}
```

### References:
none

### Notes:
For reading from a command (input process substitution), use <(command). When you write <(command), bash will run the command and hook up its output to a temporary file that it will create
