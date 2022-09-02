This readme file contains a description of the actions of the content of the commands contained in the files. NB: the first line of each script/file contains The shebang, #!/bin/bash which when used in scripts instruct the operating system to use bash as a command interpreter. The texts within the inverted commas "" are the contents of each specified file.
0-iam_betty "su betty" switches the current user to the user betty
1-who_am_i "whoami" prints the user name of the user
2-groups "groups" prints all the groups the current user is part of
3-new_owner "sudo chown betty hello" chenges the owner of the file hello to the user betty
4-empty "touch hello" creats an empty file hello
5-execute "chmod u+x hello" adds execute permission to the owner of the file hello. The file hello is in the working directory
6-multiple_permissions "chmod u+x,g+x,o+r hello" adds execute permission to the owner and the group owner, and read permission to other users, to the file hello. The file hello is in the working directory
7-everybody "chmod a+x hello" The file hello is in the working directory. INSTRUCTION:You're not allowed to use commas for this script
8-James_Bond "chmod 007 hello" sets the permission to the file hello as follows: Owner = no permission at all, Group = no permission at all, Others users = all the permissions. The file hello is in the working directory INSTRUCTION:You're not allowed to use commas for this script
9-John_Doe "chmod 753 hello" sets the mode of the file hello to this: -rwxr-x-wx The file hello is in the working directory INSTRUCTION:You're not allowed to use commas for this script
10-mirror_permissions " chmod --reference=olleh hello" sets the mode of the file hello the same as olleh’s mode. The file hello will be in the working directory. The file olleh will be in the working directory. Note: the mode of olleh will not always be 664. Make sure your script works for any mode.
11-directories_permissions "chmod a+X *" adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.
12-directory_permissions "mkdir -m 751 my_dir" creates a directory called my_dir with permissions 751 in the working directory
13-change_group "chmod school hello" Write a script that changes the group owner to school for the file hello. The file hello will be in the working directory
