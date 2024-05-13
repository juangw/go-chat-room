# Go chat room
Simple go chat room implementation using gorilla websockets

# Setup
Run program
```bash
go run main.go
```

Visit localhost:8080 for homepage

Connect a client with curl command
```bash
curl -X GET -H "Connection: Upgrade" -H "Upgrade: websocket" -H "Sec-WebSocket-Version: 13" -H "Sec-WebSocket-Key: dGhlIHNhbXBsZSBub25jZQ==" localhost:8080/connect-client
```

Publish a hardcoded message to server that will broadcast messages to all clients
```bash
curl -X GET locahost:8080/publish-message
```
