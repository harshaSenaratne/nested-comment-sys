# React Nested Comment System

This comment system module is built using React / Fastify / Prisma & Postgres. 

## Demo

[screen-capture (2).webm](https://user-images.githubusercontent.com/25275596/210443503-db66180f-fef6-4799-bd06-618ac46b8508.webm)

## Prerequisite
You should have postgres installed and you need to have your postgres database already running to connect to it (using the DATABASE_URL).

## Server Configuration
Create a .env file inside the server root folder and add the following variables to it.
```bash
DATABASE_URL="postgresql://postgres:<YOUR_PASSWORD>@localhost:<YOUR_PORT>/<DATABASE_NAME>"
```
```bash
PORT ="<SERVER_PORT>"
```
```bash
CLIENT_URL = http://localhost:3000
```

## Client Configuration
Create a .env file inside the client root folder and add the following variables to it.

```bash
REACT_APP_SERVER_URL = http://localhost:<PORT_THAT_SERVER_IS_RUNNING>
```

## Installation
Go to both client and server root folders individually and run ```npm install``` to install dependencies.

After that in server root folder run the commands to migrate the database ``` npx prisma migrate dev ```   and seed the database with some data ```npx prisma db seed ```  . 

## Usage
To start the client application go to client root folder and run  ``` npm run start ``` &  to start the server run  ```npm run devStart ``` in server root folder.
 
