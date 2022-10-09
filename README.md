# mern-auth-server & mern-auth-client
### template using
#### backend dependencies:
    "body-parser": "^1.20.1",
    "connect-mongodb-session": "^3.1.1",
    "cookie-parser": "^1.4.6",
    "cors": "^2.8.5",
    "dotenv": "^16.0.3",
    "express": "^4.18.1",
    "express-session": "^1.17.3",
    "jsonwebtoken": "^8.5.1",
    "mongoose": "^6.6.5",
    "nodemon": "^2.0.20",
    "passport": "^0.6.0",
    "passport-jwt": "^4.0.0",
    "passport-local": "^1.0.0",
    "passport-local-mongoose": "^7.1.2"

#### frontend dependencies:
    "@blueprintjs/core": "^4.11.2",
    "@testing-library/jest-dom": "^5.16.5",
    "@testing-library/react": "^13.4.0",
    "@testing-library/user-event": "^13.5.0",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-scripts": "5.0.1",
    "web-vitals": "^2.1.4"

## get your .env right:
#### backend .env
* JWT_SECRET = 
* REFRESH_TOKEN_SECRET = 
* SESSION_EXPIRY = 60 * 15
* REFRESH_TOKEN_EXPIRY = 60 * 60 * 24 * 30
* MONGO_DB_CONNECTION_STRING =
* COOKIE_SECRET = 
* WHITELISTED_DOMAINS = http://localhost:3000

##### want to generate some quick secrets? me too! run this command and paste unique ones in that .env:
- `openssl rand -base64 172 | tr -d '\ n'`
- [Read an Article - JSON Web Token (JWT) — The right way of implementing, with Node.js](https://siddharthac6.medium.com/json-web-token-jwt-the-right-way-of-implementing-with-node-js-65b8915d550e)

#### frontend .env
* REACT_APP_API_ENDPOINT = http://localhost:8081/

## steps:
1. ```yarn install``` or ```npm i``` 
2. ```yarn start```
3. add new terminal
4. ```cd mern-auth-client```
5. ```yarn install``` or ```npm i``` 
6. ```yarn start```

# and then what?
* you did it! you set up mongodb, express, react, and node in a full stack application that utilizes passport and jwt for authentication
## gratz
* don't delay start today!
* that means go build
* seriously go build
* stop doing tutorials
* go write some spaghetti code
* make a controller
* continue that MVC architecture
* add CRUD
* go build

#### notes:
* this project uses cookies for storing the jwt
* google chrome will not generate the token with localhost
* in chrome => refreshing the page in development localhost will log you out
* in in firefox and safari => refreshing maintains login state/context while testing in localhost 
