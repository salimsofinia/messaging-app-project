# Messaging App Project - WiiChat

**WiiChat** is a C# Windows Forms messaging application that supports both **Group Chat (Global Chat)** and **Peer-to-Peer (P2P)** communication over TCP. Designed with simplicity and interactivity in mind, it provides a clean interface and dynamic server connection options for seamless chatting.

---

## Features

- Join Global Group Chat via a central server.
- Initiate P2P Chats by connecting directly to another client through a P2P server.
- Toggle between Group and P2P modes in real-time.
- RichTextBox formatting with usernames, timestamps, and system messages.
- Validation for user input and server connection.
- Graceful disconnection and error handling.

---

## How It Works

### Group Chat
1. User connects to the **GroupServer**.
2. Messages are broadcasted to all connected clients.
3. Notifications when users join/leave the chat.

### Peer-to-Peer Chat
1. User connects to the **PTPServer**.
2. Select a recipient IP/port to initiate direct messaging.
3. Messages are sent privately between two clients only.

---

## Technologies

- **Language:** C# (.NET Framework)
- **UI Framework:** Windows Forms (WinForms)
- **Network:** TCP/IP using `System.Net.Sockets`
- **Multithreading:** `System.Threading` for handling concurrent clients
