# Challenge Name: Helpful Programs 
In this challenge we will learn how to run programs without man page using --help arguement.
## My solve
**Flag:** 'pwn.college{Un0pRyxpUOQVaKkTXOvgYSk1PjK.QX3IDO0wiN0AzNzEzW}'
```bash
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 13
hacker@man~helpful-programs:~$ /challenge/challenge -g 13
Correct usage! Your flag: pwn.college{Un0pRyxpUOQVaKkTXOvgYSk1PjK.QX3IDO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: We understand how to run programs without man page using --help arguement.

## What I learned
I learnt how to run programs using --help arguement.
## References
The information given to us in the pwn.college website.
