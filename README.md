# SocietyConnect

SocietyConnect is a responsive society-management portal built with React and Vite. It provides role-based screens for residents, society presidents, and administrators to manage complaints, notices, staff, residents, society profiles, and blocks.

## Requirements

- Node.js 20.19+ or 22.12+
- npm (included with Node.js)

## Run locally

From the project directory:

```sh
npm install
npm run dev
```

Open the local URL printed by Vite (usually <http://localhost:5173/>). Stop the development server with `Ctrl+C` in the terminal where it is running.

## Available commands

| Command | Description |
| --- | --- |
| `npm run dev` | Start the local Vite development server |
| `npm run build` | Create the production build in `dist/` |
| `npm run preview` | Serve the production build locally after running the build |
| `npm run lint` | Run ESLint |

To verify a production build:

```sh
npm run build
npm run preview
```

## Features

- Login screen with resident, society president, and admin role selection
- Resident dashboard, complaint submission and tracking, complaint details, and feedback
- President dashboard, complaint review, staff and resident directories, notices, and analytics
- Society profile and block information, with admin management screens
- Responsive layouts and installable-app metadata
- Browser-local persistence for demo data using `localStorage`

## Project structure

```text
public/                  Static assets, app icons, manifest, and service worker
src/
  components/            Shared UI components
  data/                  Demo data and browser-storage operations
  pages/                  Login, resident, president, and society screens
  App.jsx                 Application routes
  main.jsx                React entry point
```

## Demo limitations

This repository is a frontend demo and does not include a server, database, or configured Google sign-in. Society records and changes are stored in the current browser, so they are not shared between users or devices. The login screen and password checks are not a substitute for production authentication; do not use real credentials or sensitive information.
