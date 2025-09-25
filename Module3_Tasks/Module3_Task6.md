# Challenge Name: comparing files
In this challenge we will learn how to list the contents of files using the ls command.
## My solve
**Flag:** 'pwn.college{MhXaBXVURJ4U_AuPAf4Y2wGu6jA.QX4IDO0wiN0AzNzEzW}'
```bash
hacker@commands~listing-files:~$ ls /challenge
28335-renamed-run-16639  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/28335-renamed-run-16639
Yahaha, you found me! Here is your flag:
pwn.college{MhXaBXVURJ4U_AuPAf4Y2wGu6jA.QX4IDO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: The ls command will list files in all the directories provided to it as arguments, and in the current directory if no arguments are provided.
Directories can have lots of files (and other directories) inside them, and we won't always be here to tell you their names, hence we use ls.
## What I learned
I learnt how the ls command is helpful for listing files in directories.
## References
The information given to us in the pwn.college website.
