# ChatServer
***
#### _{Implementing a chat server in Python. There are two main components, the clients and the server. The server will be started before the clients. Using TCP sockets for communication. The server uses a TCP server socket, whereas the clients use TCP clients.}_

## Tools/Technologies Used
* Python
* TCP Sockets

## Description
_{The clients should have the following features:

Upon startup, request the server's IP address and port from the user. Attempt to join to that server. 
When a message is received from the server, print it out.
Help command. Syntax: /help
This command should print out a list of all supported commands and their behaviors
Users command. Syntax /users
This command should request a list of users from the server and then print out their names.
Direct Message command. Syntax: /dm username "message"
This command should send the message between quotes to the specified user. The client will make the request to the server.
Broadcast command. Syntax: /bc "message"
This command should send the message between quotes to all other connected users. The client will make the request to the server.
Quit command. Syntax: /quit
Disconnect from the server. Before disconnecting, send a message to the server saying you will disconnect.
The server should have the following features:

When a client tries to join, assign it a name. All messages from that IP will be marked with the given name. Names should be unique and can be simple (e.g., User 1, User 2, etc.).
When a dm request is received, send the message to the user, if any. Display an error if the name does not exist. Only the sender and the receiver should see the message.
When a bc request is received, send the message to all connected users.
When a users request is received, send a list of all users to the interested client only.
When a disconnect message is received, tell all connected users that the specified client is quitting.
If a client disconnects without sending the disconnect message, tell all connected users that the specified client has lost its connection.

Example:

Client 1:
/dm client2 "Hello there!" \
client1: Hello there! \
client2: Hello!

Client 2:
client1: Hello there! \
/bc "Hello!" \
client2: Hello!

Client 3:
client2: Hello! \
/dm client4 "Goodbye." \
server: User "client4" is not connected to the server.}_

## References
* (https://docs.oracle.com/javase/tutorial/networking/sockets/definition.html)
* (https://www.edureka.co/blog/socket-programming-python/)
* (https://www.youtube.com/watch?v=ytu2yV3Gn1I&t=19s)
* (https://www.youtube.com/watch?v=CV7_stUWvBQ&t=363s)
