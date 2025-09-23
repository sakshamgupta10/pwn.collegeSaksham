# Challenge Name: Explicit relative paths, from /
In this challenge we learnt the use of relative paths and how they are different from actual paths.
## My solve
**Flag:** 'pwn.college{INiuIwGryvOlIR4AZUSiV5xJdSt.QXwUTN0wiN0AzNzEzW}'
```bash
hacker@paths~explicit-relative-paths-from-:/$ cd /
hacker@paths~explicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{INiuIwGryvOlIR4AZUSiV5xJdSt.QXwUTN0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: Previously our relative it directly specified the directory to descend into from the current directory, but here I am going to explore more explicit relative paths.


## What I learned
I learned that in most operating systems, every directory has two implicit entries that you can reference in paths: . and ... The first, ., refers right to the same directory, so the following absolute paths are all identical to each other.
## References
The information given to us in the pwn.college website.
