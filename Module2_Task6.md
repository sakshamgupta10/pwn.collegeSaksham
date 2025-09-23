# Challenge Name: Implcit relative paths, from /
In this challenge we learnt the use of relative paths and how they are different from actual paths.
## My solve
**Flag:** 'pwn.college{4ftvhum7HKPcx9RFMX8yF-S9wUB.QX3QTN0wiN0AzNzEzW}'
```bash
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ /challenge/run
Incorrect...
You invoked this challenge with an absolute path. This challenge needs a relative path!
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{cLRk93wK4rrWK6HxXpWiOP8umIw.QX5QTN0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: I understood the difference between actual path and relative path and how relative path does not start with any root.I understood that how I specify a particular file, depends on where the terminal prompt is located.




## What I learned
I learned that a relative path is any path that does not start at root (i.e., it does not start with /). A relative path is interpreted relative to my current working directory (cwd).
My cwd is the directory that your prompt is currently located at.
## References
The information given to us in the pwn.college website.
