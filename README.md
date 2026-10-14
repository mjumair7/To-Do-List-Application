# To-Do List

A small Express app for adding, listing, and deleting tasks from a browser.

I built this to practice the basic request cycle between a front end and a Node.js server: the page sends JSON requests, Express updates the task list, and the browser redraws the result.

## Run it

Requirements: Node.js and npm.

```sh
npm install
node app.js
```

Open <http://localhost:1200>.

## API

- `GET /tasks` returns the current task list.
- `POST /tasks` accepts `{ "task": "..." }`.
- `DELETE /tasks/:index` removes one task by its array index.

## Current limits

Tasks are stored in memory, so restarting the server clears the list. There is no user account, database, edit state, or automated test suite. This is a learning project rather than a production task manager.
