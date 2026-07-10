groupadd     -> Adds a new group.
Example: sudo groupadd developers

groupdel     -> Deletes an existing group.
Example: sudo groupdel developers

groups       -> Displays the groups a user belongs to.
Example: groups
         groups ali

newgrp       -> Switches to a different group for the current session.
Example: newgrp developers

gpasswd      -> Manages group members and group passwords.
Example: sudo gpasswd -a ali developers
         sudo gpasswd -d ali developers

groupmod     -> Modifies an existing group.
Example: sudo groupmod -n programmers developers

getent group -> Displays group information from the system database.
Example: getent group
         getent group developers

id -Gn       -> Displays the names of the groups the current user belongs to.
Example: id -Gn

chgrp        -> Changes the group owner of a file or directory.
Example: sudo chgrp developers report.txt

sudo         -> Executes a command with administrator (root) privileges.
Example: sudo apt update
         sudo useradd ali

