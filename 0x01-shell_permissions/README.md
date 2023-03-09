Task 0. script that switches the current user to the user betty : su betty
Task 1. script that prints the effective username of the current user : whoami
Task 2 Groups. script that prints all the groups the current user is part of : groups
Task 3 New owner. script that changes the owner of the file hello to the user betty : chown betty hello
Task 4 Empty!.  script that creates an empty file called hello : touch hello
Task 5 Execute. script that adds execute permission to the owner of the file hello: chmod u+x hello
Task 6 Multiple permissions.Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello : chmod ug+x,o+r  hello 
Task 7 Everybody!. script that adds execution permission to the owner, the group owner and the other users, to the file hello : chmod ugo+x
Task 8 James Bond. Write a script that sets the permission to the file hello as follows
Owner: no permission at all
Group: no permission at all
Other users: all the permissions
:chmod ug-rwx,o+rwx hello
Task 9 John Doe.Write a script that sets the mode of the file hello to this -rwxr-x-wx: chmod 753
Task 10 Look in the mirror.Write a script that sets the mode of the file hello the same as olleh’s mode
The file hello will be in the working directory
The file olleh will be in the working directory
:chmod --reference=olleh hello
