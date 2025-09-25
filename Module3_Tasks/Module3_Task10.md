# Challenge Name: hidden files
In this challenge we will see that ls does not list all files by default and we need to perform a different task to view these files.
## My solve
**Flag:** 'pwn.college{8olI-UmbCNpfmv2w1rHVFkm7DYX.QXwUDO0wiN0AzNzEzW}'
```bash
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls
bin  boot  challenge  dev  etc  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-232691168324343  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-232691168324343
pwn.college{8olI-UmbCNpfmv2w1rHVFkm7DYX.QXwUDO0wiN0AzNzEzW}
hacker@commands~hidden-files:/$
```

I showed my solve before.
My thought process: We can find hide files using the ls -a command.
It is quite simple, we just write ls -a and then we see the files which were hidden.

## What I learned
I learnt how to access the hidden files using the ls -a command.
## References
The information given to us in the pwn.college website.
