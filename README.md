# Java Chatroom Application
A simple multi-client chatroom application implemented in Java using socket programming.  
This project demonstrates how to build a server-client architecture with multi-threading, enabling multiple clients to connect, send, and receive messages in real-time.

## Features
- Multi-threaded server to handle multiple clients concurrently
- Broadcast messages to all connected clients
- Notify users when clients join or leave the chat
- Console-based client interface

## Project Structure
- `Server.java` — Server-side application that listens for client connections and manages communication
- `ClientHandler.java` — Handles individual client connections and message broadcasting on the server
- `Client.java` — Client-side application that connects to the server and sends/receives messages

## Prerequisites
- Java Development Kit (JDK) 17 or higher installed  
- Basic knowledge of Java and socket programming  
- Network access between client and server machines

### Compile the code
javac Server.java ClientHandler.java Client.java

## Run the server
java Server
The server will start and listen on port 1234.

## Run the client
Before running the client, update the Server IP address in Client.java to the server machine's IP (e.g., 192.168.1.100).
Socket socket = new Socket("SERVER_IP_ADDRESS", 1234);
Then run:
java Client

## Usage
When the client runs, enter your username.

Type messages and press Enter to send.

To leave the chat, type /quit and press Enter.

## Notes
Ensure that the server machine’s firewall allows connections on port 1234.

All clients must be on the same network or have proper routing to the server.

This project is for educational purposes and lacks advanced security features.

