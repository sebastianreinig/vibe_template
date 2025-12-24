# Project Context

> [!IMPORTANT]
> This file provides essential context for AI agents working on this project. Update it as the project evolves.

## Project Overview

**Name:** [Your Project Name]  
**Purpose:** [Brief description of what this project does]  
**Status:** [Development / Alpha / Beta / Production]

## Technology Stack

> [!TIP]
> Defining your tech stack upfront helps AI agents make consistent, compatible recommendations.

### Frontend
- **Framework:** [e.g., React, Vue, Angular, Svelte]
- **Language:** [e.g., TypeScript, JavaScript]
- **Styling:** [e.g., Tailwind CSS, CSS Modules, Styled Components]
- **State Management:** [e.g., Redux, Zustand, Context API]
- **Build Tool:** [e.g., Vite, Webpack, Next.js]

### Backend
- **Runtime/Framework:** [e.g., Node.js/Express, Python/FastAPI, Go/Gin]
- **Language:** [e.g., TypeScript, Python, Go, Rust]
- **Database:** [e.g., PostgreSQL, MongoDB, SQLite]
- **ORM/Query Builder:** [e.g., Prisma, SQLAlchemy, TypeORM]

### Infrastructure
- **Containerization:** [e.g., Docker, Podman]
- **Orchestration:** [e.g., Kubernetes, Docker Compose]
- **CI/CD:** [e.g., GitHub Actions, GitLab CI, Jenkins]
- **Hosting:** [e.g., Vercel, AWS, Azure, GCP]

## Architecture

### High-Level Overview

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│    Frontend     │────▶│     Backend     │────▶│    Database     │
│   (Client)      │◀────│     (API)       │◀────│   (Storage)     │
└─────────────────┘     └─────────────────┘     └─────────────────┘
```

### Directory Structure

```
project-root/
├── frontend/          # Frontend application
├── backend/           # Backend services
├── shared/            # Shared types/utilities
├── docs/              # Documentation
├── .devcontainer/     # DevContainer configurations
└── agents/            # AI agent configuration
```

## Key Conventions

### Code Style
- [e.g., Use ESLint + Prettier for frontend]
- [e.g., Use Black + isort for Python]
- [e.g., Maximum line length: 100 characters]

### Naming Conventions
- **Files:** [e.g., kebab-case for files, PascalCase for components]
- **Variables:** [e.g., camelCase]
- **Constants:** [e.g., SCREAMING_SNAKE_CASE]
- **Database:** [e.g., snake_case for tables and columns]

### Git Workflow
- **Branch naming:** [e.g., feature/, bugfix/, hotfix/]
- **Commit messages:** [e.g., Conventional Commits]
- **PR process:** [e.g., Required reviewers, CI checks]

## Important Decisions

| Decision | Rationale | Date |
|----------|-----------|------|
| [e.g., Chose PostgreSQL over MongoDB] | [e.g., Need for complex queries and transactions] | [YYYY-MM-DD] |

## External Dependencies

- **APIs:** [List any external APIs the project uses]
- **Services:** [List external services like auth providers, payment gateways]

## Known Limitations

- [Document any known limitations or technical debt]
