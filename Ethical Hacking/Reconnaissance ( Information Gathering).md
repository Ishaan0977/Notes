- It is the process of collecting as much information as possible about a target network .
	- Required for identifying ways to intrude into an organization's/Victim's network system.
	- It is the first step before mounting any attack.
- We collect useful information about the target PC
	- Such as IP address , list of open ports , vulnerability etc.

### Objective of Reconnaissance
- Collect Network information
	- Domain name , IP addresses , Internal Domain name , services running (TCP,UDP).
- Collect system information
	- User names , routing tables, System names , system architecture , password etc.

### Types of Reconnaissance
a. Passive Reconnaissance
b. Active Reconnaissance

### [[Passive Reconnaissance]]
- In this type of information gathering we collect information about the target indirectly.
	- without direct communication with the target system.
	- collection of the data that are publically available for webpage/application.
	- we can collect information using archive.org , Whois , netcraft and harvester tools.
	- we can also use search engine and search operators available in search engine.

### [[Active Reconnaissance]](D:\Github\Notes\Notes\Ethical Hacking\Active Reconnaissance)
- In this type of information gathering we collect information directly by communicating with victim system
	- can provide more detailed information about the target machine  . but as we directly communicating with the target machine there is also risk of detection.
	- can be carried out using network mapper ([[NMAP]]), Nessus , metasploit framework etc.
	- we can also use mail tracker and DNS enumeration etc.
### Proxy chaining 
- work as intermediary for connecting with victim system
- to hide the source IP address
- fake source address of the proxy
- IP spoofing can also be used.
- Proxy chain available under ==/etc/proxychain4.conf== we can open it with any text editor
- in that file many methods are available such as ==dynamic proxy , strict proxy chain , random proxy chain and round robin proxy chain==
- remove the hash from the option we want to use 
- also from the DNS server to change the location  of DNS server
