# Challenge Name: catting absolute paths
In this challenge we will learn how to specify cat's arguments as absolute paths:
## My solve
**Flag:** 'pwn.college{I-oiqsv7NZtt50H7QJZ37K9kuH8.QX5ETO0wiN0AzNzEzW}'
```bash
hacker@commands~catting-absolute-paths:~$ cat /flag
pwn.college{I-oiqsv7NZtt50H7QJZ37K9kuH8.QX5ETO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: Since we can read the home directory with cat command at its absolute path: /flag we will not copy it to our home directory but will make it readable.

## What I learned
I learnt that we can specify cat's arguments as absolute paths. 
## References
The information given to us in the pwn.college website.
