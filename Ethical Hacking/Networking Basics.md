# Networking : Basic Concepts

## What is a ==computer network== ?

A communication system for ==connecting computer/hosts==.
- Better connectivity.
- Better communication.
- Better ==sharing of resources==.
- Bring people together.

## ==Types== of computer network :

- ### Local Area Network (LAN) :
	- Connects hosts within a relatively small geographical area.
		- ==Faster.==
		- ==Cheaper.==
- ### Wide Area Network :
	- Hosts maybe widely dispersed across campuses , cities , countries.
		- ==Slower==.
		- ==Expensive==.

## Data communication over a network :
- ###  [[Circuit Switching]]
- ### [[Packet Switching]]

## Type of ==delays== :

### 1. Propagation delay :-
- Time take by a data signal to propagate from one node to other.
### 2. Transmission delay :-
- Time taken by the transmitter to send out a packet.
### 3. Processing delay :-
- Time taken by a node to process a packet.

# Layered Network Architecture

- ### [[Open Systems Interconnection (OSI) Reference Model]]
	- Seven layer Model.
	- Communication functions are partitioned into a hierarchical set of layers.
- ### Objective :-
	- Systematic approach to design.
	- Changes in one layer should not require changes in other layers.
- ### [[TCP-IP]]
![[Screenshot (71) 1.png]]

# Internetworking devices :-
- ### Hub
	- Extends the span of a single LAN.
	- Broadcasts messages to every node.
- ### Bridge/Layer 2 switch
	- Connects two or more LAN's together.
	- Works at data link layer level.
- ### Router/Layer 3 switch
	- Connects any combination of LAN's and WAN's.
	- Works at network layer level.

# What does IP do?
- ### IP transports datagram (packets) from a source node to a destination node.
	- Responsible for routing the packets.
	- Breaks a packet into smaller packets , if required.
	- Unreliable service
		- A packet may be lost in transit.
		- Packets may arrive out of order.
		- Duplicate packets may be generated.

# What does TCP do?
- ### TCP provides a connection-oriented , reliable service for sending messages.
	- Split a message into packets.
	- Reassemble packets at destination.
	- Resend packets that were lost in transit.
- ### Interface with IP :
	- Each packet forwarded to IP for delivery.
	- Error control is done by TCP.

# What does UDP do?
- ### UDP provides a connectionless , unreliable service for sending datagrams (packets).
	- Messages small enough to fit in a packet (eg: DNS query).
	- Simpler (and faster) than TCP.
	- Never split data into multiple packets.
	- Does not care about error control.
- ### Interface with IP :
	- Each UDP packet sent to IP for delivery.

# Addresses in TCP/IP
![[Screenshot (73).png]]

# Encapsulation
- ### Basic Concept :
	- As data flows down the protocol hierarchy , headers ( and trailers ) get appended to it.
	- As data moves up the hierarchy , headers ( and trailers ) get stripped off.
- ### Example
	- Client wants to send 200 bytes of data 4 bytes of TFTP header gets added
![[Screenshot (74).png]]

# ![[IP Layer]]
