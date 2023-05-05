# GroupChat Application

The GroupChat application is a simple messaging/chat program that follows a client-server architecture. It allows users to communicate with each other in real-time using multicast communication.

## How to Run

To run the GroupChat application, follow these steps:

1. Compile the Java source files:
```
javac GroupChat.java
```

2. Run the application by executing the `GroupChat` class with the required command-line arguments:

```
java GroupChat <multicast-host> <port-number>
```

Replace `<multicast-host>` with the desired multicast group address, such as `239.0.0.0`, and `<port-number>` with the desired port number, for example, `1234`.

3. When prompted, enter your name to identify yourself in the chat.

4. Start typing messages in the console window. Press Enter to send a message.

- To exit the application, type `Exit` and press Enter.

## Architecture

The GroupChat application follows the client-server architecture. Here's an overview of the components:

- The `GroupChat` class represents the client-side application. It handles user input, sends messages to the server, and receives messages from the server.

- The `ReadThread` class is a separate thread that runs in the background to read incoming messages from the server and display them in the console.

## Dependencies

The GroupChat application has no external dependencies beyond the standard Java libraries.

## Limitations

- The application is designed for communication within a multicast group on a local network.

- Multicast communication requires support from the network infrastructure and may not be available in all environments.

## Troubleshooting

If you encounter any issues or errors while running the application, ensure that:

- You have provided the correct command-line arguments: `<multicast-host>` and `<port-number>`.
- The multicast group address and port number are available and accessible in your network environment.
- There are no network or firewall restrictions preventing multicast communication.
