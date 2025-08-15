# TCP Secure Multi-Client Chat Server in C++

A lightweight, **multi-threaded TCP chat server** built in C++ that supports multiple clients, secure communication, and real-time message broadcasting.

This project serves as a **foundation for secure distributed applications** — you can extend it into encrypted file transfer, blockchain logging, or even vehicular network simulations.

---

## 📌 Features
- 📡 **Multi-client support** using POSIX threads or `std::thread`
- 🔒 **Optional end-to-end encryption** with AES-256 (RSA key exchange for symmetric keys)
- 💬 Real-time broadcasting to all connected clients
- 🔑 Simple username/password authentication
- 📜 Server-side message logging with timestamps
- ⚙️ Configurable port & max connections

---

## 🛠️ Tech Stack
- **Language:** C++17
- **Networking:** BSD/POSIX sockets
- **Threading:** `std::thread` or `pthread`
- **Security:** OpenSSL (AES/RSA)
- **Build System:** CMake

---

## 🚀 Getting Started

### Prerequisites
- **Linux** environment (Ubuntu/Debian recommended)
- C++17 compatible compiler (`g++` or `clang++`)
- OpenSSL library installed

```bash
sudo apt update
sudo apt install g++ cmake libssl-dev
````

---

### Build & Run

#### Clone the Repository

```bash
git clone https://github.com/yourusername/tcp-secure-chat.git
cd tcp-secure-chat
```

#### Build the Project

```bash
mkdir build && cd build
cmake ..
make
```

#### Run the Server

```bash
./server <port>
```

#### Run a Client

```bash
./client <server_ip> <port>
```

---

## 💻 Example Usage

**Server Output:**

```text
[SERVER] Listening on port 5000...
[SERVER] Client connected: Alice
[SERVER] Message from Alice: "Hello world!"
```

**Client Output:**

```text
[CLIENT] Connected to server 127.0.0.1:5000
[Alice]: Hello world!
[Bob]: Hi Alice!
```

---

## 📂 Project Structure

```
tcp-secure-chat/
├── src/
│   ├── server.cpp
│   ├── client.cpp
│   ├── encryption.cpp
│   └── utils.cpp
├── include/
│   ├── encryption.hpp
│   ├── utils.hpp
├── CMakeLists.txt
└── README.md
```

---

## 🔮 Future Extensions

* Encrypted file transfer between clients
* Blockchain-based chat logging
* Integration with VANET (Vehicular Network) simulations for secure vehicle messaging
* WebSocket bridge for browser-based clients

---

## 📜 License

This project is licensed under the MIT License — feel free to use, modify, and distribute.

---

## 🤝 Contributing

Pull requests are welcome! If you have ideas for improvements, feel free to open an issue or submit a PR.

---

## 🌟 Acknowledgements

* **OpenSSL** for cryptographic functions
* BSD/POSIX sockets documentation
* The C++ community for open-source support

```

---

If you want, I can also create a **diagram** showing **how clients and server communicate** so your repo looks extra professional.  
Would you like me to make that diagram next?
```
