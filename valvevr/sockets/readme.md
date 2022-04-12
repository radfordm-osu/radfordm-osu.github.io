#Sockets
Sockets are used for the controlled placement of objects.

##Sockets
	Sockets have several public values, including:
		- HoldingSocketable: Whether the socket is currently in use.
		- _sawBoardSocket: Whether the socket is for Sawable Boards.
- AllowedObjectType: The type of object to accept in the socket. If not set, any socketable can be used.
- AttachTransform: A transform that the socketable will be snapped to. If not set, the socketable will float in place
##Socketables
For an object to be socketable, Socketable.cs or a similar script must be put on the object. An object that is already in a socket cannot be put directly into another, but can be taken out of one and then put into the other.

##Board Socket
Board sockets are sockets that only let boards snap into them. To be defined as a board socket, the object with the Socketable.cs script must be named SawBoardSocket or SawBoardSocket (X), where X is a number. These are used in the saw objects.

##Nail Socket
Nail sockets are sockets that only allow nails to be put into them. These are used when making an object that a user will be nailing together. This could also be adapted for screws in the future.

##Hat Socket
The hat socket is on a user’s head. Only hat objects can be placed here.
