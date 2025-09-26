# Challenge Name: Learning Complex Usage
In this challenge we will learn how to print arbitrary files to the terminal.
## My solve
**Flag:** 'pwn.college{0z7l8t33UH9MsaOvjdfGulGkAab.QX1ITO0wiN0AzNzEzW}'
```bash
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /challenge/flag
Correct argument! Here is the /challenge/flag file:
cat: /challenge/flag: No such file or directory
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /challenge/flag
Correct argument! Here is the /challenge/flag file:
cat: /challenge/flag: No such file or directory
hacker@man~learning-complex-usage:~$ ls -la /challenge/
total 20
drwxr-xr-x 1 root root 4096 Sep 26 12:56 .
drwxr-xr-x 1 root root 4096 Sep 26 12:57 ..
-rwsr-xr-x 1 root root   74 Jan 14  2025 .init
-rwsr-xr-x 1 root root 1115 Sep  1 05:06 DESCRIPTION.md
-rws--x--x 1 root root  475 Jan 14  2025 challenge
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /challennge/.init
Correct argument! Here is the /challennge/.init file:
cat: /challennge/.init: No such file or directory
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{0z7l8t33UH9MsaOvjdfGulGkAab.QX1ITO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: We understand how to print arbitrary files to the terminal.

## What I learned
I learnt how to print arbitrary files to the terminal.
## References
The information given to us in the pwn.college website.

