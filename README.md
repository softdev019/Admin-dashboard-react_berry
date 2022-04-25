

## Quick Start in [Docker](https://www.docker.com/)

> Get the code

```bash
$ cd react-berry-dashboard
```

> Start the app in Docker

```bash
$ docker-compose pull  # download dependencies 
$ docker-compose build # local set up
$ docker-compose up    # start the app 
```

The React UI starts on port `3000` and expects an API server on port `5000` (saved in configuration).

<br />

![React Nodejs Berry - Open-source full-stack seed project crafted by CodedThemes and AppSeed.](https://user-images.githubusercontent.com/51070104/137620059-07547eb2-0e7c-45e3-b825-67f5c72e4d3e.gif)


## How to use it

To use the product Node JS (>= 12.x) is required and GIT to clone/download the project from the public repository.

**Step 1** - Clone the project

```bash
$ git clone https://github.com/app-generator/react-berry-dashboard.git
$ cd react-berry-dashboard
```

<br >

**Step 2** - Install dependencies via NPM or yarn

```bash
$ npm i
// OR
$ yarn
```

<br />

**Step 3** - Start in development mode

```bash
$ npm run start 
// OR
$ yarn start
```

<br />

## Configure the backend server

The product comes with a usable JWT Authentication flow that provides only the basic requests: login/logout/register. 

**API Server URL** - `src/config/constant.js` 

```javascript
const config = {
    ...
    API_SERVER: 'http://localhost:5000/api/'  // <-- The magic line
};
```

<br />

**API Server Descriptor** - POSTMAN Collection

The API Server signature is provided by the [Unified API Definition](https://docs.appseed.us/boilerplate-code/api-unified-definition)


<br />

## Node JS API Server

The product is also open-source and is already configured to work with Berry Dashboard Template - product features:

- Typescript / `NodeJS` / `Express` Server
- JWT authentication (`passport-jwt` strategy)
- Persistence: `SQLite` / `TypeORM`

<br />

![Node JS API - Open-source API server built on top of Express Nodejs Framework.](https://user-images.githubusercontent.com/51070104/124934824-c210a700-e00d-11eb-9d01-e05bd8bfb608.png)

<br />

### Compile the API Server

**Step 1** - Clone the project

```bash
$ cd api-server-nodejs
```

**Step #2** - Install dependencies via NPM or Yarn

```bash
$ npm i
// OR
$ yarn
```

**Step 3** - Run the SQLite migration via TypeORM

```
$ npm run typeorm migration:run
// OR 
$ yarn typeorm migration:run
```

**Step 4** - Start the API server (development mode)

```bash
$ npm run dev
// OR
$ yarn dev
```

The API server will start using the `PORT` specified in `.env` file (default 5000).

<br /> 

---
[React Node JS Berry](https://appseed.us/product/react-node-js-berry-dashboard) - Provided by [CodedThemes](https://codedthemes.com/) and **AppSeed [App Generator](https://appseed.us/app-generator)**.
