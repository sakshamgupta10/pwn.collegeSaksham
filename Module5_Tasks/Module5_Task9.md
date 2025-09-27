# Challenge Name: Multiple Options for Tab Completion
In this challenge we learn what happens varies based on the specific shell and its options when there are multiple options.

## My solve
**Flag:** 'pwn.college{kMRuyAqtrgFNjuLeKMIK4pAm-s4.0lN0EzNxwiN0AzNzEzW}'
```bash
hacker@globbing~multiple-options-for-tab-completion:~$ ls
No ls for you in this level! Use tab-completion instead!
hacker@globbing~multiple-options-for-tab-completion:~$ cd /challenge/files
hacker@globbing~multiple-options-for-tab-completion:/challenge/files$ cat pwncollege/p
cat: pwncollege/p: No such file or directory
hacker@globbing~multiple-options-for-tab-completion:/challenge/files$ cat pwncollege/p-
cat: pwncollege/p-: No such file or directory
hacker@globbing~multiple-options-for-tab-completion:/challenge/files$ ls
No ls for you in this level! Use tab-completion instead!
hacker@globbing~multiple-options-for-tab-completion:/challenge/files$ bash
hack-the-planet        pwn-college            pwncollege-family      pwncollege-flamingo    pwncollege-hacking
pwn                    pwn-the-planet         pwncollege-flag        pwncollege-flyswatter
hacker@globbing~multiple-options-for-tab-completion:/challenge/files$ cat pwncollege-flag
pwn.college{kMRuyAqtrgFNjuLeKMIK4pAm-s4.0lN0EzNxwiN0AzNzEzW}
```

I showed my solve before.
My thought process: We understand how to use bash and use tab.

## What I learned
I learnt how to use tab.
## References
The information given to us in the pwn.college website.
