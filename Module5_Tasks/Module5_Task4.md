# Challenge Name: Matching paths with []
In this challenge we will further learn what [] can do.
## My solve
**Flag:** 'pwn.college{gtZ0qEzw0SFYqxviXHcIqSUDMcZ.QX0IDO0wiN0AzNzEzW}'
```bash
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[absh]
You got it! Here is your flag!
pwn.college{gtZ0qEzw0SFYqxviXHcIqSUDMcZ.QX0IDO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: We understand how to use the [] glob further and what it does.
The square brackets are, essentially, a limited form of ?, in that instead of matching any character, [] is a wildcard for some subset of potential characters, specified within the brackets.

## What I learned
I learnt how to use the [] glob and how it works. I also learnt that globbing happens on a path basis, so we can expand entire paths with our globbed arguments.
## References
The information given to us in the pwn.college website.
