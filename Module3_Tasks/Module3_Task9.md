# Challenge Name: moving files
In this challenge we will learn how to move files using mv command.
## My solve
**Flag:** 'pwn.college{MMqtT36noB-qUBZL7tTy2u10jyR.0VOxEzNxwiN0AzNzEzW}'
```bash
hacker@commands~moving-files:~$ ls
COLLEGE  f
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{MMqtT36noB-qUBZL7tTy2u10jyR.0VOxEzNxwiN0AzNzEzW}
```

I showed my solve before.
My thought process: We can move files using the mv command.
It is quite simple, we just write mv and then write the file name we want to move and then after a space write what file we want to move it to and it gets moved.

## What I learned
I learnt how to move files using the mv command.
## References
The information given to us in the pwn.college website.
