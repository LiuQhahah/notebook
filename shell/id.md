# id command

Display current user and group identity.More information: https://www.gnu.org/software/coreutils/id.

 - Display current user's ID (UID), group ID (GID) and groups to which they belong:
   id

 - Display the current user identity as a number:
   id -u

 - Display the current group identity as a number:
   id -g

 - Display an arbitrary user's ID (UID), group ID (GID) and groups to which they belong:
   id {{username}}

# example user VS root
$ id    
uid=1000(liu) gid=1000(liu) groups=1000(liu),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),116(lpadmin),126(sambashare),999(docker)

root@Honor:~# id
uid=0(root) gid=0(root) groups=0(root)

root id is 0