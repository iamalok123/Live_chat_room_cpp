# LiveChatRoomCpp

A simple and efficient chat room application implemented in C++ using Boost.Asio for asynchronous network communication and threading for handling concurrent client connections.

## Project Overview

ChatRoomCpp is a robust chat room application that enables multiple clients to connect to a server and exchange messages in real-time. Built with modern C++ practices, it leverages Boost.Asio for efficient network operations and threading for concurrent client management.

## Key Features

- **Asynchronous Communication**: Utilizes Boost.Asio for non-blocking I/O operations
- **Multi-threading Support**: Handles multiple client sessions simultaneously
- **Room Management**: Efficient management of connected clients in chat rooms
- **Message Handling**: Robust message encoding, decoding, and delivery system

## Architecture

### Core Components

1. **Session**
   - Manages individual client connections
   - Handles message reading and writing
   - Manages client socket operations

2. **Room**
   - Manages connected clients
   - Handles client addition and removal
   - Facilitates message broadcasting to all participants

3. **Message**
   - Handles message encoding and decoding
   - Manages message headers and body
   - Ensures reliable message delivery

### Critical Functionalities

#### Async I/O
- Non-blocking I/O operations using Boost.Asio
- Efficient handling of multiple client connections
- Asynchronous read and write operations

#### Threading
- Concurrent client session management
- Separate thread for each client connection
- Efficient resource utilization

#### Session Management
- Robust client connection handling
- Asynchronous message processing
- Reliable message delivery system

#### Room Management
- Centralized client tracking
- Efficient message broadcasting
- Dynamic client management

## Requirements

- C++17 or later
- Boost library
- CMake 3.10 or later


## Usage

1. Start the server:
```bash
./chatApp <port number>
```

2. Connect clients:
```bash
./clientApp <port number>
```

