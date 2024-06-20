## Prerequisites
- [Node.js](https://nodejs.org/en/) (used v21.6.0 for development)
- [NestJS CLI](https://docs.nestjs.com/cli/overview) (optional, but recommended)
- [MongoDB](https://www.mongodb.com/) (either local or cloud-based)
## Getting Started
### Installation
1. Install the dependencies:
    ```bash
    npm install
    ```
2. Rename a `.env-example` to `.env` file at the root of the project and add the following environment variables:
    ```env
    APP_PORT=3000
    ExpiresIn=60
    NODE_ENV=development
    for dev or production url
    DATABASE_TYPE=mongodb
    DATABASE_PORT=27017
    DATABASE_USERNAME=root
    DATABASE_PASSWORD=secret
    DATABASE_NAME=api
    DATABASE_URL=mongodb://mongo:27017
    for auth
    Replace `your_secret_key` with a strong secret key.
     
    AUTH_JWT_SECRET=secret
    AUTH_JWT_TOKEN_EXPIRES_IN=15m
## Run microservice offline, watching changes in realtime local development
```
npm run start:dev
By default run project on 3000
there is message server started that application running successfully
```
## Build NestJS app for production enviroment
```
nest build 
```