# 0x01. Shell, permissions
## Resources
### Read
* [Permissions](http://linuxcommand.org/lc3_lts0090.php)

### man or help:
`chmod`, `sudo`, `su`, `chown`, `chgrp`, `id`, `groups`, `whoami`, `adduser`, `useradd`, `addgroup`
## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:
### Permissions
* What do the commands `chmod`, `sudo`, `su`, `chown`, `chgrp` do
* Linux file permissions
* How to represent each of the three sets of permissions (owner, group, and other) as a single digit
* How to change permissions, owner and group of a file
* Why can’t a normal user `chown` a file
* How to run a command with root privileges

How to change user ID or become superuser
### Other Man Pages
* How to create a user
* How to create a group
* How to print real and effective user and group IDs
* How to print the groups a user is in
* How to print the effective userid

## Requirements
* Allowed editors: `vi`, `vim`, `emacs`
* Linux
* All your scripts should be exactly two lines long (`$ wc -l file` should print 2)
* The first line of all your files should be exactly `#!/bin/bash`
* You are not allowed to use backticks, `&&`, `||` or `;`
* All your files must be executable
## Tasks
#### 0. [My name is Betty](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/0-hello_world)
Create a script that switches the current user to the user `betty`.

* You should use exactly 8 characters for your command (+1 character for the new line)
* You can assume that the user `betty` will exist when we will run your script
#### 1. [Who am I](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/1-confused_smiley)
Write a script that prints the effective username of the current user.
#### 2. [Groups](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/2-hellofile)
Write a script that prints all the groups the current user is part of.
#### 3. [New owner](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/3-twofiles)
Write a script that changes the owner of the file `hello` to the user `betty`.
#### 4. [Empty!](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/4-lastlines)
Write a script that creates an empty file called `hello`.
#### 5. [Execute](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/5-firstlines)
Write a script that adds execute permission to the owner of the file `hello`.

* The file `hello` will be in the working directory
#### 6. [Multiple permissions](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/6-third_line)
Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file `hello`.

* The file `hello` will be in the working directory
#### 7. [Everybody!](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/7-file)
Write a script that adds execution permission to the owner, the group owner and the other users, to the file `hello`

* The file `hello` will be in the working directory
* You are not allowed to use commas for this script
#### 8. [James Bond](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/8-cwd_state)
Write a script that sets the permission to the file `hello` as follows:

* Owner: no permission at all
* Group: no permission at all
* Other users: all the permissions
The file `hello` will be in the working directory You are not allowed to use commas for this script
#### 9. [John Doe](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/9-duplicate_last_line)
Write a script that sets the mode of the file `hello` to this:

`-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello`
* The file `hello` will be in the working directory
* You are not allowed to use commas for this script
#### 10. [Look in the mirror](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/10-no_more_js)
Write a script that sets the mode of the file `hello` the same as `olleh`’s mode.

* The file `hello` will be in the working directory
* The file `olleh` will be in the working directory
#### 11. [Directories](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/11-directories)
Create a script that adds execute permission to all subdirectories of the **current directory** for the owner, the group owner and all other users.

Regular files should not be changed.
#### 12. [More directories](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/12-newest_files)
Create a script that creates a directory called `my_dir` with permissions 751 in the working directory.
#### 13. [Change group](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/13-unique)
Write a script that changes the group owner to `school` for the file `hello`

* The file `hello` will be in the working directory
#### 14. [Owner and group](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/14-findthatword)
Write a script that changes the owner to `vincent` and the group owner to `staff` for all the files and directories in the working directory.
#### 15. [Symbolic links](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/15-countthatword)
Write a script that changes the owner and the group owner of `_hello` to `vincent` and `staff` respectively.

* The file `_hello` is in the working directory
* The file `_hello` is a symbolic link
#### 16. [What's next?](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/16-whatsnext)
Write a script that changes the owner of the file `hello` to `betty` only if it is owned by the user `guillaume`.

* The file hello will be in the working directory
#### 17. [Star Wars](https://github.com/najlae01/alx-system_engineering-devops/blob/main/0x02-shell_redirections/17-hidethisword)
Write a script that will play the StarWars IV episode in the terminal.
