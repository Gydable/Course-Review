# React - Express basic setup
This repository has the basic bare bones code to run a React Frontend and Node/Express Backend and running them together. The project uses MongoDB as the database storage.

## Hosting and connecting the MongoDB database
Since we are using MongodDB database, we will need to create a cluster. Go over this awesome [blog post](https://www.mongodb.com/blog/post/quick-start-nodejs-mongodb--how-to-get-connected-to-your-database) that clearly explains how to host a MongoDB cluster and set it up with NodeJS.

## Download and install tools
1. [VS Code](https://code.visualstudio.com/) (Recommended but not required)

## The APP
The app combines two separate applications. Client which serves the FrontEnd (using React), and the API (in Node/Express)

## How to run both the servers together
1. Clone the repository.
2. Open your terminal and navigate to the root directory (course-review).
3. Run `npm run installation` to install all dependencies.
4. Run `npm run dev`.

## How to run the Node server seperately
1. In your terminal, navigate to the api directory.
2. Run `npm install` to install all dependencies.
3. Run `npm start` to start the app.

## How to run the Client seperately
1. In a different terminal, navigate to the client directory.
2. Run `npm install` to install all dependencies.
3. Run `npm start` to start the app.

## Make sure they are running
1. With the two apps running, open your browser in http://localhost:3000/.
2. If you see a webpage saying Welcome to React, it means the FrontEnd is working.
3. If the same webpage has the phrase API is working properly, it means the API is working too!
4. Enjoy coding!
