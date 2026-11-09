# Life CRM

Life CRM is a modern, extensible CRM platform built with React, NestJS, and PostgreSQL.

## Architecture

- **Frontend**: React, TypeScript, Vite, Apollo GraphQL (`packages/twenty-front`)
- **Backend**: NestJS, TypeScript, TypeORM, PostgreSQL (`packages/twenty-server`)
- **UI Library**: Shared design system and components (`packages/twenty-ui`)
- **Shared**: Core types, constants, and utilities (`packages/twenty-shared`)
- **Deployment**: Docker Compose infrastructure (`packages/twenty-docker`)

## Quick Start (Docker)

To run the application locally using Docker:

```bash
docker compose -f packages/twenty-docker/docker-compose.yml --env-file packages/twenty-docker/.env up -d
```

Access the application in your browser at:
`http://localhost:3000`

## Structure

```
Life-crm/
├── packages/
│   ├── twenty-front/                   # Web frontend application
│   ├── twenty-server/                  # Backend API and server
│   ├── twenty-ui/                      # UI component library
│   ├── twenty-shared/                  # Shared data models and logic
│   ├── twenty-docker/                  # Docker Compose configuration
│   ├── twenty-emails/                  # Email templates
│   ├── twenty-front-component-renderer/# Dynamic front components
│   ├── twenty-utils/                   # Shared utility functions
│   └── twenty-sdk/                     # Client SDK
├── nx.json                             # Monorepo build orchestrator
└── package.json                        # Monorepo configuration
```
