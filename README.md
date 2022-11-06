# Startup-Management-init.d-in-DevOps

The first process of Linux system is (init.d) which is a daemon. A daemon is a program that runs continuously as a background process and wakes up to handle periodic service requests, which often come from remote processes. Daemons run silently in the background to monitor and take care of certain subsystems to ensure that the operating system runs properly. A printer daemon monitors and takes care of printing services. A network daemon monitors and maintains network communications, and so on. 

In case of for our unix systems httpd, inetd, sshd etc are daemons that are running and whose status can be checked and changed from time to time. This repo will have startup managemenet through init.d. I'm using centos 7 using Oracle VM VirtualBox


Being a system process the init belongs to the system configuration directory folder as shown below:

![image](https://user-images.githubusercontent.com/97732099/200176105-883b15ce-8436-423f-83ea-97383fb3bd03.png)


Above you'll see the init.d folder which contains all the programs running in the back which affect functioning of the system.
When we get into this directory of init.d then what we see is that it only contains a function file which is responsible for starting & stopping various functions that are happening in the background.

![image](https://user-images.githubusercontent.com/97732099/200176169-d4ae5aa7-d957-436d-a612-65819b5793f5.png)


Now when we wish to start a service then:
> service [service_name] [action]

However if you wish to start the htptd service using the service command then an error will occur:

![image](https://user-images.githubusercontent.com/97732099/200176221-45d23878-9d00-4059-9bfa-9d94ba84c6df.png)

It is because service command is used for very basic functionalities of the system, for a service like httpd systemctl command is used.

![image](https://user-images.githubusercontent.com/97732099/200037195-55b1aabe-4a09-4b5e-94e4-5e49010ab9a2.png)



# Service-Management-in-DevOps
systemd is a System Management Daemon which replaces the sysvinit process to become the first process with PID = 1, which gets executed in user space during the Linux start-up process. It is a system that is designed specifically for the Linux kernel. It is now being used as a replacement of init.d to overcome shortcomings of it. 

As shown above systemctl is used to enable, start, stop, kill or to check the status of a daemon (program running in behind). Its command format is,

> systemctl start [service-name], $ systemctl poweroff
Examples:

> systemctl status httpd
Systemctl checks whether the service/process httpd is running or not.

![image](https://user-images.githubusercontent.com/97732099/200176649-fa7747a8-8567-47d4-a66e-63419181636b.png)

> systemctl enable httpd
Systemctl enables the service/process httpd to be able to work with.

![image](https://user-images.githubusercontent.com/97732099/200176702-5af3d40d-1dd0-465a-92c0-d2fbce3e9c13.png)

> systemctl start httpd
Systemctl starts the service/process httpd.

![image](https://user-images.githubusercontent.com/97732099/200176757-c18b7b20-f8e7-4a4d-b903-a43c04734c84.png)


> systemctl status httpd
Now if you again check the status of httpd, then it appears as running actice as compared to previous status shown above.

![image](https://user-images.githubusercontent.com/97732099/200176843-cb6d1d27-3136-42f3-929c-2e6b88a636f9.png)






# Virtualization-in-DevOps







# Memory_Storage-&-File_System-in-DevOps





