# Virtual Circuit Approach

- ### Similar in concept of [[Circuit Switching]] .
	- A route is established before packet transmission is start.
	- All packet follows the same path.
	- The links compromising the path are not dedicated ; ==Different from circuit switching in this aspect==.
- ## Analogy 
	- Telephone system. 

## How it ==works==?
- Route is established prior.
- Packet forwarded from one node to the next using store-and-forward scheme.
- Only the virtual circuit number need to be carried by a packet
	- Each intermediate node maintains a table.
	- Created during route establishment.
	- used for packet forwarding.
- No dynamic routing decision is taken by the intermediate route.