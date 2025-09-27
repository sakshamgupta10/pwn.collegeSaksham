# Challenge Name: Exclusionary Globbing
In this challenge we learn how to filter out files in a glob.
## My solve
**Flag:** 'pwn.college{oEwrmdS16oOh7zVrFCvb3cY8wlj.QX2IDO0wiN0AzNzEzW}'
```bash
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{oEwrmdS16oOh7zVrFCvb3cY8wlj.QX2IDO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: We understand how to filter out files in a glob.
If the first character in the brackets is a ! or a ^, the glob inverts, and that bracket instance matches characters that aren't listed.
## What I learned
I learnt how to filter out files in a glob.
## References
The information given to us in the pwn.college website.
