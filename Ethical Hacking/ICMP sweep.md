- nmap command = nmap -PE IP address(of the target machine)
- Packet send is ICMP request type 8 and received ICMP echo packet is type 0
- If no reply means host is down
- can only be used by root user
- To use ICMP sweep we have to disable arp ping to do so command is = 
	- nmap -PE IP address --disable-arp-ping
- By default it also scans some common ports , to check only the host is alive or not without scanning port = nmap -PE -sn IP address.