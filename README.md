Multi-Threaded Server-Client Implementation
This repository contains a Java-based implementation of a multi-threaded server-client model. The example demonstrates how to handle multiple client connections concurrently using threads, allowing efficient communication between the server and multiple clients.

Features
Multi-threaded Server:
Listens for client connections on a specified port.
Creates a new thread for each client connection to handle communication independently.
Client:
Simulates multiple clients connecting to the server concurrently.
Each client sends a message to the server and receives a response.
Socket Communication:
Utilizes Java's Socket and ServerSocket classes for TCP-based communication.
How It Works
The Server:

Listens on port 8010 for incoming client connections.
Upon receiving a connection, spawns a new thread to handle the client's request.
Sends a greeting message back to the client.
The Client:

Creates multiple threads, each representing a client.
Each client connects to the server, sends a message, and waits for the server's response.
File Descriptions
Server.java:

Implements the multi-threaded server.
Uses a Consumer<Socket> to process client requests in individual threads.
Client.java:

Implements a client that creates multiple threads to simulate concurrent connections to the server.
Each thread sends a message to the server and receives a response.
