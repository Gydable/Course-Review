# React - Express basic setup
This repository has the basic bare bones code to run a React Frontend and Node/Express Backend and running them together. The project uses MongoDB as the database storage.

## Pre-requisites:
* Create a Github account if you don’t have one.
* If you don’t have Git installed in your computer,  install Git using this guide. [Git - Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
* This a template repository. So, you will fork this repository in your GitHub account before working on it. This will give you a complete ownership of your code. To fork this project, click on the Fork button on the top right corner.
* Once you have the forked project, you will clone it to your computer to get started. To clone the project, click on the green “Clone or Download” button and follow the instructions.
* Learn about GitHub and Git commands. We will use git throughout the program, so make sure you have basic understanding of GIT.
* We will use Visual Studio Code as a text editor. If you have a different preference like Sublime Text, Atom etc., feel free to stick with it. Install [Visual Studio Code](https://code.visualstudio.com/) 


## Hosting and connecting the MongoDB database
Since we are using MongodDB database, we will need to create a cluster. Go over this awesome [blog post](https://www.mongodb.com/blog/post/quick-start-nodejs-mongodb--how-to-get-connected-to-your-database) that clearly explains how to host a MongoDB cluster and set it up with NodeJS.

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
