# Challenge Name: Matching with *
In this challenge we will learn what * is.
## My solve
**Flag:** 'pwn.college{YQUyHQi2p_RhQX_5Zf4fDg7pJkn.QXxIDO0wiN0AzNzEzW}'
```bash
hacker@globbing~matching-with-:~$ cd /c*
hacker@globbing~matching-with-:/challenge$ ./run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{YQUyHQi2p_RhQX_5Zf4fDg7pJkn.QXxIDO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: We understand how to use the * glob and what it does.
When it encounters a * character in any argument, the shell will treat it as a "wildcard" and try to replace that argument with any files that match the pattern. 

## What I learned
I learnt how to use the * glob.
## References
The information given to us in the pwn.college website.
