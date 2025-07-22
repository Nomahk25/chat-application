# 💬 Terminal Chat App (Python Socket + Threads)

A simple terminal-based chat application using **Python sockets** and **multithreading**. Users can join a chat room by connecting to a central server using a chosen nickname and send/receive messages in real-time.

---

## 🚀 Features

- Real-time chat over TCP
- Multiple clients can connect simultaneously
- Nickname system for identity
- Graceful disconnect and message broadcast when users leave
- Fully terminal-based using native Python

---

## 📁 File Structure

chat-app/
│
├── server.py # Chat server
├── client.py # Chat client
└── README.md


---

## ⚙️ How It Works

- The server (`server.py`) waits for incoming client connections.
- Each client (`client.py`) connects to the server and is prompted to choose a nickname.
- All messages from clients are broadcast to everyone connected.
- When a client disconnects, the server informs the others.

---

## 🧠 Requirements

- Python 3.x

You can install any missing modules using:

```bash
pip install -r requirements.txt

ℹ️ This app uses only standard Python libraries (socket, threading) — no external dependencies needed.

🖥️ Running the App
1. Start the Server

Open a terminal window and run:
python server.py

You should see:
Server is running...

2. Start One or More Clients

In new terminal windows, run:
python client.py

Enter your nickname when prompted, and start chatting!
You can open as many client instances as you'd like (locally or over LAN if modified).

🌐 Customizing Host/Port

In both server.py and client.py, change:
HOST = '127.0.0.1'  # For local use
PORT = 55555

To allow remote access:

Use your public/private IP instead of 127.0.0.1
Make sure the port is open and not blocked by firewall

📄 License
This project is licensed under the MIT License. Free to use and modify!

🙋 Author
Built by Nomanguni Khumalo with Python & 💬
