# Message Queues

[Socket.io Chat Example](https://socket.io/get-started/chat/)

- Explain to a non-technical recruiter what the Chat Example (above) does.
  - a chat application that allows mutliple users to communication through a single server by utilizing Socket.io
- What proof of life are we getting on the backend from the above app?
  - The server logs events as they happen, including the initial connection with the client
- Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?
  - A Broadcast flag

[Rooms](https://socket.io/docs/v4/rooms)

- What is a room and how might a room be useful?
  - A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients:
- How do you join a room?
  - You can call join to subscribe the socket to a given channel:

        io.on("connection", (socket) => {
          socket.join("some room");
        });
- how do you leave a room?
  - To leave a channel you call leave in the same fashion as join.

[Namespaces](https://socket.io/docs/v4/namespaces/)

- What is a Namespace and what does it allow you to do?
  - A Namespace is a communication channel that allows you to split the logic of your application over a single shared connection (also called "multiplexing").
- Each namespace potentially has its own what? (hint: 3 things)
  - Event handlers, rooms, and middlewares
- Discuss a possible use case for separate namespaces
  - you want to create a special namespace that only authorized users have access to, so the logic related to those users is separated from the rest of the application. An example would be a namespace specifically for the admin of a companny.

## Things I want to know more about

- Implementing rooms into our projects this week

[Return home](https://khofstetter94.github.io/reading-notes/)
