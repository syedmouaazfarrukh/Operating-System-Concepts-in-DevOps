# Startup-Management-init.d-in-DevOps

The first process of Linux system is (init.d) which is a daemon. A daemon is a program that runs continuously as a background process and wakes up to handle periodic service requests, which often come from remote processes. Daemons run silently in the background to monitor and take care of certain subsystems to ensure that the operating system runs properly. A printer daemon monitors and takes care of printing services. A network daemon monitors and maintains network communications, and so on. 

In case of for our unix systems httpd, inetd, sshd etc are daemons that are running and whose status can be checked and changed from time to time. This repo will have startup managemenet through init.d. I'm using centos 7 using Oracle VM VirtualBox


Being a system process the init belongs to the system configuration directory folder as shown below:

![image](https://user-images.githubusercontent.com/97732099/200034014-230c4e68-9aba-4c9b-b773-0c7f89ef7979.png)
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




# Virtualization-in-DevOps




# Memory_Storage-&-File_System-in-DevOps





