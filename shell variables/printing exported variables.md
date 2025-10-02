# Printing exported variables
Try the env command: it'll print out every exported variable set in your shell, and you can look through that output to find the FLAG variable

## Solution
Used env command to get flag.

```sh
Connected!
hacker@variables~printing-exported-variables:~$ env
SHELL=/run/dojo/bin/bash
HOSTNAME=variables~printing-exported-variables
PWD=/home/hacker
MANPATH=/run/dojo/share/man:
DOJO_AUTH_TOKEN=139bdc7bdd8fe3e8b10279aa1d70538c483cf7940082b9afcbb865582663c1e8
HOME=/home/hacker
LANG=C.UTF-8
FLAG=pwn.college{wqC-hqZftjEjomFSxlQ_rBGxmHm.QX4UTN0wCM0AzNzEzW}
TERMINFO=/run/dojo/share/terminfo
TERM=xterm-256color
SHLVL=2
LC_CTYPE=C.UTF-8
SSL_CERT_FILE=/run/dojo/etc/ssl/certs/ca-bundle.crt
PATH=/run/challenge/bin:/run/dojo/bin:/root/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
DEBIAN_FRONTEND=noninteractive
_=/run/dojo/bin/env
```

## Flag: 

```
pwn.college{wqC-hqZftjEjomFSxlQ_rBGxmHm.QX4UTN0wCM0AzNzEzW}
```

### References:
none

### Notes:
env command prints out every exported variable set in your shell.
