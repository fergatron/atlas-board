# Atlas Board

This project is a demo of different ways to visual flight data in the flight simulation space. The app is comprised of a React/TypeScript front end and Node backend talking to a relational and document databases.

## Tech Stack

| Layer | Stack | Purpose |
| --- | --- | --- |
| Frontend | React 19, TypeScript, Vite, Tailwind | Modern dashboard SPA, fetches data from Express API. |
| Backend | Node.js (Express) + TypeScript | REST API with routes for auth, projects, and documents. |
| Relational DB | PostgreSQL | Stores structured entities: users, projects, permissions. |
| Document DB | MongoDB | Stores flexible documents, notes, or project data. |
| Auth | JWT (with bcrypt password hashing) | Login/register endpoints + token-based access. |
| Storage | Local uploads or AWS S3 mock | For document attachments. |
| DevOps | Docker + docker-compose + GitHub Actions | Run PostGres + Mongo locally, build/test pipeline. |

This project is a monoreop with package management (npm workspaces).

* Build tool (frontend): Vite