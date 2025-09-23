# Challenge Name: Position Elsewhere
In this challenge we learn that we can navigate around directories by using the cd command.

## My solve
**Flag:** 'pwn.college{4ftvhum7HKPcx9RFMX8yF-S9wUB.QX3QTN0wiN0AzNzEzW}'
```bash
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/zoneinfo/posix/Asia directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /usr/share/zoneinfo/posix/Asia
hacker@paths~position-elsewhere:/usr/share/zoneinfo/posix/Asia$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{4ftvhum7HKPcx9RFMX8yF-S9wUB.QX3QTN0wiN0AzNzEzW}
hacker@paths~position-elsewhere:/usr/share/zoneinfo/posix/Asia$
```

I showed my solve before.
My thought process: I understood that using the cd command we can change directories and did the same.
## What I learned
I learned how to change directories using the cd command and that each process has a directory in which it's currently hanging out. I also learnt the ~ prompt shows the current path that my shell is located at.
## References
The information given to us in the pwn.college website.
