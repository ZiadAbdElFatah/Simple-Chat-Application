# Simple Chat Application
This is a simple chat application built using Java. It consists of a **client** and a **server** that allow multiple users to communicate in real-time. The server handles incoming connections and broadcasts messages to all connected clients, while the client provides a user-friendly interface for sending and receiving messages.


## Features ##
* **Real-time messaging**: Send and receive messages instantly.

* **Multiple clients**: The server supports multiple clients simultaneously.

* **Simple GUI**: The client has an easy-to-use graphical interface.

* **Java NIO**: Uses Java's Non-blocking I/O (NIO) for efficient communication.

## Project Structure ##
* **SimpleChatClient.java**: The client-side application. It connects to the server and provides a GUI for sending and receiving messages.

* **SimpleChatServer.java**: The server-side application. It accepts client connections and broadcasts messages to all connected clients.

## Code Overview
#### Client (SimpleChatClient.java)
* **GUI**: Built using JFrame, JTextArea, and JTextField.

* **Networking**: Connects to the server using SocketChannel and communicates via BufferedReader and PrintWriter.

* **Message Handling**: Sends messages to the server and displays incoming messages in the text area.

#### Server (SimpleChatServer.java)
* **Server Setup**: Listens for client connections on port 5000 using ServerSocketChannel.

* **Client Handling**: Each client is handled by a ClientHandler thread, which reads messages and broadcasts them to all clients.

* **Broadcasting**: Uses the tellEveryone method to send messages to all connected clients.
---
