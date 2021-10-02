# awk command

- Print the fifth column (a.k.a. field) in a space-separated file:
   awk '{print $5}' {{filename}}
- Print the second column of the lines containing "foo" in a space-separated file:
   awk '/{{foo}}/ {print $2}' {{filename}}

- Print the last column of each line in a file, using a comma (instead of space) as a field separator:
   awk -F ',' '{print $NF}' {{filename}}

- Print every third line starting from the first line:
   awk 'NR%3==1' {{filename}}


# example print the first output
$ id                   
uid=1000(liu) gid=1000(liu) groups=1000(liu),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),116(lpadmin),126(sambashare),999(docker)

divide it by space

$ id | awk '{print $1}'
uid=1000(liu)