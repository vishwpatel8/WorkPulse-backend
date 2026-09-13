# TaskPulse Backend

The backend service for **TaskPulse**, a unified project management and workforce tracking platform designed to combine project management, time tracking, and activity monitoring into a single system.

TaskPulse uses **WebSocket-based real-time communication** to keep project and time-tracking data synchronized without relying heavily on repeated third-party API polling.

## 🚀 Tech Stack

- **NestJS** — Backend framework
- **PostgreSQL** — Primary database
- **Neon** — Managed PostgreSQL infrastructure
- **Prisma ORM** — Database access and schema management
- **WebSockets** — Real-time communication and synchronization
- **JWT** — Authentication and authorization
- **TypeScript** — Application language

## ✨ Core Features

- User authentication and authorization
- Workspace and team management
- Project and task management
- Task status and workflow management
- Project deadlines and progress tracking
- Time tracking
- Real-time task and project synchronization
- WebSocket-based live updates
- Employee activity tracking
- Desktop application integration
- Activity and time-tracking data ingestion
- Screenshot metadata management
- Role-based access control

## 🧠 Why TaskPulse?

Traditional project-management and time-tracking workflows often require multiple systems to work together. This can introduce synchronization delays, duplicated data, and dependency on third-party APIs.

TaskPulse is designed around a **single platform with real-time communication**, allowing project activity and time-tracking information to stay synchronized as work happens.

The backend acts as the central source of truth for the web application and desktop application.

## 🔌 Real-Time Architecture

TaskPulse uses WebSockets for real-time communication between clients and the backend.

Instead of continuously polling APIs for changes, connected clients can receive relevant updates as soon as they occur.

This enables:

- Live task updates
- Real-time project progress
- Immediate time-tracking updates
- Live activity synchronization
- Reduced unnecessary API requests
- Better synchronization between the web and desktop applications

## 🗄️ Database

TaskPulse uses PostgreSQL as its primary relational database.

The database stores core application data such as:

- Users
- Workspaces
- Teams
- Projects
- Tasks
- Time entries
- Activity records
- Permissions
- Desktop activity information

PostgreSQL is hosted using **Neon**.

## 🔐 Authentication & Authorization

The API uses token-based authentication and role-based authorization to control access to workspace, project, task, and tracking resources.

Different user roles can have different permissions for managing projects, reviewing activity, and accessing tracking information.

## 🖥️ Desktop Integration

The TaskPulse desktop application is built with Electron.js and communicates with this backend to provide:

- Time tracking
- OS-level activity information
- Screenshot capture metadata
- Active-work tracking
- Real-time synchronization

The backend provides the APIs and WebSocket infrastructure required to synchronize desktop activity with the TaskPulse web application.

## 📡 API & WebSocket Communication

The backend exposes REST APIs for standard application operations and WebSocket connections for real-time events.

REST APIs are primarily responsible for:

- Authentication
- CRUD operations
- Project management
- Task management
- Time entries
- User and workspace management

WebSockets are primarily responsible for:

- Real-time updates
- Synchronization events
- Live task changes
- Tracking updates
- Client notifications

## 📄 License

This is a private and proprietary project.

The source code may not be copied, modified, distributed, sold, published, or used for personal portfolios or other purposes without explicit written permission.

See [LICENSE](LICENSE) for the full terms.
