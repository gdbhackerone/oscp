#OSCP

OSCP Preparation 

Day 0 </br>
From HTB Starting Point Machines - Tier 0 Machines - Meow
We are not discussing answer to the machines but what knowledge one should have after he solved the machine.

#How to connect via openvpn to HTB,
via linux terminal
via windows openvpn program

#Things one should know or learn in the process
installing VirtualBox/VMWare

Networking
#Machines have unique IP Address (on same network atleast)
there are different interfaces through which a machine can connect to other machines/internet
like on Linux eth0 wlan0 tun0 which stands for Ethernet Wireless-LAN, tunnel respectively
when we connect via OpenVPN, a tun0 can be seen in ifconfig output in terminal


#How can one know if device is reachable ?
ping it,
ping can help verify if the device is responding to ICMP packets

That was about just knowing if it's alive/responding to ICMP/ or reachable

#what if you want to know more about what services running on machine/ or ports accepting connection and responding.
nmap - NMAP can help one to check required/all ports on mahcine if they are open/closed/filtered.

#it will always be helpful if one remembers some common ports around
there are normally* two types well-known ports, and others
#0-1023 port numbers are used by system process/ or definite process/ or process that dont usually change and are common on each system.
beyond 1023, i.e. 1024 - 65535 are utilized by various process as required and defined by system administrators


#One can do nmap scan on a machine and know by open ports which services are running in most of the cases,
sometimes scan needs to be extended beyond 1000 ports to discover more services and know the unknown.

So to sum it up
things one should learn nicely before jumping to machine 2 of starting point machines on HTB
-What are IP Address,
-What are ports in computer and how they work, common port numbers
-how to verify machine state by ping
-how does ping work, 
-what it means if you get ping response
-which layer in OSI does ping works
-what is ICMP and where it is used
-what are OSI layers in network and how they differ from TCP/IP Layers
-What is OpenVPN and how does it works
-how can you connect via openVPN, what are the ways on  Linux and Windows or Mac machines
-Installing/configuring Virtual Machines using VirtualBox/VMWare or any other Hypervisor Platform
-Installing/configuring an Operating System, one should know how Windows/Linux is installed normally.
-Know some common Linux and Windows commands to read navigate delete list files and service status 
-nmap - know various switches what they do, -sC -sV -sT -A ... and more, we will talk about this more..
-Tools of trade - ping, ifconfig, cat, ls, cd,hostname, nmap
