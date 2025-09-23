# Challenge Name: Position Thy Self
In this challenge we learn that we can navigate around directories by using the cd command.
**Flag:** 'pwn.college{YnTubinMieqirCyAdrom-QRfXwm.QX2QTN0wiN0AzNzEzW}'
```bash
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /sys/kernel directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /sys/kernel
hacker@paths~position-thy-self:/sys/kernel$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{YnTubinMieqirCyAdrom-QRfXwm.QX2QTN0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: I understood that using the cd command we can change directories and did the same.
## What I learned
I learned how to change directories using the cd command.
## References
The information given to us in the pwn.college website.
