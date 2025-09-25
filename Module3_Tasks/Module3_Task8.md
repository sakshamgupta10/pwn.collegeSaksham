# Challenge Name: removing files
In this challenge we will learn how to delete files using rm command.
## My solve
**Flag:** 'pwn.college{M5eJqpVJHFLSrVVMVO1D2caUg5t.QX2kDM1wiN0AzNzEzW}'
```bash
hacker@commands~removing-files:~$ touch PWN
hacker@commands~removing-files:~$ touch COLLEGE
hacker@commands~removing-files:~$ ls
COLLEGE  PWN  f
hacker@commands~removing-files:~$ rm PWN
hacker@commands~removing-files:~$ ls
COLLEGE  f
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{M5eJqpVJHFLSrVVMVO1D2caUg5t.QX2kDM1wiN0AzNzEzW}
```

I showed my solve before.
My thought process: We can delete files using the rm command.
It is quite simple, we just write rm and then write the file name we want to delete, then we delete a file.

## What I learned
I learnt how to delete files using the rm command.
## References
The information given to us in the pwn.college website.
