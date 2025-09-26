# Challenge Name: Searching for Manuals 
In this challenge we will learn how to search through a hidden manual.
## My solve
**Flag:** 'pwn.college{YLjm5zL0MUZaZkOZVs04m8fvhoK.QX2EDO0wiN0AzNzEzW}'
```bash
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k challenge
jmzaksmfvh (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man jmzaksmfvh
hacker@man~searching-for-manuals:~$ /challenge/challenge --jmzaks 500
Correct usage! Your flag: pwn.college{YLjm5zL0MUZaZkOZVs04m8fvhoK.QX2EDO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: We understand how to search through a hidden manual using man man command.

## What I learned
I learnt how to search through a hidden manual.
## References
The information given to us in the pwn.college website.
