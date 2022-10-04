# Socket.io

[Web sockets](https://en.wikipedia.org/wiki/WebSocket)

- What is a Web Socket?
  - WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.
- Describe the Web Socket request/response handshake and what happens once the connection is established.
  - The handshake starts with an HTTP request/response, allowing servers to handle HTTP connections as well as WebSocket connections on the same port. Once the connection is established, communication switches to a bidirectional binary protocol which does not conform to the HTTP protocol.
- Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client.
  - request

[Socket.io Tutorial](https://www.tutorialspoint.com/socket.io/)

- What does the event handler io.on() do?
  - The io.on event handler handles connection, disconnection, etc., events in it, using the socket object.
- Describe some possible proof of life or proof that the code works as expected
  - You can use strategic console logs to log when a user connects and when a user disconnects.
- What does socket.emit() do?
  - To broadcast an event to all the clients, we can use the io.sockets.emit method.

[Socket.io vs Web Sockets](https://www.educba.com/websocket-vs-socket-io/)

- What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).
  - WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.
  - Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.
- When would you use Socket.IO?
  - It provides full-duplex communication, which helps in persisting the connection established between the Client and the Web Server. It also lives up to the standards and provides the accuracy and efficiency stream events to and from with negligible latency. WebSocket removes the overhead and reduce complexity. It makes real-time communication effortless and efficient.
- When would you use WebSockets?
  - It provides full-duplex communication, which helps in persisting the connection established between the Client and the Web Server. It also lives up to the standards and provides the accuracy and efficiency stream events to and from with negligible latency. WebSocket removes the overhead and reduce complexity. It makes real-time communication effortless and efficient.

[OSI Model Explained](https://www.youtube.com/watch?v=vv4y_uOneC0)

- What are a couple of key takeaways from this video?
  - The application layer provides services for network applications. The presentation layer recieves data from the application layer, translates it, uses data compression, and encryption/decryption. The session layer helps set up and manage connections, uses APIs and NETBIOS, uses authentication/authorization with the server, keeps track of the files that are being downloaded. The transport layer, controls the reliablility of communication through segmentation, flow control, and error control, the protocols for this layer are TCP and UDP. The network layer works for the trasmission of the recieved data segments from one computer to another, it uses logical addressing, routing, and path determination. The data link layer recieves the data packet from the network layer and handles physical addressing, it deals with accessing the media with framing and controlling how data is placed and recieved from the media (using media access control and error detection). The physical layer converts BITs into signals which interacts with the specific media being used.

[TCP Handshakes Explained](https://www.youtube.com/watch?v=xMtP5ZB3wSk)

- Translate the gist of this video to a non-technical friend
  - TCP is Transimission Control Protocol. With TCP, data can be delivered successfully and accurately. It uses a 3-way handshake to establish a connection.
    - Step One: The client sends a SYN segment to the server, asking for synchronization
    - Step Two: The server replies with SYN-ACK
    - Step Three: The client replies with ACK, with is like "Yes"

## Things I want to know more about

- Everything about Web Sockets and Socket.io

[Return home](https://khofstetter94.github.io/reading-notes/)
