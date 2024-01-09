# Datagram Approach

- ## Basic Concept :
	- No route is established beforehand.
	- Each ==packet== is transmitted as a ==independent entity==.
	- Does ==not maintain any history==.
- ## Analogy :
	- Postal System.
- ## Every intermediate node has to take routing decisions by dynamically.
	- Makes ==use of routing table==.
	- Every packet must contain source and destination addresses.
	- Duplicate packets may also be generated.

- ## Advantages :
	- Faster than virtual circuit for smaller number of packets.
		- ==No routing establishment and termination==.
	- More flexible.
	- Packets between two hosts may follow different paths.
		- ==Can handle congestion/failed link sometimes==.

# Datagram Packet Switching
- ### No initial delay.
- ### The packets are send out independently.
	- May follow different paths
	- Also follows store-and-forward approach.
