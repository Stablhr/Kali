# 🗂️ Kali — Social Content Planner

## 📖 Project Overview

Kali is a social media content planning and scheduling app. It provides a weekly time-grid content planner where you can drag posts into time slots, manage boards with multiple views, keep track of your inbox, and get an at-a-glance dashboard of what's coming up.

This project is a single React SPA (frontend only) built with **React 19**, **TypeScript**, and **Tailwind CSS v4**, backed by a local store with optional MongoDB/Blob integrations.

### Key Features

- **Dashboard** — At-a-glance overview of boards, due-soon items, and planner previews.
- **Inbox** — Incoming items with quick actions.
- **Boards** — Kanban boards with board views: **Board**, **Calendar**, **Table**, **Timeline**, and **Map**.
- **Schedule** — Day-column planner with drag-and-drop between days and an unscheduled pool.
- **Content Planner** — Weekly time grid (6 AM – 11 PM) to schedule social posts by hour; drag posts between slots and the unscheduled pool.
- **Social** — Compose modal, bulk scheduling, analytics, media library, webhooks, and OAuth account connection (YouTube, Facebook, Instagram, TikTok).
- **Theme** — Light & dark mode with adaptive surfaces.

## 🛠️ Tech Stack

| Layer       | Technology                                     |
| ----------- | ---------------------------------------------- |
| Framework   | React 19                                       |
| Language    | TypeScript                                     |
| Build tool  | Vite 8                                         |
| Styling     | Tailwind CSS v4                                |
| Routing     | React Router v7                                |
| Drag & drop | @hello-pangea/dnd                              |
| Icons       | Lucide React                                   |
| Linter      | Oxlint                                         |

## 📁 Project Structure

```
/
├── public/            # Static assets
├── src/
│   ├── assets/        # Images & logos
│   ├── components/    # UI components
│   │   ├── auth/          # Sign in / sign up
│   │   ├── boards/        # Boards, lists, cards & views
│   │   ├── card-modal/    # Card detail modal & fields
│   │   ├── common/        # Shared adaptive components
│   │   ├── content-planner/  # Weekly time grid planner
│   │   ├── dashboard/     # Home dashboard
│   │   ├── dev/           # Dev/test pages
│   │   ├── inbox/         # Inbox view
│   │   ├── layout/        # Sidebar, app shell
│   │   ├── planner/       # Day-column schedule planner
│   │   ├── shared/        # Buttons, inputs, modals, skeletons
│   │   └── social/        # Compose, analytics, social calendar
│   ├── hooks/         # Theme & adaptive hooks
│   ├── lib/           # API clients, feature hooks
│   ├── store/         # Data store, schema & persistence
│   ├── utils/         # Date, color, format helpers
│   ├── App.tsx        # Routes & app entry
│   └── main.tsx       # Bootstrap
├── .env.example       # Environment variables template
├── index.html
├── package.json
└── vite.config.ts
```

## ⚙️ Prerequisites

- Node.js 18+
- npm
- Git

## 🚀 Getting Started

### 1. Clone the repository

```sh
git clone https://github.com/Stablhr/Schedflow.git
cd SchedFlow
```

### 2. Install dependencies

```sh
npm install
```

### 3. Configure environment variables

```sh
cp .env.example .env.local   # add your OAuth keys, MongoDB URI, etc.
```

### 4. Start the dev server

```sh
npm run dev
```

The app runs on: `http://localhost:5173`

## 📜 Available Scripts

| Command           | Description                            |
| ----------------- | -------------------------------------- |
| `npm run dev`     | Start the Vite dev server              |
| `npm run build`   | Type-check (`tsc -b`) + production build |
| `npm run preview` | Preview the production build           |
| `npm run lint`    | Lint with Oxlint                       |

## 🌿 Git Branching Workflow

### Branch Structure

```
main
└── feature/<short-description>
    ├── fix/<short-description>
    ├── hotfix/<short-description>       # (urgent production fixes)
    └── chore/<short-description>        # (configs, deps, refactors)
```

| Type     | Pattern                      | Example                |
| -------- | ---------------------------- | ---------------------- |
| Feature  | `feature/<short-description>` | `feature/content-planner` |
| Bug Fix  | `fix/<short-description>`    | `fix/sidebar-tooltip`  |
| Hotfix   | `hotfix/<short-description>` | `hotfix/login-redirect`|
| Chore    | `chore/<short-description>`  | `chore/update-deps`    |

### Starting a new feature

```sh
# 1. Make sure main is up to date
git checkout main
git pull origin main

# 2. Create your branch
git checkout -b feature/content-planner

# 3. Work on your changes, then commit
git add .
git commit -m "feat: add content planner calendar"

# 4. Push your branch
git push origin feature/content-planner
```

### Merging back to main

Open a Pull Request (`feature/...` → `main`) and get it reviewed before merging.

## 📝 Commit Message Convention

This project follows [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/):

```
<type>[optional scope]: <description>
```

| Type       | Description                          |
| ---------- | ------------------------------------ |
| `feat`     | New feature                          |
| `fix`      | Bug fix                              |
| `chore`    | Maintenance, deps, config            |
| `style`    | Formatting, no logic change          |
| `refactor` | Code restructure, no behavior change |
| `perf`     | Performance improvement              |
| `test`     | Adding or updating tests             |
| `docs`     | Documentation updates                |
| `revert`   | Revert a previous commit             |

Examples:

```sh
git commit -m "feat: make content planner calendar resizable"
git commit -m "fix(sidebar): keep tooltip aligned on collapse"
git commit -m "chore: update react to v19"
git commit -m "docs: update README setup steps"
```

See the full specification at [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/).

## 🤝 Contributing

- Branch off `main` using the branch naming above.
- Follow the commit message convention.
- Open a Pull Request into `main`.
- Request a code review before merging.