# Server Administration

### Multi-User Operating Systems <a href="#multi-user-operating-systems" id="multi-user-operating-systems"></a>

An operating system is considered as multi-user if it allows multiple people/users to use a computer and not affect each other's files and preferences. Linux based operating systems are multi-user in nature.

### User/Group Management <a href="#usergroup-management" id="usergroup-management"></a>

* Users in Linux has an associated user ID called UID attached to them.
* A group is a collection of one or more users.&#x20;
* A group makes it easier to share permissions among a group of users.
* Each group has a group ID called GID associated with it.

#### id command <a href="#id-command" id="id-command"></a>

`id` command can be used to find the uid and gid associated with an user. It also lists down the groups to which the user belongs to.

The uid and gid associated with the root user is 0. ![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image30.png)

A good way to find out the current user in Linux is to use the whoami command.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image35.png)

**"root" user or superuser is the most privileged user with** **unrestricted access to all the resources on the system. It has UID 0**\


Important files associated with users/groups

| /etc/passwd | Stores the user name, the uid, the gid, the home directory, the login shell etc |
| ----------- | ------------------------------------------------------------------------------- |
| /etc/shadow | Stores the password associated with the users                                   |
| /etc/group  | Stores information about different groups on the system                         |
