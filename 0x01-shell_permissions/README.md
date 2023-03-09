Task 0. script that switches the current user to the user betty : su betty
Task 1. script that prints the effective username of the current user : whoami
Task 2 Groups. script that prints all the groups the current user is part of : groups
Task 3 New owner. script that changes the owner of the file hello to the user betty : chown betty hello
Task 4 Empty!.  script that creates an empty file called hello : touch hello
Task 5 Execute. script that adds execute permission to the owner of the file hello: chmod u+x hello
Task 6 Multiple permissions.Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello : chmod ug+x,o+r  hello 
Task 7 Everybody!. script that adds execution permission to the owner, the group owner and the other users, to the file hello : chmod 755
