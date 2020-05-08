# Class 19 - Message Queues - 5/7/2020

## Real Time Message application with Socket.io
* Socket.io enables real-time and full duplex communication between the client and the web servers.
* The drawback of Real Time communication is that the clients will not receive missed out messages while they lose connection with the server because it doesn't track the delivery status of each event.

## Message Queues
* Routing events and messaging between clients.
  * Any connected client can 'publish' a message into the server.
  * Any connected client can 'subscribe' to receive message by type.
* See which clients are connected, to which Queues they are attached and further, to which events they are subscribed.
* Receiving any published message and then distributing it out to all connected and subscribed clients.
* Queue will keep track of the delivery status of every event/message.
* Queue will track missed messages while clients lose connection with server and send it to clients when the connection is back online. 