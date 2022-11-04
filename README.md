# Startup-Management-init.d-in-DevOps

The first process of Linux system is (init.d) which is a daemon. A daemon is a program that runs continuously as a background process and wakes up to handle periodic service requests, which often come from remote processes. Daemons run silently in the background to monitor and take care of certain subsystems to ensure that the operating system runs properly. A printer daemon monitors and takes care of printing services. A network daemon monitors and maintains network communications, and so on. 

In case of for our unix systems httpd, inetd, sshd etc are daemons that are running and whose status can be checked and changed from time to time. This repo will have startup managemenet through init.d. I'm using centos 7 using Oracle VM VirtualBox




init.d is a daemon which is the first process of the Linux system.


Then other processes, services, daemons, and threads are started by init. One can write their own scripts in '/etc/init.d' location to start services automatically on system boot. Services can be started and stopped manually by using service command.







