# OIBSIP_Python-Programming_3
📌 Project Objective

The objective of this project is to develop a Client–Server Chat Application using Python.

The application enables multiple users to communicate in real-time over a network using socket programming and multithreading.

This project demonstrates:

Network communication using sockets

Client–server architecture

Multithreading for handling multiple users

GUI development using Tkinter

Real-time message broadcasting

🛠 Tools and Technologies Used

Python 3

Socket Module – Network communication

Threading Module – Handling multiple clients simultaneously

Tkinter – GUI development

ScrolledText Widget – Displaying chat messages

🧱 Project Structure
Chat-Application/
│
├── server.py
├── client.py
└── README.md

🔹 server.py

Creates and manages the server

Handles multiple client connections

Broadcasts messages to all connected clients

Manages usernames and disconnections

🔹 client.py

Connects to the server

Provides GUI for sending and receiving messages

Displays real-time chat updates

Allows user to enter username

⚙️ Steps Performed
1️⃣ Server Implementation

Created a socket server using socket.AF_INET and socket.SOCK_STREAM

Bound server to:

Host: 127.0.0.1

Port: 5555

Listened for incoming client connections

Stored connected clients and usernames

Implemented broadcast function to send messages to all clients

2️⃣ Client Implementation

Created client socket

Connected to server using IP and port

Prompted user to enter username

Built chat GUI using Tkinter

Allowed sending messages to server

3️⃣ Multithreading

Used threading module to:

Handle multiple clients simultaneously

Receive messages without freezing GUI

Created separate threads for:

Handling each client (server side)

Receiving messages (client side)

4️⃣ Real-Time Communication

Server receives messages from one client

Broadcasts messages to all connected clients

Displays join and leave notifications

Ensures continuous communication without blocking

5️⃣ GUI Development

Built user-friendly chat window

Implemented:

Scrollable chat area

Message input field

Send button

Automatically scrolls to latest message

🔄 How the Application Works

Start the server (server.py)

Launch one or more clients (client.py)

Each client enters a username

Clients connect to the server

Messages are sent to the server

Server broadcasts messages to all clients

Users can chat in real time

▶️ How to Run
Step 1: Start Server
python server.py

Step 2: Start Client (in new terminal window)
python client.py


You can open multiple clients to simulate multiple users.

✅ Key Features

Client–Server Architecture

Real-time messaging

Multi-client support

Username-based chat system

Join/Leave notifications

Multithreaded implementation

Simple GUI interface

🚀 Outcome

The final outcome is a fully functional real-time chat application that allows multiple users to communicate over a local network.

This project successfully combines:

Network programming concepts

Multithreading

GUI development

Real-time communication systems

It demonstrates practical implementation of socket programming and concurrent systems, which are fundamental concepts in networking and distributed systems.
