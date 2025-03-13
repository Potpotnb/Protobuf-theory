# Distributed Caching System: Simplified Implementation

Welcome to the **Distributed Caching System** repository! This project provides a practical implementation of a distributed caching system, focusing on essential concepts and features. It includes an LRU cache eviction policy, single-machine concurrent caching, an HTTP server, consistent hashing, distributed nodes, cache breakdown prevention, and Protobuf-based communication. This repository is designed to help you understand and build a basic yet functional distributed caching system.

## 📖 Overview

This project implements the following key features:

- **LRU Cache Eviction Policy**: Efficiently manage cache size by removing the least recently used items.
- **Single-Machine Concurrent Cache**: Support concurrent access to the cache in a single-machine environment.
- **HTTP Server**: Expose the cache functionality via an HTTP interface.
- **Consistent Hashing**: Distribute data across multiple nodes using consistent hashing for scalability.
- **Distributed Nodes**: Enable communication and coordination between multiple cache nodes.
- **Cache Breakdown Prevention**: Implement mechanisms to prevent cache breakdown under high load.
- **Protobuf Communication**: Use Protobuf for efficient and structured communication between nodes.

## 🚀 Features

- **LRU Eviction Policy**: Manage cache size effectively with the Least Recently Used (LRU) algorithm.
- **Concurrency Support**: Handle multiple concurrent requests in a single-machine cache.
- **HTTP Interface**: Access the cache via a simple HTTP API.
- **Consistent Hashing**: Distribute data evenly across nodes for scalability.
- **Distributed Architecture**: Support multiple nodes working together as a distributed cache.
- **Cache Breakdown Prevention**: Protect the system from cache breakdown under high traffic.
- **Protobuf Integration**: Use Protobuf for efficient and type-safe communication.

## 🛠️ Getting Started

### Prerequisites

To run the code in this repository, you'll need:

- **Go 1.16+** (or the latest stable version)
- **Protobuf Compiler (`protoc`)**
- **Basic understanding of distributed systems and caching concepts**

### Installation

1. Clone the repository:

2. Install dependencies:
   - Install the Protobuf compiler (`protoc`) if not already installed.
   - Install Go dependencies:
     ```bash
     go mod download
     ```

3. Compile Protobuf files:
   ```bash
   protoc --go_out=. --go-grpc_out=. proto/cache.proto
   ```

4. Run the application:
   - Start testing demo (if applicable):
     ```bash
     bash main.sh
     ```

## 📂 Project Structure

```
Distributed Caching System/
├── geecache/lru                      # LRU cache implementation
├── geecache/single                 # Single-machine concurrent cache
├── geecache/consistenthash                    # Consistent hashing implementation
├── geecache/geecachepb/                      # Protobuf definitions and generated code
├── main.go                     # Entry point for the application
├── main.sh                     # Some test samples by shell command
├── go.mod                      # Go module file
└── README.md                   # This file
```

## 📚 Resources

- **LRU Cache**: [Wikipedia](https://en.wikipedia.org/wiki/Cache_replacement_policies#Least_recently_used_(LRU))
- **Consistent Hashing**: [Wikipedia](https://en.wikipedia.org/wiki/Consistent_hashing)
- **Protobuf**: [Official Documentation](https://developers.google.com/protocol-buffers)
- **Cache Breakdown Prevention**: [Blog Post](https://en.wikipedia.org/wiki/Cache_stampede)

## 🤝 Contributing

We welcome contributions! If you'd like to improve this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

Please ensure your code adheres to the project's coding standards and includes appropriate documentation.

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.


Happy coding! 🎉 Explore, learn, and build a functional distributed caching system with this repository.
