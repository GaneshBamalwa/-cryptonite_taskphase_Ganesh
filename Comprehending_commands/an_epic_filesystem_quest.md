# CTF Challenge: an epic filesystem quest

## Table of Content

- commands-executed: , ls -a , ls , cd , cd ../ , cat
- flag :pwn.college{8lKWOnDWVnnBF-sAQl3NZ9zBnxf.dljM4QDLzETN0czW}



### Output:
```console
hacker@commands~an-epic-filesystem-quest:~$ cd ../../
hacker@commands~an-epic-filesystem-quest:/$ ls
README  challenge  flag  lib32   media  opt   run   sys  var
bin     dev        home  lib64   mnt    proc  sbin  tmp
boot    etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ cat README 
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/openid/server/__pycache__
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/lib/python3/dist-packages/openid/server/__pycache__
cat: /usr/lib/python3/dist-packages/openid/server/__pycache__: Is a directory
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/lib/python3/dist-packages/openid/server/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/openid/server/__pycache__$ ls
BLUEPRINT                server.cpython-38.pyc
__init__.cpython-38.pyc  trustroot.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/openid/server/__pycache__$ cat BLUEPRINT 
Great sleuthing!
The next clue is in: /usr/local/lib/python3.8/dist-packages/networkx/drawing/tests/__pycache__

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/openid/server/__pycache__$ cd /usr/local/lib/python3.8/dist-packages/networkx/drawing/tests/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/networkx/drawing/tests/__pycache__$ ls -a
.      __init__.cpython-38.pyc     test_layout.cpython-38.pyc
..     test_agraph.cpython-38.pyc  test_pydot.cpython-38.pyc
.GIST  test_latex.cpython-38.pyc   test_pylab.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/networkx/drawing/tests/__pycache__$ cat .GIST 
Lucky listing!
The next clue is in: /opt/aflplusplus/qemu_mode/qemuafl/hw/ipack

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/networkx/drawing/tests/__pycache__$ cd /opt/aflplusplus/qemu_mode/qemuafl/hw/ipack
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/hw/ipack$ ls
Kconfig  MEMO  ipack.c  meson.build  tpci200.c
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/hw/ipack$ cat MEMO
Lucky listing!
The next clue is in: /opt/linux/linux-5.4/Documentation/driver-api/i3c

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/hw/ipack$ ls /opt/linux/linux-5.4/Documentation/driver-api/i3c
NOTE-TRAPPED           index.rst              protocol.rst
device-driver-api.rst  master-driver-api.rst
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/hw/ipack$ cat /opt/linux/linux-5.4/Documentation/driver-api/i3c/NOTE-TRAPPED 
Yahaha, you found me!
The next clue is in: /usr/share/icons/Adwaita/24x24

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/qemu_mode/qemuafl/hw/ipack$ cd /usr/share/icons/Adwaita/24x24
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Adwaita/24x24$ ls
actions  apps  devices  emblems  emotes  legacy  mimetypes  status  ui
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Adwaita/24x24$ ls -a
.   .SPOILER  apps     emblems  legacy     status
..  actions   devices  emotes   mimetypes  ui
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Adwaita/24x24$ cat .SPOILER 
Tubular find!
The next clue is in: /opt/linux/linux-5.4/drivers/scsi/libfc

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Adwaita/24x24$ CD /opt/linux/linux-5.4/drivers/scsi/libfc
bash: CD: command not found
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Adwaita/24x24$ cd /opt/linux/linux-5.4/drivers/scsi/libfc
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/scsi/libfc$ ls -a
.  ..  .BRIEF  Makefile  fc_disc.c  fc_elsct.c  fc_exch.c  fc_fcp.c  fc_frame.c  fc_libfc.c  fc_libfc.h  fc_lport.c  fc_npiv.c  fc_rport.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/scsi/libfc$ cat .BRIEF 
Tubular find!
The next clue is in: /usr/lib/python3/dist-packages/jedi/third_party/typeshed/stdlib/2/multiprocessing
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/scsi/libfc$ ls /usr/lib/python3/dist-packages/jedi/third_party/typeshed/stdlib/2/multiprocessing
WHISPER  __init__.pyi  dummy  pool.pyi  process.pyi  util.pyi
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/scsi/libfc$ 
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/scsi/libfc$ cat /usr/lib/python3/dist-packages/jedi/third_party/typeshed/stdlib/2/multiprocessing/WHISPER 
Lucky listing!
The next clue is in: /usr/share/emacs/26.3/etc/images/gnus

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/scsi/libfc$ cd /usr/share/emacs/26.3/etc/images/gnus
hacker@commands~an-epic-filesystem-quest:/usr/share/emacs/26.3/etc/images/gnus$ ls
CLUE                exit-gnus.pbm  get-news.pbm      gnus.xbm        mail-send.pbm  preview.xbm   rot13.pbm      toggle-subscription.pbm  uu-post.pbm
README              exit-gnus.xpm  get-news.xpm      gnus.xpm        mail-send.xpm  preview.xpm   rot13.xpm      toggle-subscription.xpm  uu-post.xpm
catchup.pbm         exit-summ.pbm  gnntg.pbm         important.pbm   next-ur.pbm    receipt.pbm   save-aif.pbm   unimportant.pbm
catchup.xpm         exit-summ.xpm  gnntg.xpm         important.xpm   next-ur.xpm    receipt.xpm   save-aif.xpm   unimportant.xpm
cu-exit.pbm         followup.pbm   gnus-pointer.xbm  kill-group.pbm  post.pbm       reply-wo.pbm  save-art.pbm   unsubscribe.pbm
cu-exit.xpm         followup.xpm   gnus-pointer.xpm  kill-group.xpm  post.xpm       reply-wo.xpm  save-art.xpm   unsubscribe.xpm
describe-group.pbm  fuwo.pbm       gnus.png          mail-reply.pbm  prev-ur.pbm    reply.pbm     subscribe.pbm  uu-decode.pbm
describe-group.xpm  fuwo.xpm       gnus.svg          mail-reply.xpm  prev-ur.xpm    reply.xpm     subscribe.xpm  uu-decode.xpm
hacker@commands~an-epic-filesystem-quest:/usr/share/emacs/26.3/etc/images/gnus$ cat CLUE
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{8lKWOnDWVnnBF-sAQl3NZ9zBnxf.dljM4QDLzETN0czW}
```

