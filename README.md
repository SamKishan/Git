# Git
By Sampreet Kishana
The file contains the configuration for CISCO ASA 5506.
The following VLANs were created
  DMZ
  PRODUCTION
  EMPLOYEE
  BYOD
Web server was started in the DMZ network. Port forwarding from the web server (ports 80,443, and 22) to the Internet. 
Hosts on all VLANs were given Internet access.

Firewall (ACL) rules
  DMZ can be reached from all Internal networks but cannot initiate traffic to internal networks.
  Production can be reached from empployee and BYOD
  BYOD cannot be reached from anywhere but has internet access.
  
DOCKER 
  A docker web server container that would alert the user they are trying to access a malicious web site. 
 
PROTECTION AGAINST MALWARE 
  IDS (Snort) on Web server. 
  ACLs on the ASA (Router)
  
  
