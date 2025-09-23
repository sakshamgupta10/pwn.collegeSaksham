# Challenge Name: home sweet home
In this challenge we will learn that our shell session will start with your home directory as your current working directory.
## My solve
**Flag:** 'pwn.college{UApuOVC3hMsWP_dIwLzjqa_yS-C.QXzMDO0wiN0AzNzEzW}'
```bash
hacker@paths~home-sweet-home:/challenge$ cd /challenge
hacker@paths~home-sweet-home:/challenge$ ./run
You must provide an argument to /challenge/run when you invoke it!
hacker@paths~home-sweet-home:/challenge$ cd temp
bash: cd: temp: No such file or directory
hacker@paths~home-sweet-home:/challenge$ cd tmp
bash: cd: tmp: No such file or directory
hacker@paths~home-sweet-home:/challenge$ cd /tmp
hacker@paths~home-sweet-home:/tmp$ /challenge/run ~/f
Writing the file to /home/hacker/f!
... and reading it back to you:
pwn.college{UApuOVC3hMsWP_dIwLzjqa_yS-C.QXzMDO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: When I read that every user has a home directory, I connected it with what I’d seen earlier in Linux — that /home usually holds all user folders. Since I’m logged in as hacker, I realized my personal space must be /home/hacker. 

## What I learned
I learnt every user has a home directory, typically under /home in the filesystem and that the home directory is typically where users store most of their personal files.
## References
The information given to us in the pwn.college website.
