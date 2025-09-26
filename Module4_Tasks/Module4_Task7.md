# Challenge Name: Helpful for Builtins 
In this challenge we will learn about builtin commands .
## My solve
**Flag:** 'pwn.college{A-LG6yKXKwS_WgtTqPmWaUpFfLX.QX0ETO0wiN0AzNzEzW}'
```bash
hacker@man~help-for-builtins:~$ help cd
cd: cd [-L|[-P [-e]] [-@]] [dir]
    Change the shell working directory.

    Change the current directory to DIR.  The default DIR is the value of the
    HOME shell variable. If DIR is "-", it is converted to $OLDPWD.

    The variable CDPATH defines the search path for the directory containing
    DIR.  Alternative directory names in CDPATH are separated by a colon (:).
    A null directory name is the same as the current directory.  If DIR begins
    with a slash (/), then CDPATH is not used.

    If the directory is not found, and the shell option `cdable_vars' is set,
    the word is assumed to be  a variable name.  If that variable has a value,
    its value is used for DIR.

    Options:
      -L        force symbolic links to be followed: resolve symbolic
                links in DIR after processing instances of `..'
      -P        use the physical directory structure without following
                symbolic links: resolve symbolic links in DIR before
                processing instances of `..'
      -e        if the -P option is supplied, and the current working
                directory cannot be determined successfully, exit with
                a non-zero status
      -@        on systems that support it, present a file with extended
                attributes as a directory containing the file attributes

    The default is to follow symbolic links, as if `-L' were specified.
    `..' is processed by removing the immediately previous pathname component
    back to a slash or the beginning of DIR.

    Exit Status:
    Returns 0 if the directory is changed, and if $PWD is set successfully when
    -P is used; non-zero otherwise.
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "A-LG6yKX".
hacker@man~help-for-builtins:~$ /challenge/challenge --A-LG6yKX
bash: /challenge/challenge: No such file or directory
hacker@man~help-for-builtins:~$ challenge --secret A-LG6yKX
Correct! Here is your flag!
pwn.college{A-LG6yKXKwS_WgtTqPmWaUpFfLX.QX0ETO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: We understand the usage of builtin commands.
Like I wrote builtin cd, builtin challenge; then I saw what happened and understood.

## What I learned
I learnt how to use builtin commands.
## References
The information given to us in the pwn.college website.
