
# User API Web Application

This is a basic Node.js web application exposing a REST API that creates and stores user parameters in a Redis database.

## Functionality

1. Start a web server.
2. Create a user.

## Installation

This application is written in Node.js and uses a Redis database.

### 1. Install Node.js

Download and install Node.js:

https://nodejs.org/

### 2. Install Redis

Download and install Redis:

https://redis.io/download

### 3. Install the application

Go to the root directory of the application (where the `package.json` file is located) and run:

```bash
npm install
```

## Usage

### 1. Start the web server

From the root directory of the project, run:

```bash
npm start
```

The web server will be available in your browser at:

http://localhost:3000

### 2. Create a user

Send a POST request using the terminal:

```bash
curl --header "Content-Type: application/json" \
  --request POST \
  --data '{"username":"sergkudinov","firstname":"sergei","lastname":"kudinov"}' \
  http://localhost:3000/user
```

Expected output:

```json
{"status":"success","msg":"OK"}
```

Another way to test your REST API is to use Postman:

https://www.postman.com/

## Testing

From the root directory of the project, run:

```bash
npm test
```

## DSTI DevOps Lab

Repository: dsti-userapi-cicd

This project is part of the DSTI DevOps lab on Continuous Integration and Continuous Delivery.
