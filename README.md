# Comments Service
 Microservice to manage comments

## Features
- [XSS](https://en.wikipedia.org/wiki/Cross-site_scripting) Protection (via [sanitize-html](https://www.npmjs.com/package/sanitize-html))
- Flags spam (via [Akismet](https://akismet.com/))

## Running Locally
- [Git](https://git-scm.com/downloads)
- [Node Js](https://nodejs.org/en/)
- [MongoDB](https://www.mongodb.com/) (To use the Mongo DB interface, you need to install Mongo Compass)

#### 1. Clone the repo and install dependencies
```bash
git clone 
cd comments-service
npm i
```

#### 2. Modify the .env file
Save `sampledotenv` as `.env` and then add your database and Akismet API details.

#### 3. Startup your MongoDB
Usually this is just: `mongod` on the command line.

#### 4. Start the server
To run in production mode where code is transpiled by Babel into a `dist` folder and run directly in `node`:
```bash
npm start
```

To run in development mode where code is run by [babel-node](https://babeljs.io/docs/en/babel-node) via [nodemon](https://nodemon.io) and re-transpiled any time there is a change:
```bash
npm run dev
```
