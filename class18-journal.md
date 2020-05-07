# Class 18 - Socket.io - 5/6/2020

## Socket.io
* It is a library that enables real-time and full duplex communication between the client and the web servers.
* It provides websocket protocol to provide the interface.
* It also provides broadcasting, namespacing and other means of segmenting connected clients into groups.
* Client Side: a library that runs inside the browser.
* Server Side: a library for Node.js
* Connect to a server over HTTP. The session is "kept alive" through it's internal use of the websocket protocol, with session information being preserved.
* Events are sent with `emit()` and received with `on()`.
* Clients emit events.
* Server listens events and responds (boradcast or emit) to them.
* Not every client will have a listener for every event.
* The server may not have a listener for every event a client sends.