# Project for Web Development 2023/2024

## MEVN Stack

- MongoDB
- Express.js
- Vue.js
- Node.js

Node.js is required in order to run backend <https://nodejs.org/en/download>.

## Run Backend

`mongod` daemon service must be installed and running in background. Use following command to perform this task.

``` zsh
brew install mongodb-community
brew services start mongodb-community
```

Then `Express.js` server must be started along with MongoDB database.

```zsh
cd backend
node server.js
```

Server backend running on: `http://localhost:8080/`

DB server running on: `mongodb://localhost:27017/mevn-todo_db`

## Run Frontend

Change directory to `frontend` and start server. Follow steps below.
```zsh
cd frontend
npm run serve
```

Application is running on: `http://localhost:8081/`

### REST API Methods

#### POST `/api/tutorials` - creates new TODO

#### GET `/api/tutorials` - retrieves all TODOs

#### GET `/api/tutorials/:id` - retrieves TODO by `id`

#### PUT `/api/tutorials/:id` - updates TODO by `id`

#### DELETE `/api/tutorials/:id` - deletes TODO by `id`

#### DELETE `/api/tutorials` - deletes all TODOs

#### GET `/api/tutorials?title=[keyword]` - searches `keyword` in title in all TODOs
