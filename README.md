# Customer CRUD (React + Vite + json-server)

A small full-stack-feeling CRUD app: a React frontend for viewing, searching,
adding, editing, and deleting customer records, backed by a `json-server`
mock REST API. Built as a React data-fetching / state-management exercise.

## Stack

- React 18 + Vite
- Tailwind CSS
- TanStack Query (`@tanstack/react-query`) for data fetching, caching, and mutations
- Axios
- `json-server` as a mock REST backend

## Features

- List customers in a searchable, paginated table
- View a single customer's details
- Add a new customer
- Edit an existing customer
- Delete a customer

## Getting started

Install dependencies:

```bash
npm install
```

Start the mock API (serves data from `customers.json` on `http://localhost:3000`):

```bash
npx json-server --watch customers.json
```

In a separate terminal, start the frontend:

```bash
npm run dev
```

Vite will print the local URL (typically `http://localhost:5173`).

## Project structure

```
src/
├── components/    # Layout, nav, and the main CRUD table
├── user/          # Add / Edit / View pages for a single customer
└── assets/        # Images
```

## Notes

`customers.json` contains fake data generated for development purposes only
(via [`@faker-js/faker`](https://fakerjs.dev/)) — no real customer
information is used anywhere in this project.
