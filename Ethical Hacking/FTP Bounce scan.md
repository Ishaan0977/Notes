- It connevts a FTP server , adn establishs a control connection , and ask the FTP server to intiate an active data transfer process\
- command = nmap -b IP(target) IP(client)
	- By default username is anonymous and password is wwwuser@
- -v means verbose for more details
- To provide password nmap -v(for more details) -b username:password@IP (target) IP (client)