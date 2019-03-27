# Project-skeleton

## Tech

- TypeScript
- Frontend
  - React
  - Redux
- Backend
  - Express
- Database
  - none
- Docker-compose
  - currently from database only

## Installation

- Clone project
- Go to project root
- Install dependencies `npm install`
- Set up database
  - Start a container with postgres instance
    - `docker-compose up -d`
  - Define schemas
    - `psql "postgresql://todoapplicationdev:passwd@localhost:2345/tododbdev" --file ddl.sql`
  - Seed the database
    - `psql "postgresql://todoapplicationdev:passwd@localhost:2345/tododbdev" --file seed.sql`
  - Test it works
    - `psql "postgresql://todoapplicationdev:passwd@localhost:2345/tododbdev" -c "SELECT * FROM todoapp.task"`
- Run development server `npm start`
- Open browser [http://localhost:3000/](http://localhost:3000/)

## Licence

[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)