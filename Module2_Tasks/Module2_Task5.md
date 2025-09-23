# Challenge Name: Position yet Elsewhere
In this challenge we learn that we can navigate around directories by using the cd command.

## My solve
**Flag:** 'pwn.college{UutNZWWilU04MU2J-X_-7uUfK7I.QX4QTN0wiN0AzNzEzW}'

```bash
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /
hacker@paths~position-yet-elsewhere:/$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{UutNZWWilU04MU2J-X_-7uUfK7I.QX4QTN0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: I understood that using the cd command we can change directories and did the same then used cd to change from ~ to /.
## What I learned
I learned how to change directories using the cd command and that each process has a directory in which it's currently hanging out. 
## References
The information given to us in the pwn.college website.
