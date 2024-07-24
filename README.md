# Intranet Communication and File Sharing Application

## Project Overview

This project aims to develop a web-based application for intranet communication and file sharing. The application will function without internet access, making it suitable for emergency situations and environments with unreliable internet connectivity. It will support future extensions to iOS and Android platforms. The primary features include file sharing, real-time communication (audio, video, and messaging), and robust connectivity across Local Area Networks (LAN), Wide Area Networks (WAN), and Internet Exchange Points (IXP).

## Features

1. **File Sharing:**

   - Securely share files between users within the intranet.
   - Support for large files with high transfer speeds due to local network utilization.

2. **Real-Time Communication:**

   - **Audio and Video Calls:** High-quality audio and video calls using WebRTC.
   - **Messaging:** Instant messaging with text, images, and file attachments.
   - **Group Chat:** Create and manage group conversations.

3. **Connectivity:**

   - **Local Discovery:** Use mDNS for discovering devices on the same LAN.
   - **NAT Traversal:** Implement local STUN/TURN servers for NAT traversal within the intranet.
   - **Fallback Mechanism:** Seamlessly switch between LAN, WAN, and IXP networks for uninterrupted connectivity.

4. **Security:**

   - End-to-end encryption for all communications and file transfers.
   - User authentication and authorization mechanisms.

5. **Offline Support:**
   - Store messages and files locally and synchronize when connectivity is restored.

## Project Structure

- **Frontend:** Developed using React/Vue.js for a dynamic and responsive user interface.
- **Backend:** Built with Go for high performance and concurrency capabilities.
- **WebRTC:** Used for real-time communication (audio, video, and messaging).
- **Database:** Distributed database like CockroachDB or Couchbase for resilient and scalable data storage.
- **Signaling Server:** Facilitates initial connection setup between peers.

## Getting Started

### Prerequisites

- Node.js and npm (for frontend development)
- Go (for backend development)
- Docker (optional, for containerized deployment)

1. **Install Frontend Dependencies:**

   ```sh
   cd frontend
   npm install
   ```

2. **Install Backend Dependencies:**

   ```sh
   cd backend
   go mod tidy
   ```

### Running the Application

1. **Start the Backend Server:**

   ```sh
   cd backend
   go run main.go
   ```

2. **Start the Frontend Development Server:**

   ```sh
   cd frontend
   npm start
   ```

3. **Access the Application:**
   Open your browser and navigate to `http://localhost:3000`.

## TODO List

1. **Frontend:**

   - [ ] Design and implement user interface for file sharing.
   - [ ] Integrate WebRTC for real-time communication.
   - [ ] Develop messaging interface and group chat functionality.

2. **Backend:**

   - [ ] Set up and configure STUN/TURN servers.
   - [ ] Implement user authentication and authorization.
   - [ ] Develop file sharing API endpoints.
   - [ ] Ensure secure data transmission and storage.

3. **General:**
   - [ ] Perform extensive testing and debugging.
   - [ ] Optimize performance for large-scale deployments.
   - [ ] Write comprehensive documentation.

<!-- ## Contributing

We welcome contributions from the community! Please read our [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests. -->
