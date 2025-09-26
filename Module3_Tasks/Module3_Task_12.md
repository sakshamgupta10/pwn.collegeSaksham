# Challenge Name: making directories
In this challenge we will learn how to make directories using the mkdir command.
## My solve
**Flag:** 'pwn.college{g2a69ZR56tb6FrqTWWyl-oMUHzU.QXxMDO0wiN0AzNzEzW}'
```bash
hacker@commands~making-directories:~$ mkdir /tmp/pwn
mkdir: cannot create directory ‘/tmp/pwn’: File exists
hacker@commands~making-directories:~$ touch /tmp/pwn/college
touch: cannot touch '/tmp/pwn/college': Not a directory
hacker@commands~making-directories:~$ rm /tmp/pwn
hacker@commands~making-directories:~$ mkdir /tmp/pwn
hacker@commands~making-directories:~$ touch /tmp/pwn/college
hacker@commands~making-directories:~$ /challenge/run
Success! Here is your flag:
pwn.college{g2a69ZR56tb6FrqTWWyl-oMUHzU.QXxMDO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: We can make directories using the mkdir command.
It is quite simple, we just write mkdir, then our directory name and then the directory is created.

## What I learned
I learnt how to create directories using the mkdir command.
## References
The information given to us in the pwn.college website.
