# Architecture

![](<../.gitbook/assets/image (3) (1).png>)



* The Linux kernel is monolithic in nature.
* System calls are used to interact with the Linux kernel space.
* Kernel code can only be executed in the kernel mode. Non-kernel code is executed in the user mode.
* Device drivers are used to communicate with the hardware devices.
