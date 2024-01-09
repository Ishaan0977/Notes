# Packet Switching

- ### Modern form of long distance data communication.
	- Network resources are ==not dedicated==.
	- A link ==can be shared==.
- ### The basic technology has evolved over time but the basic concept has remained the same.
- ### Data transmitted in short packets (Kbytes).
	- A longer message is broken up into smaller ==Chunks==.
	- The ==Chunks are called Packets==.
	- Every packet contains a header
		- Which contains relevant information for routing , etc.


![[pasted image 0.png]]


- ### Packet switching is based on store-and-forward concept.
	- Each intermediate network node receives a whole packet.
	- Decides the route.
	- Forwards the packet along the selected route.
- Each intermediate note(router) maintains a ==routing table==.

## ==Advantages== :

- ### Links can be shared ; so link utilization is better.
- ### Suitable for computer-generated(bursty) traffic.
- ### Buffering and data rate conversion can be performed easily.
- ### Some packets may be given priority over others, if desired.

## How are packets Transmitted ?

### Two alternative approaches :

### [[Virtual Circuits]]
### [[Datagram Approach]]