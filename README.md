# George's Music Library Project

## Introduction

This is a music libary API built with NODE JS, Express, interacting with PostgreSQL. The user can create, read, update and delete both artists and albums in the database. This project does not have a GUI, I reccomend using postman to [Postman](https://www.postman.com/downloads/) to interact with the API.


## Quick Start and Commands

1. Clone the repo:

```bash
git clone https://github.com/george-xixi/music-library.git
```
2. Initialise npm:

```bash
npm init
```

3. Install dev dependecies

The relevant dev dependencies are:

```bash
npm i -D dotenv
```
```bash
npm i -D chai
```

```bash
npm i -D mocha
```
```bash
npm i -D supertest
```
4. Create file with enviroment variables 

create .env and .env.test file in root directory 
```bash
touch .env
```

```bash
touch .env.test
```

In the .env files, these are the variables you need:
PGUSER=
PGHOST=
PGPASSWORD=
PGDATABASE=(make sure this is different in .env and .env.test)
PGPORT=
PORT=(optional, but this will default to 4000 if you don't choose)

5. To run tests:

```bash
npm test
```

4. Download Postman and pgAdmin 

- [Postman](https://www.postman.com/downloads/)
- [pgAdmin](https://www.pgadmin.org/download/)


## API Endpoints and Methods

Artists endpoints and methods

| **Methods** |   **Urls**   |     **Actions**      |
| :---------- | :----------: | :------------------: |
| GET         |   /artists   |   get all artists    |
| GET         | /artists/:id |   get artist by id   |
| POST        |   /artists   |    add new artist    |
| PUT         | /artists/:id | update artist by id  |
| DELETE      | /artists/:id | remove artists by id |

Albums endpoints and methods

| **Methods** |        **Urls**         |              **Actions**              |
| :---------- | :---------------------: | :-----------------------------------: |
| GET         |         /albums         |            get all albums             |
| GET         |       /albums/:id       |            get album by id            |
| POST        | /artists/:artistId/album| add new albums to the specific artist |
| PUT         |       /albums/:id       |          update album by id           |
| DELETE      |       /albums/:id       |          remove album by id           |
