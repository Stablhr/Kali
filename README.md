# Kali (SchedFlow)

A social media content planning and scheduling app built with React 19, TypeScript, and Tailwind CSS. Plan posts across a weekly time grid, drag-and-drop between time slots, manage boards, and track engagement insights — all in one place.

## Tech Stack

- [React 19](https://react.dev) + [Vite](https://vite.dev)
- [TypeScript](https://www.typescriptlang.org)
- [Tailwind CSS v4](https://tailwindcss.com)
- [@hello-pangea/dnd](https://github.com/hello-pangea/dnd)
- [React Router v7](https://reactrouter.com)
- [Lucide React](https://lucide.dev) icons

## Getting Started

```bash
npm install
npm run dev
```

## Available Scripts

| Command           | Description                          |
| ----------------- | ------------------------------------ |
| `npm run dev`     | Start the Vite dev server            |
| `npm run build`   | Type-check (`tsc -b`) + production build |
| `npm run lint`    | Lint with Oxlint                     |
| `npm run preview` | Preview the production build         |

## Commit Conventions

This project follows the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) specification. Commit messages should use the following structure:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

Common types:

- **feat** — a new feature
- **fix** — a bug fix
- **docs** — documentation only changes
- **style** — formatting, missing semicolons, whitespace; no code change
- **refactor** — code change that neither fixes a bug nor adds a feature
- **perf** — a performance improvement
- **test** — adding or updating tests
- **chore** — build tooling, dependencies, miscellaneous maintenance
- **revert** — revert a previous commit

Examples:

```
feat: add resizable calendar width on content planner
fix(sidebar): keep navigation tooltip aligned on collapse
docs: update commit conventions reference
```

See the full specification at [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/).
