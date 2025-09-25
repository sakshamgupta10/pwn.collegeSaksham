# Challenge Name: An Epic Filesystem Quest
In this challenge we will test our knowledge by playing a game with our knowledge of cd,ls and cat commands.
## My solve
**Flag:** 'pwn.college{ojPvSh5TeGYLPDUtMWT-94HfB-B.QX5IDO0wiN0AzNzEzW}'
```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
MESSAGE  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin      challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat MESSAGE
Great sleuthing!
The next clue is in: /usr/share/racket/pkgs/htdp-lib/stepper/private/compiled

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/share/racket/pkgs/htdp-lib/stepper/private/compiled
TEASER                       lifting_rkt.dep         model_rkt.zo             shared_rkt.dep                   view-controller-typed_rkt.zo
annotate_rkt.dep             lifting_rkt.zo          mred-extensions_rkt.dep  shared_rkt.zo                    view-controller_rkt.dep
annotate_rkt.zo              macro-unwind_rkt.dep    mred-extensions_rkt.zo   syntax-hider_rkt.dep             view-controller_rkt.zo
beginner-defined_rkt.dep     macro-unwind_rkt.zo     my-macros_rkt.dep        syntax-hider_rkt.zo              xml-box_rkt.dep
beginner-defined_rkt.zo      marks_rkt.dep           my-macros_rkt.zo         syntax-property_rkt.dep          xml-box_rkt.zo
display-break-stuff_rkt.dep  marks_rkt.zo            reconstruct_rkt.dep      syntax-property_rkt.zo           xml-sig_rkt.dep
display-break-stuff_rkt.zo   model-settings_rkt.dep  reconstruct_rkt.zo       vertical-separator-snip_rkt.dep  xml-sig_rkt.zo
find-tag_rkt.dep             model-settings_rkt.zo   shared-typed_rkt.dep     vertical-separator-snip_rkt.zo   xml-snip-helpers_rkt.dep
find-tag_rkt.zo              model_rkt.dep           shared-typed_rkt.zo      view-controller-typed_rkt.dep    xml-snip-helpers_rkt.zo
hacker@commands~an-epic-filesystem-quest:/$ cat TEASER
cat: TEASER: No such file or directory
hacker@commands~an-epic-filesystem-quest:/$ cd TEASER
bash: cd: TEASER: No such file or directory
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/share/racket/pkgs/htdp-lib/stepper/private/compiled/TEASER
cat: /usr/share/racket/pkgs/htdp-lib/stepper/private/compiled/TEASER: Permission denied
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/racket/pkgs/htdp-lib/stepper/private/compiled
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/htdp-lib/stepper/private/compiled$ cat TEASER
Lucky listing!
The next clue is in: /usr/share/matplotlib/matplotlib.conf

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/htdp-lib/stepper/private/compiled$ ls  /usr/share/matplotlib/matplotlib.conf
INSIGHT-TRAPPED  matplotlibrc.template
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/htdp-lib/stepper/private/compiled$ cat  /usr/share/matplotlib/matplotlib.conf/INSIGHT-TRAPPED
Great sleuthing!
The next clue is in: /opt/busybox/busybox-1.33.2/include/config/feature/ip/route
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/htdp-lib/stepper/private/compiled$ cat /opt/busybox/busybox-1.33.2/include/config/feature/ip/route
cat: /opt/busybox/busybox-1.33.2/include/config/feature/ip/route: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/htdp-lib/stepper/private/compiled$ cd /opt/busybox/busybox-1.33.2/include/config/feature/ip/route
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/ip/route$ ls
TRACE  dir.h
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/ip/route$ cat TRACE
Congratulations, you found the clue!
The next clue is in: /usr/share/racket/collects/data/private/compiled

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/ip/route$ cd /usr/share/racket/collects/data/private/compiled
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/collects/data/private/compiled$ ls
WHISPER  count-bits-in-fixnum_rkt.dep  count-bits-in-fixnum_rkt.zo
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/collects/data/private/compiled$ cat WHISPER
Congratulations, you found the clue!
The next clue is in: /usr/aarch64-linux-gnu/bin

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/collects/data/private/compiled$ ls /usr/aarch64-linux-gnu/bin/WHISPER
ls: cannot access '/usr/aarch64-linux-gnu/bin/WHISPER': No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/collects/data/private/compiled$ ls /usr/aarch64-linux-gnu/bin
SECRET-TRAPPED  ar  as  ld  ld.bfd  ld.gold  nm  objcopy  objdump  ranlib  readelf  strip
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/collects/data/private/compiled$ cat SECRET-TRAPPED
cat: SECRET-TRAPPED: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/collects/data/private/compiled$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/aarch64-linux-gnu/bin/usr/aarch64-linux-gnu/bin
ls: cannot access '/usr/aarch64-linux-gnu/bin/usr/aarch64-linux-gnu/bin': No such file or directory
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/aarch64-linux-gnu/bin
SECRET-TRAPPED  ar  as  ld  ld.bfd  ld.gold  nm  objcopy  objdump  ranlib  readelf  strip
hacker@commands~an-epic-filesystem-quest:/$ cat SECRET-TRAPPED
cat: SECRET-TRAPPED: No such file or directory
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/aarch64-linux-gnu/bin/SECRET-TRAPPED
Yahaha, you found me!
The next clue is in: /usr/share/nmap

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/nmap
hacker@commands~an-epic-filesystem-quest:/usr/share/nmap$ ls
SPOILER            nmap-os-db     nmap-protocols  nmap-service-probes  nmap.dtd  nse_main.lua  scripts
nmap-mac-prefixes  nmap-payloads  nmap-rpc        nmap-services        nmap.xsl  nselib
hacker@commands~an-epic-filesystem-quest:/usr/share/nmap$ cat SPOILER
Great sleuthing!
The next clue is in: /usr/local/lib/python3.8/dist-packages/blinker/__pycache__

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/nmap$ ls -a /usr/local/lib/python3.8/dist-packages/blinker/__pycache__
.  ..  .README  __init__.cpython-38.pyc  _utilities.cpython-38.pyc  base.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/share/nmap$ cat /usr/local/lib/python3.8/dist-packages/blinker/__pycache__/.README
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/arch/xtensa/variants

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/nmap$ ls /opt/linux/linux-5.4/arch/xtensa/variants
BRIEF-TRAPPED  csp  dc232b  dc233c  de212  fsf  test_kc705_be  test_kc705_hifi  test_mmuhifi_c3
hacker@commands~an-epic-filesystem-quest:/usr/share/nmap$ cat /opt/linux/linux-5.4/arch/xtensa/variants/BRIEF-TRAPPED
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{ojPvSh5TeGYLPDUtMWT-94HfB-B.QX5IDO0wiN0AzNzEzW}
```

I showed my solve before.
My thought process: It was a long task but it helped me understand when do use certain commands like ls,cat,cd.

## What I learned
I learnt how to use commands like ls,cat,cd.

## References
The information given to us in the pwn.college website.
