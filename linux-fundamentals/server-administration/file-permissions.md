# File Permissions

On a Linux operating system, each file and directory is assigned access permissions for the owner of the file, the members of a group of related users and everybody else. This is to make sure that one user is not allowed to access the files and resources of another user.

![](<../../.gitbook/assets/image (3).png>)

![](<../../.gitbook/assets/image (6).png>)

![](<../../.gitbook/assets/image (5) (1).png>)

#### Chmod command <a href="#chmod-command" id="chmod-command"></a>

The chmod command is used to modify files and directories permissions in Linux.

The chmod command accepts permissions in as a numerical argument. We can think of permission as a series of bits with 1 representing True or allowed and 0 representing False or not allowed.

| Permission              | rwx | Binary | Decimal |
| ----------------------- | --- | ------ | ------- |
| Read, write and execute | rwx | 111    | 7       |
| Read and write          | rw- | 110    | 6       |
| Read and execute        | r-x | 101    | 5       |
| Read only               | r-- | 100    | 4       |
| Write and execute       | -wx | 011    | 3       |
| Write only              | -w- | 010    | 2       |
| Execute only            | --x | 001    | 1       |
| None                    | --- | 000    | 0       |

Each digit is independent of the other two. Therefore, `750` means the current user can read, write, and execute, the group cannot write, and others cannot read, write, or execute.

`744`, which is a typical default permission, allows read, write, and execute permissions for the owner, and read permissions for the group and “world” users.

#### `664 => rw-rw-r--` <a href="#chmod-664-rw-rw-r" id="chmod-664-rw-rw-r"></a>

```
chmod 664 example.txt
```

\
**Chown command**

The chown command is used to change the owner of files or directories in Linux.

Command syntax: chown \\\<new\_owner> \\\<file\_name>

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image6.png)

**Chgrp command**

The chgrp command can be used to change the group ownership of files or directories in Linux. The syntax is very similar to that of chown command.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image27.png)

Chgrp command can also be used to change the owner of a directory in the similar way.\
\
