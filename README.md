# Timeline Application

A full-stack timeline management application that allows users to create, manage, and share different types of timelines with AI-powered segment generation.

🚀 **Live Demo:** [https://timeline-frontend-three.vercel.app/](https://timeline-frontend-three.vercel.app/)

## Overview

This monorepo contains both the frontend and backend for the Timeline Application, enabling users to create structured timelines for roadmaps, projects, and more with intelligent scheduling and tracking capabilities.

## Features

- **User Authentication** - Secure JWT-based authentication with token refresh
- **Timeline Management** - Create public/private timelines with different time units (daily, weekly, monthly)
- **Segment Management** - Organize timeline segments with goals, references, and scheduling
- **AI Integration** - Generate timeline segments using AI
- **Timeline Forking** - Duplicate and customize existing timelines
- **Responsive UI** - Modern Next.js frontend with Tailwind CSS

## Tech Stack

### Frontend (`/client`)
- Next.js 14 (App Router)
- TypeScript
- Tailwind CSS
- Playwright (E2E testing)

### Backend (`/server`)
- Node.js + Express
- TypeScript
- PostgreSQL
- JWT Authentication
- Jest (Testing)

## Getting Started

### Prerequisites
- Node.js (v14+)
- PostgreSQL (v12+)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd timeline-app
```

2. Install dependencies for both projects:
```bash
# Install client dependencies
cd client
npm install

# Install server dependencies
cd ../server
npm install
```

3. Set up environment variables:
   - Create `.env` file in `/server` directory (see server README for details)
   - Create `.env.local` file in `/client` directory

4. Start the development servers:
```bash
# Terminal 1 - Start backend
cd server
npm run dev

# Terminal 2 - Start frontend
cd client
npm run dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser

## Project Structure

```
├── client/          # Next.js frontend application
│   ├── src/
│   │   ├── app/     # App router pages and components
│   │   ├── lib/     # API services and utilities
│   │   └── contexts/# React contexts
│   └── tests/       # E2E tests
│
└── server/          # Express backend API
    ├── src/
    │   ├── modules/ # Feature modules (auth, timeline, segment, user)
    │   └── shared/  # Shared utilities and middleware
    └── api/         # API entry point
```

## Documentation

- **API Documentation:** [View API Docs](https://frost-petroleum-f94.notion.site/API-Documentation-Timeline-App-1b06b12c876680388e5ecbe541130a30)
- **Client README:** See `/client/README.md`
- **Server README:** See `/server/README.md`

## License

This project is open source and available under the MIT License.
