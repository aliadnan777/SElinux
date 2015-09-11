# SElinux

* SELinux is an acronym for Security-enhanced Linux
* It is a security feature of the Linux kernel
* It is designed to protect the server against misconfigurations and/or compromised daemons
* It put limits and instructs server daemons or programs what files they can access and what actions they can take by defining a security policy
* SELinux is an implementation of a MAC(Mandatory Access Control) security mechanism
* It is built into the Linux kernel and enabled by default on Fedora, CentOS, RHEL and a few other Linux distributions
* SELinux allows server admin to define various permissions for all process
* It defines how all processes can interact with other parts of the server like pipes, files, network ports, sockets, directories, and many other processes
* SELinux puts restrictions on these objects according to the policy

### Example

* consider an apache user with full permission can only access /var/www/html directory, but can not touch other parts of the system such as /etc directory without policy modification. If an attacker managed to gain access to sendmail mail or apache web server, would only have access to exploited server and the files normally has access as defined in the policy for the server. An attacker can not access the other parts of the system or internal LAN. In other words, damage can be now restricted to the particular server and files. The cracker will not able to get a shell on your server via common daemons such as Apache /Sendmail
*  SELinux offers the following security features
   * Protect data of user from unauthorized access
   * Protect other daemons or programs from unauthorized access
   * Protect network ports / sockets / files from unauthorized access
   * Protect server against exploits
   * Avoid privilege and much more



