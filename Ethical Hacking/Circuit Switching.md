# Circuit Switching

- ### A ==dedicated communication== path is established between two stations.
	- The path follows a ==fixed sequence of intermediate links==.
	- A logical channel gets dedicated on each physical link for connection.
- ### After initial circuit establishment , data bits sent continuously without any delay.

![[Screenshot (53) 1.png]]

- ### Three steps are required for communication.
	1. Connection establishment
		1. required before data transmission.
	2. Data transfer
		1. Can proceed at maximum speed.
	3. Connection termination
		1. Required after data transmission is over.
		2. For deallocation of network resources.

## ==Drawbacks== :

- ### Channel capacity is dedicated during the entire duration of communication.
	- Acceptable for voice communication.
	- Vey inefficient for bursty traffic like data.
- ### There is a initial delay
	- For connection establishment.
