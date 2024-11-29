# simple application utilizing Java socket programming, "Chat Application'

## Overview

Chat Application
The Chat Application is a simple client-server communication system implemented in Java. It is designed to demonstrate the core principles of network programming using sockets and the graphical user interface using Java Swing. The project provides a real-time messaging platform where a Server can host a chat and a Client can connect to it for communication.


## Features

- Real-time messaging between server and client.
- Simple and clean user interface.
- Timestamp for each message.
- Auto-scrolls as messages are sent or received.


## How to Run

### Step 1: Setup the Environment
1. Save the provided code into two files:
   - `Server.java`
   - `Client.java`

2. Ensure both files are located in the same directory.

### Step 2: Compile the Code
Open a terminal or command prompt, navigate to the directory containing the files, and compile the code:

bash
javac Server.java Client.java

### Step 3: Start the Server
Run the server by executing the following command:
bash
java Server
The server application will open a window and listen on port `6001`.

### Step 4: Start the Client
Open a new terminal or command prompt, and start the client application:

bash
java Client
The client application will open in a new window and connect to the server at `127.0.0.1` (localhost).

## Usage

1. The **Server** window is for the host.
2. The **Client** window is for the user who wants to connect to the server.
3. Messages typed in the text box at the bottom of either window can be sent by clicking **Send** or pressing **Enter**.
4. Messages sent or received appear in the chat area with a timestamp.


## Code Structure

### Server
- **Server.java** is the host program that listens on port `6001` for client connections.
- Accepts messages from connected clients and displays them in its window.

### Client
- **Client.java** connects to the server at `127.0.0.1` on port `6001`.
- Sends messages to the server and displays received messages in its window.

## Notes
- To run the application on different machines, ensure both systems are connected to the same network.
- Replace `127.0.0.1` in `Client.java` with the server's IP address for remote connections.
- Ensure port `6001` is open on both the server and client machines.


## Troubleshooting
- **Cannot connect to server:** Ensure the server is running and the IP/port is correct.
- **Messages not appearing:** Check for exceptions in the terminal. Both client and server must use the same port.

Enjoy chatting with this lightweight application!
