Overview
The Reliable UDP Client-Server System facilitates the reliable transfer of files between a client and a server using the User Datagram Protocol (UDP). This system enhances the traditional UDP behavior by incorporating reliability features to ensure the secure and accurate transmission of data.

Repository Structure
The repository contains two main components:

Client:
client.cpp: Implementation of the Reliable UDP Client.

Server:
server.cpp: Implementation of the Reliable UDP Server.

Build Instructions:
Client
Navigate to the client directory.
Run the following command to build the client:
make

Server
Navigate to the server directory.
Run the following command to build the server:
make

Usage
Client
Run the client executable with the following command:
./client <server_hostname> <server_port> <filename> <window_size>
<server_hostname>: Hostname or IP address of the server.
<server_port>: Port number on which the server is listening.
<filename>: Name of the file to be requested from the server.
<window_size>: Window size in bytes for reliable data transfer.

Server
Run the server executable with the following command:
./server <port_number> <window_size>
<port_number>: Port number on which the server will listen for incoming connections.
<window_size>: Window size in bytes for reliable data transfer.

Example
Client
./client localhost 12345 example.txt 1000

Server
./server 12345 1000

Dependencies
The Reliable UDP Client-Server System relies on standard C++ libraries and POSIX headers. Ensure that your system has the necessary libraries installed.

Contributors
Iqra Rasool
Sheeza Aslam
