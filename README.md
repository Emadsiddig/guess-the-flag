# Postgres Quiz App

A small Node.js/Express quiz application that reads quiz questions from a PostgreSQL database and renders them with EJS.

## Features

- Express server with EJS rendering
- PostgreSQL connection using `pg`
- Environment-based database configuration with `.env`
- Static files served from `public/`
- Quiz validation and scoring

## Project structure

- `index.js` — main application entry point
- `package.json` — project dependencies and metadata
- `.env` — local configuration (not committed)
- `.gitignore` — excludes `node_modules` and `.env`
- `views/index.ejs` — page template
- `public/` — static assets
- `flags.csv` — quiz data source (if needed)

## Setup

1. Install dependencies:

```bash
npm install
```

2. Create a `.env` file in this directory with values like:

```env
DB_USER=postgres
DB_PASSWORD=Print1482@
DB_HOST=localhost
DB_NAME=world
DB_PORT=5432
PORT=3000
```

3. Make sure PostgreSQL is running and the `world` database contains the `flags` table.

4. Start the server:

```bash
node index.js
```

5. Open the app in your browser:

```text
http://localhost:3000
```

