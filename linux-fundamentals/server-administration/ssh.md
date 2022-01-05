# SSH

The ssh command is used for logging into the remote systems, transfer files between systems and for executing commands on a remote machine. SSH stands for secure shell and is used to provide an encrypted secured connection between two hosts over an insecure network like the internet.

Reference: [https://www.ssh.com/ssh/command/](https://www.ssh.com/ssh/command/)

#### Passwordless Authentication Using SSH <a href="#passwordless-authentication-using-ssh" id="passwordless-authentication-using-ssh"></a>

Using this method, we can ssh into hosts without entering the password. This method is also useful when we want some scripts to perform ssh-related tasks.



Steps for setting up a passwordless authentication with a remote host:

1. Install openssh package which contains all the commands related to ssh.
2. Generate a key pair using the ssh-keygen command.
3. After running the ssh-keygen command successfully, we should see two keys present in the `~/.ssh` directory. `id_rsa` is the private key and `id_rsa.pub` is the public key. Do note that the private key can only be read and modified by you.
4. Transfer the public key to the remote host
   1. There are multiple ways to transfer the public key to the remote server. We will look at one of the most common ways of doing it using the ssh-copy-id command.
   2. Install the openssh-clients package to use ssh-copy-id command.
5. Our public key should be in `~/.ssh/authorized_keys` now.

`~/.ssh/authorized_key` contains a list of public keys. The users associated with these public keys have the ssh access into the remote host.

#### How to run commands on a remote host ? <a href="#how-to-run-commands-on-a-remote-host" id="how-to-run-commands-on-a-remote-host"></a>

General syntax: ssh \\\<user>@\\\<hostname/hostip> \\\<command>

#### How to transfer files from one host to another host ? <a href="#how-to-transfer-files-from-one-host-to-another-host" id="how-to-transfer-files-from-one-host-to-another-host"></a>

General syntax: scp \\\<source> \\\<destination>
