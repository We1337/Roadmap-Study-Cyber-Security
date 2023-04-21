In computer networking, a socket is a software abstraction that represents a communication endpoint. A socket allows an application to establish a network connection, send and receive data over the network, and close the connection when finished.

Sockets are typically used in client-server applications, where one application acts as the client and another application acts as the server. The client application creates a socket and uses it to connect to a specific IP address and port on the server. Once the connection is established, the client can send and receive data over the socket using various socket functions.

On the server side, the server application creates a socket and binds it to a specific IP address and port. The server then listens for incoming connections on the socket, accepting and processing each connection as it arrives.

Sockets are often implemented as an Application Programming Interface (API) that provides a set of functions for creating, connecting, and managing sockets. Examples of socket APIs include the Berkeley Sockets API used in Unix-like operating systems and the Windows Sockets API used in Microsoft Windows.

Sockets can be implemented using various network protocols, such as TCP, UDP, and raw IP. The protocol used by a socket determines how data is transmitted over the network, how errors are handled, and how connections are established and closed.