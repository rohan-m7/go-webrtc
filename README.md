# go-webrtc 🚀 | WebRTC Library for Go

**go-webrtc** is a lightweight and scalable **WebRTC library for Go** that enables **peer-to-peer audio, video, and data streaming**. Built on top of [Pion WebRTC](https://github.com/pion/webrtc), it provides an easy-to-use API for handling signaling, media exchange, and real-time communication.

---

## **Features** ✨

✅ Peer-to-peer **audio & video calls**  
✅ Secure **signaling and session management**  
✅ **ICE/STUN/TURN** support for NAT traversal  
✅ **WebSocket & gRPC** integration  
✅ **Error handling & logging** for production readiness  
✅ Optimized for **high-performance & scalability**

---

## **Installation** 📦

```sh
 go get github.com/yourusername/go-webrtc
```

---

## **Getting Started** 🛠️

```go
package main

import (
    "log"
    "github.com/yourusername/go-webrtc"
)

func main() {
    config := webrtc.NewConfig()
    peer, err := webrtc.NewPeerConnection(config)
    if err != nil {
        log.Fatal(err)
    }

    peer.Start()
}
```

---

## **Use Cases** 📌

🔹 **VoIP Calls** (Private & Secure)  
🔹 **Live Video Streaming**  
🔹 **Real-time Chat & Data Channels**  
🔹 **IoT & Edge Communication**

---

## **Configuration** ⚙️

You can configure `go-webrtc` with custom signaling, STUN/TURN servers, and error handling.

```go
config := webrtc.Config{
    ICEServers: []string{"stun:stun.l.google.com:19302"},
    LogLevel: "debug",
}
```

---

## **Error Handling & Logging** 📝

Proper error handling and logging are built-in to ensure reliability in production.

```go
log.SetLevel(log.DebugLevel)
log.Info("WebRTC connection initialized.")
```

---

## **Contributing** 🤝

We welcome contributions! Open an issue or submit a pull request.

---

## **License** 📜

MIT License – Free to use and modify.
