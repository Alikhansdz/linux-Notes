when You run  "ls -l" it gives detailed information about the files 
and directories, it print like this
 "-rwxr-xr-x 1 ali it 1024 Jun 29 notes.txt"
-rwxr-xr-x
││  |  │
││  │  └── Others' permissionsr(r-x)
││  └──── Group permissions(r-x)
│└────── Owner permissions(rwx)
└──────── File type(-)

also the values used to assign permission ,
 ie read =4,write =2 ,execute =1 total=4+2+1 =7 (rwx)
so if you want to give all permision to owner,groups,and other 
use chmod777 here first 7(4+2+1) gives (rwx) permissions  to owner
the second 7 gives (rwx) permissions to groups ,and the last 7 gives
(rwx) permission to others

chmod = Changes the permissions of a file or directory.

example= chmod+w example.txt

chmod+x = Adds the execute permission.

example= chmod+x ai.txt

chmod755 = Sets permissions using numeric (octal) notation.

example= chmod755 ali.txt (gives rwx permissions to the fil owner
r-x to groups and otheres because of 5 (4+1 rx))

chown = change owner if the file

example= sudo  chown ali  alimarks.txt

chgrp = Changes the group owner of a file or directory.

example= chgrp developeres alimemo.txt

id = Displays information about the current or specified user.

example= uid=1000(ali) gid=1000(ali) groups=1000(ali),27(sudo),100(users)

{Meaning:
uid = User ID  gid = Primary Group ID
 groups = All groups the user belongs to }

whoami = Displays the current logged-in username.

example=whoami 

groups = Displays all groups the current user belongs to.

example= groups      result = ali sudo docker
Meaning:

ali → Primary group
sudo → Can use sudo to perform administrative tasks
docker → Can manage Docker without root privileges
