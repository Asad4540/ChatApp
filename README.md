JAVA CHAT APPLICATION

DESCRIPTION:
A basic chat application using JAVA SWING for GUI and JAVA NETWORKING for real-time communication between a SERVER and CLIENT.

TECHNOLOGIES USED:

1. GUI – JAVA SWING
- JFRAME: Main window of the app.
- JPANEL: Container for components.
- JTEXTFIELD: Input box to type messages.
- JBUTTON: Button to send messages.
- JLABEL: To show text and icons.

2. NETWORKING – JAVA
- SERVERSOCKET: Waits for clients to connect.
- SOCKET: Connects to server.
- DATAINPUTSTREAM & DATAOUTPUTSTREAM: For reading and writing messages.

3. LAYOUT – JAVA AWT
- BOXLAYOUT: Arranges GUI components vertically or horizontally.

4. JAVA I/O
- BufferedReader and PrintWriter (not used directly but common in similar apps).

FEATURES:

SERVER SIDE:
- Accepts connection from client.
- Sends and receives messages.
- Shows messages on GUI.

CLIENT SIDE:
- Connects to server.
- Sends and receives messages.
- Updates chat window instantly.

KEY FEATURES:
- REAL-TIME MESSAGING between server and client.
- USER-FRIENDLY INTERFACE using Swing.
- CHAT UPDATES live with timestamps.

FILES OVERVIEW:

SERVER.JAVA
- PURPOSE: Waits for client, displays messages, sends responses.
- SETUP: Uses JFrame, JPanel, JLabel, JTextField, JButton.
- NETWORKING: Listens on port (like 443), handles client via Socket.
- HANDLING MESSAGES: Reads client messages, displays them, and sends server messages.
- FUNCTION: formatLabel(String out) – adds timestamp and formats message.

CLIENT.JAVA
- PURPOSE: Connects to server, sends & receives messages.
- SETUP: Same GUI as server.
- NETWORKING: Connects to 127.0.0.1 (localhost).
- HANDLING MESSAGES: Sends message from GUI, receives and displays from server.
- FUNCTION: formatLabel(String out) – adds timestamp and formats message.

HOW TO RUN:

1. COMPILE AND START SERVER:
   javac Server.java
   java chatApp.Server

2. COMPILE AND START CLIENT:
   javac Client.java
   java chatApp.Client

NOTE: Start the server first before running the client.

SENDING MESSAGES:
- Type message in input box.
- Click "Send".
- Message appears in both server and client windows.

MESSAGE FLOW:
- Messages are sent via Socket.
- GUI updates live as messages arrive.

SUMMARY:
- JAVA SWING for user interface.
- JAVA NETWORKING for connection.
- EASY TO USE, great beginner project.
