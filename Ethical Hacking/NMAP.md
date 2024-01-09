- NMAP is a free , open source tool for vulnerability scanning and network discovery.
- Generic command to run NMAP on command prompt :
   nmap [scan types] [options] host or network
- The main features of nmap are :
	- Host discovery 
	- Port scanning
	- Service and version detection
	- OS detection

### Host Discovery
- To detect live host nmap queries multiple hosts , if it gets reply then target/host is marks as alive . This is known as Ping sweep operation.
- Host discovery are most commonly done using these following methods :
	- ICMP Echo
	- TCP syn ack
	- Time stamp packet
- Various host scan techniques are supported by NMAP :
	- [[ICMP sweep]]
	- [[Broadcast sweep]]
	- [[Non-echo ICMP]]
	- [[TCP sweep]]
	- [[UDP sweep]]
- Commands that use all types (except UDP sweep) are -sP , -sn, -sl , -Pn etc
| Command   | Full form              | Meaning                             |
| --------- | ---------------------- | ----------------------------------- |
| -sP       | Ping scan              | Only checks if host is alive or not |
| -sL       | List scan              | Simply lists targets to scan        |
| -PN       | Treat all hosts online | skips host discovery                |
| -PS/PA/PU |                        | TCP SYN / TCP ACK / UDP sweep       |
| -PE/PP/PM |                        | ICMP Echo / Timestamp / Subnet      |
| -PO       |                        | IP protocol ping                    |          |                        |                                     |

### Port Scanning
- Techniques
	- [[TCP Connect scan]]
	- [[TCP SYN scan]]
	- [[TCP Stealth scan]]
	- [[FTP Bounce scan]]
- some commands 
	- -F : fast mode , scans fewer ports then default
	- -r : scans ports consecutively (serial vise) not randomize
	- --top-ports (numbers): scan ( numbers) most common ports
- By ==default 1000 ports are scanned==.

### OS Detection
- ACK sending FIN|PSH|URG to a closed port
	- Most OS will return ACK with the same sequence number
	- but windows will return ACK packet with ACK+1
- Type of service probing with ICMP_Port_Unreachable message
	- Most OS will return TOS =0
	- Linux will return TOS = 0XC0
- commands for OS detection
	- -O
	- -a
	- --osscan-limit
	- --osscan-guess : Guess OS more aggressively

### Version detection
- sV : probe open ports to determine service/version info

### Script
- To list all the scripts of NMAP 
	- ls -al /usr/share/nmap/scripts/
- to find some specific script =  ls | grep "keyword"  
- to use script = --script=script_name.nse IP address  or --script script name IP address
- Some common scripts
	- ==smb-os== for ==os detection== . command =  Nmap-p445 --script smb-os-discovery IP address  if port 445 is closed then command is sudo Nmap-sU -sS --script smb-os-detection -p U:137, T:139 IP address 
	- to check any ==web sever== is running on target machine or not  command  nmap --script ==http-methods== IP  
	- ==port used is 80 (apache)==
	- to check ==anonymous ftp login== supported or not  nmap --script ==ftp-anon IP==  
	- ==port used port 21(ftp)  ==
	-  for ==ssh login credentials ssh-brute.nse== is used  
	- for ==system ID and pass smb-brute== is used
- To run default script command is -sC
- to edit any script we can use any editor such as leafpad and by using .nse extension
### Vulnerability scanning scripts
- ftp-vsftpd-backdoor.nse for checking ==backdoor available on ftp server==
-  http-slowloris-checek.nse Tests a ==web server== for vulnerability to the Slowloris ==DoS attack without actually launching a DoS attack==.
- ssh-brute.nse for brute forcing ==ssh credentials== 
	- port 22 should be open 
	- ssh service should be running
- smb-brute.nse for system credentials 
### Malware Scanning script
- nmap --script http-malware-host IP address
### Aggressive search
- For aggressive search command used is "-A".
- It checks Host up/down , open/close ports , Service version as well as Operating system.




