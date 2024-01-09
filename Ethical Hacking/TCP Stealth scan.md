- Carry out port scanning while avoiding detection
- Try to hide themselves among normal network traffic
- not to be logged (stealth)
#### How it works ?
- Flag probe packets also known as Inverse Mapping
	- Response is sent back only by closed port
	- Intruder determines what services do not exist , and can infer the only one that exists.
	- Slow scan rate
- -sS option is used
- If port is open it ignores if it is close it sends RST packet