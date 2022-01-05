# Process Management

Some useful commands that can be used to monitor the processes on Linux systems.

#### ps (process status) <a href="#ps-process-status" id="ps-process-status"></a>

The ps command is used to know the information of a process or list of processes.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image24.png)

If you get an error "ps command not found" while running ps command, do install **procps** package.

ps without any arguments is not very useful. Let's try to list all the processes on the system by using the below command.

Reference: [https://unix.stackexchange.com/questions/106847/what-does-aux-mean-in-ps-aux](https://unix.stackexchange.com/questions/106847/what-does-aux-mean-in-ps-aux)

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image42.png)

We can use an additional argument with ps command to list the information about the process with a specific process ID.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image2.png)

We can use grep in combination with ps command to list only specific processes.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image1.png)

**top**

The top command is used to show information about Linux processes running on the system in real time. It also shows a summary of the system information.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image53.png)

For each process, top lists down the process ID, owner, priority, state, cpu utilization, memory utilization and much more information. It also lists down the memory utilization and cpu utilization of the system as a whole along with system uptime and cpu load average.\
\
**Memory Management**

In this section, we will study about some useful commands that can be used to view information about the system memory.

#### free <a href="#free" id="free"></a>

The free command is used to display the memory usage of the system. The command displays the total free and used space available in the RAM along with space occupied by the caches/buffers.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image22.png)

free command by default shows the memory usage in kilobytes. We can use an additional argument to get the data in human-readable format.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image5.png)

Checking Disk Space

In this section, we will study about some useful commands that can be used to view disk space on Linux.

#### df (disk free) <a href="#df-disk-free" id="df-disk-free"></a>

The df command is used to display the free and available space for each mounted file system.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image36.png)

#### du (disk usage) <a href="#du-disk-usage" id="du-disk-usage"></a>

The du command is used to display disk usage of files and directories on the system.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image10.png)

The below command can be used to display the top 5 largest directories in the root directory.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image18.png)

Systemd

Systemd is a system and service manager for Linux operating systems. Systemd units are the building blocks of systemd. These units are represented by unit configuration files.

The below examples shows the unit configuration files available at /usr/lib/systemd/system which are distributed by installed RPM packages. We are more interested in the configuration file that ends with service as these are service units.

![](https://linkedin.github.io/school-of-sre/level101/linux\_basics/images/linux/admin/image16.png)

#### Managing System Services <a href="#managing-system-services" id="managing-system-services"></a>

Service units end with .service file extension. Systemctl command can be used to start/stop/restart the services managed by systemd.

| Command                        | Description                           |
| ------------------------------ | ------------------------------------- |
| systemctl start name.service   | Starts a service                      |
| systemctl stop name.service    | Stops a service                       |
| systemctl restart name.service | Restarts a service                    |
| systemctl status name.service  | Check the status of a service         |
| systemctl reload name.service  | Reload the configuration of a service |

\
\
\
\
\
\
