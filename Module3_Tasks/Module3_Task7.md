# Challenge Name: touching files
In this challenge we will learn how to create files using touch command.
## My solve
**Flag:** 'pwn.college{E8qhe5PpjhBH0zM0fIeFhStrL4a.QXwMDO0wiN0AzNzEzW}'
```bash
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ ls
bin  hsperfdata_root  tmp.TpSOPGOVKK
hacker@commands~touching-files:/tmp$ touch /tmp/pwn
hacker@commands~touching-files:/tmp$ touch /tmp/college
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.TpSOPGOVKK
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{E8qhe5PpjhBH0zM0fIeFhStrL4a.QXwMDO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: We can create files using the touch command.
It is quite simple, we just write touch and then write the file name we want, then we create a file.

## What I learned
I learnt how to create files using the touch command.
## References
The information given to us in the pwn.college website.
