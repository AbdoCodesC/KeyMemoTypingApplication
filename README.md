# KeyMemo

**KeyMemo** is a real-time collaborative typing application inspired by platforms like Keybr. It allows users to practice typing while synchronizing typing activity across connected clients in real time.

The application uses WebSockets to enable low-latency communication between users, providing a responsive collaborative typing experience.

### Live Demo

[**Visit KeyMemo →**](https://keymemo.vercel.app)

### Features

- **Real-Time Synchronization:** Instantly synchronizes typing activity between connected users.
- **Collaborative Typing:** Enables multiple users to participate in shared typing sessions.
- **Low-Latency Communication:** Uses WebSocket connections for efficient, bidirectional communication.
- **Optimized Data Transmission:** Implements delta-based updates instead of repeatedly broadcasting the entire application state.
- **Responsive Interface:** Built with React and TypeScript for a dynamic user experience.

### Tech Stack

| Technology | Purpose |
|---|---|
| React | Frontend development |
| TypeScript | Type safety and maintainability |
| Node.js | Backend runtime |
| Socket.IO | Real-time, bidirectional communication |
| Vercel | Deployment |

### Technical Highlights

One of the main engineering challenges was optimizing real-time communication between connected clients.

Initially, broadcasting the entire application state for every typing update created unnecessary network overhead. I addressed this by implementing delta-based updates, transmitting only the changes rather than repeatedly sending the full state.

This improved communication efficiency and helped maintain responsive synchronization, with latency measured under 50ms during testing.

### Project Availability

This repository serves as a public showcase of KeyMemo. The application's source code is not open source.

**Try it out:** [https://keymemo.vercel.app](https://keymemo.vercel.app)
