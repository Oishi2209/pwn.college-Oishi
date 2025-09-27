# Filesystem quest
In this challenge, I have hidden the flag! Here, you will use ls and cat to follow my breadcrumbs and find it

## Solution
Used cd to enter / directory. Then used ls command to see contents. Used cat to look into any suspicious files. Then followed through on each step as instructed.

```sh
Connected!
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
BLUEPRINT  bin  boot  challenge  dev  etc  flag  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
hacker@commands~an-epic-filesystem-quest:/$ cat BLUEPRINT
Lucky listing!
The next clue is in: /usr/share/icons/ubuntu-mono-light/stock/32

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/icons/ubuntu-mono-light/stock/32
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/ubuntu-mono-light/stock/32$ ls
LEAD
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/ubuntu-mono-light/stock/32$ cat LEAD
Great sleuthing!
The next clue is in: /opt/linux/linux-5.4/arch/nios2

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/ubuntu-mono-light/stock/32$ cd /opt/linux/linux-5.4/arch/nios2
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/nios2$ ls
EVIDENCE  Kconfig  Kconfig.debug  Makefile  boot  configs  include  kernel  lib  mm  platform
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/nios2$ cat EVIDENCE
Lucky listing!
The next clue is in: /usr/share/perl/5.30.0/File

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/nios2$ cd /usr/share/perl/5.30.0/File
hacker@commands~an-epic-filesystem-quest:/usr/share/perl/5.30.0/File$ ls
Basename.pm  Compare.pm  Copy.pm  Fetch.pm  Find.pm  GlobMapper.pm  INFO  Path.pm  Temp.pm  stat.pm
hacker@commands~an-epic-filesystem-quest:/usr/share/perl/5.30.0/File$ cat INFO
Tubular find!
The next clue is in: /usr/share/doc/git/contrib/git-shell-commands

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/perl/5.30.0/File$ ls -la /usr/share/doc/git/contrib/git-shell-commands
total 28
drwxr-xr-x 1 root   root   4096 Sep 27 11:47 .
drwxr-xr-x 1 root   root   4096 Sep 26 17:07 ..
-rw-r--r-- 1 root   root    839 Feb 17  2020 README
-rw-r--r-- 1 hacker hacker   75 Sep 27 11:47 TIP-TRAPPED
-rw-r--r-- 1 root   root    283 Feb 17  2020 help
-rw-r--r-- 1 root   root    227 Feb 17  2020 list
hacker@commands~an-epic-filesystem-quest:/usr/share/perl/5.30.0/File$ cat /usr/share/doc/git/contrib/git-shell-commands/README
Sample programs callable through git-shell.  Place a directory named
'git-shell-commands' in the home directory of a user whose shell is
git-shell.  Then anyone logging in as that user will be able to run
executables in the 'git-shell-commands' directory.

Provided commands:

help: Prints out the names of available commands.  When run
interactively, git-shell will automatically run 'help' on startup,
provided it exists.

list: Displays any bare repository whose name ends with ".git" under
user's home directory.  No other git repositories are visible,
although they might be clonable through git-shell.  'list' is designed
to minimize the number of calls to git that must be made in finding
available repositories; if your setup has additional repositories that
should be user-discoverable, you may wish to modify 'list'
accordingly.
hacker@commands~an-epic-filesystem-quest:/usr/share/perl/5.30.0/File$ ls /usr/share/doc/git/contrib/git-shell-commands
README  TIP-TRAPPED  help  list
hacker@commands~an-epic-filesystem-quest:/usr/share/perl/5.30.0/File$ ls /usr/share/doc/git/contrib/git-shell-commands/TIP-TRAPPED
/usr/share/doc/git/contrib/git-shell-commands/TIP-TRAPPED
hacker@commands~an-epic-filesystem-quest:/usr/share/perl/5.30.0/File$ cat /usr/share/doc/git/contrib/git-shell-commands/TIP-TRAPPED
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/include/linux/can
hacker@commands~an-epic-filesystem-quest:/usr/share/perl/5.30.0/File$ cd /opt/linux/linux-5.4/include/linux/can
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/linux/can$ ls
NOTE  can-ml.h  core.h  dev  dev.h  led.h  platform  rx-offload.h  skb.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/linux/can$ cat NOTE
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/LICENSES/deprecated

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/include/linux/can$ cd /opt/linux/linux-5.4/LICENSES/deprecated
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/LICENSES/deprecated$ ls .a
ls: cannot access '.a': No such file or directory
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/LICENSES/deprecated$ ls -a
.  ..  .GIST  GPL-1.0  ISC  Linux-OpenIB  X11
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/LICENSES/deprecated$ cat .GIST
Lucky listing!
The next clue is in: /usr/lib/x86_64-linux-gnu/perl5/5.30/auto/Text/Iconv
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/LICENSES/deprecated$ cd /usr/lib/x86_64-linux-gnu/perl5/5.30/auto/Text/Iconv
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl5/5.30/auto/Text/Iconv$ ls
Iconv.so  POINTER  autosplit.ix
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl5/5.30/auto/Text/Iconv$ cat POINTER
Lucky listing!
The next clue is in: /usr/share/doc/libicu66

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl5/5.30/auto/Text/Iconv$ ls /usr/share/doc/libicu66
ALERT-TRAPPED  changelog.Debian.gz  copyright
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl5/5.30/auto/Text/Iconv$ cat /usr/share/doc/libicu66/ALERT-TRAPPED
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{EBdVzuiAz9ilxYQnis5LnQQBlDI.QX5IDO0wCM0AzNzEzW}

```

## Flag: 

```
pwn.college{EBdVzuiAz9ilxYQnis5LnQQBlDI.QX5IDO0wCM0AzNzEzW}
```

### References:
none

### Notes:
Patience.
