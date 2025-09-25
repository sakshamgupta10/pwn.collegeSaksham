# Challenge Name: comparing files
In this challenge we will learn that the diff compares two files line by line and shows you exactly what's different between them.
## My solve
**Flag:** 'pwn.college{4WR58TQCKSLWz_40Qev6ai1EZ_B.01MwMDOxwiN0AzNzEzW}'
```bash
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
78a79
> pwn.college{4WR58TQCKSLWz_40Qev6ai1EZ_B.01MwMDOxwiN0AzNzEzW}
```

I showed my solve before.
My thought process: The diff commands basically shows me the difference between 2 files.
I use the diff command and write the file names after that with a space in between the file names and then see the difference.

## What I learned
I learnt how to use the diff command when we look for changes between files.  
## References
The information given to us in the pwn.college website.
