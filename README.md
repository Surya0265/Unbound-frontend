# Command Gateway Frontend

A secure, terminal-styled execution system frontend built with React, TypeScript, and Vite.

## Features

- 🖥️ **Terminal Interface**: A sleek, dark-mode terminal UI for command execution.
- 🔒 **Secure Authentication**: API key-based authentication with role-based access control.
- ⚡ **Real-time Updates**: Instant feedback on command status and approvals.
- 📝 **Audit Logging**: Comprehensive logs for all actions (Admin only).
- 🚦 **Approval Workflow**: System for reviewing and approving sensitive commands.

## Tech Stack

- **Framework**: React 18
- **Build Tool**: Vite
- **Language**: TypeScript
- **Styling**: TailwindCSS (Custom Terminal Theme)
- **Routing**: React Router

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd command-gateway-frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory:
   ```env
   VITE_API_BASE=http://localhost:3001/
   ```
   > **Note**: Ensure the URL includes the protocol (http://) and a trailing slash (/).

### Running Locally

Start the development server:

```bash
npm run dev
```

The application will be available at `http://localhost:5173`.

### Building for Production

Build the project for production:

```bash
npm run build
```

The output will be in the `dist` directory.

## Deployment

### Vercel

This project includes a `vercel.json` configuration for easy deployment on Vercel.

1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` to deploy.

The configuration handles:
- SPA routing rewrites
- Cache headers for performance
- Build command and output directory configuration

## Project Structure

```
src/
├── api/          # API client and type definitions
├── components/   # React components (Dashboard, Login, etc.)
├── context/      # Context providers (AuthContext)
└── main.tsx      # Entry point
```
