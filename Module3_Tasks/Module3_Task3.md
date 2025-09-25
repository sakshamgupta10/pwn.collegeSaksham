# Challenge Name: more catting practice 
In this challenge we will learn how to specify all sorts of paths as arguements to commands and practice more cat.
## My solve
**Flag:** 'pwn.college{UzHbPkulSftfmZzIkuEFQPcb4LO.QXwITO0wiN0AzNzEzW}'
```bash
You cannot use the 'cd' command in this level, and must retrieve the flag by
absolute path. Plus, I hid the flag in a different directory! You can find it
in the file /usr/share/nodejs/flag. Go cat it out **without** cding into that
directory!
hacker@commands~more-catting-practice:~$ cat /usr/share/nodejs/flag
pwn.college{UzHbPkulSftfmZzIkuEFQPcb4LO.QXwITO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: Retrieving the flag without using cd was bit tricky but using cat command instead of cd helped.

## What I learned
I learnt that we can use cat instead of cd to change directories. 
## References
The information given to us in the pwn.college website.
