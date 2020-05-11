# app-test

A user creation test application :bug: :bar_chart: :clipboard:

## Created with

* [Node.js](https://nodejs.org/en/)
* [Jest](https://jestjs.io/)
* [Docker](https://www.docker.com/)
* [PostgreSQL](https://www.postgresql.org/)
* [Factory Girl](https://www.npmjs.com/package/factory-girl)

## How to use this

### On windows

```json
"pretest": "set NODE_ENV=test && sequelize db:migrate",
"test": "set NODE_ENV=test && jest",
"posttest": "set NODE_ENV=test && sequelize db:migrate:undo:all"
```

### Linux or MAC

```json
"pretest": "NODE_ENV=test sequelize db:migrate",
"test": "NODE_ENV=test jest",
"posttest": "NODE_ENV=test sequelize db:migrate:undo:all"
```

### After settings

``yarn install or npm install``

``yarn test or npm test``
