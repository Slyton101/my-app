# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

[![Deploy to GitHub Pages](https://github.com/Slyton101/my-app/actions/workflows/deploy.yml/badge.svg)](https://github.com/Slyton101/my-app/actions/workflows/deploy.yml)

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.

## Running with Docker

This project includes a multi-stage Docker setup for building and running the app in a production-like environment.

- **Node.js version:** 22.13.1 (slim)
- **Exposed port:** 4173 (Vite preview server)

### Build and run with Docker Compose

To build and start the app using Docker Compose:

```sh
docker compose up --build
```

The app will be available at [http://localhost:4173](http://localhost:4173).

- No environment variables are required by default. If you add a `.env` file, uncomment the `env_file` line in `docker-compose.yml`.
- The container runs as a non-root user for improved security.

If you add additional services (e.g., a database), update `docker-compose.yml` accordingly.
