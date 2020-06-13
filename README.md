# Course-Review basic setup
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

## Weekly Goals

This is a fun project that allows users to rate courses from various colleges and review them. We would want our application to be able to produce a User Interface through which a person will be able to interact to view reviews and comment on the courses of a college. We would also want the user to log in so that only a logged-in user can comment and rate a course.

If you already have experience with these languages/frameworks and finish the goals ahead, feel free to go ahead with the next sections and even try the bonus implementations :)

### Week 1
Let's get started!

* Make sure that you are able to set up the project and run it.
* Learn how to use [Postman](https://www.postman.com/). Postman is an industry-standard tool that allows users to communicate with the backend server APIs. Check out this [Tutorial](https://www.guru99.com/postman-tutorial.html) which is really helpful if you have never had any experience with it.
* Server (Backend)
  1. This is the first week and we are just getting started so let’s start with something small. In the backend, first, ensure that your node server is able to connect to the MongoDB database. Use this detailed Tutorial to give you an idea about how to set things up.
  2. Now, create a simple API endpoint that will store college, department, course number, and its related rating(number)  and comments (string) which indicates the rating of a course and store it in the database.
* Client (FrontEnd)
  1. Create a way for users to input a college’s name, department name, the course number, and its associated rating. This will call the API in the backend so that the data will be stored. For now, the UI can be a very simple single page.


### Week 2
Let's build apis for our core feature

* Add APIs so that given a college, department, and course, the user will be able to retrieve a given review/ comments.
* Add APIs so that the reviews are editable. (At this point, anyone can edit any review but we will take care of that later!)
* Also, think about how filtering is done. For example, when a user inputs the college name, you need to provide all  departments along with their courses. The user will then be able to select a course and view/edit the reviews and comments.
See example for inspiration: [Rate My Professors](https://www.ratemyprofessors.com/)
* Test that your API endpoints using postman to ensure that that they are working properly. When you test, make sure you are covering the edge cases and testing in detail. We aren't writing any formal unit tests so this is a good chance to ensure you do not have any bugs in your code.

### Week 3
* Create web pages that already allows users to input a college name. 
* Given a college name, the users will be taken to a new webpage that shows a list of departments with courses from which a user can select a course.
* Make sure that the courses can be viewed/edited.

**Bonus**
* If you want your webpage to be more dynamic looking and cool, let your imagination run free. Take inspiration from various sources so that you can and create beautiful webpages. 
* Take inspiration from [Dribbble](https://dribbble.com/) and [Uplabs](https://www.uplabs.com/)

### Week 4
Now that people can actually comment and review about a course, we want the users to not be able to spam random comments and reviews to courses. We want the reviews to be genuine so one way to do this is to ensure that the users are signed up in our platform and only allow logged-in users to rate and review a course.

* Learn about JWT. For this week, concentrate on learning and ensure that you have a clear understanding of what JWT is. 
* Take a look at Passport.JS. It is a very popular authentication middleware for Node.js. (It is recommended to use popular existing packages like Passport.js for  authentication as they are thoroughly tested and cover lots of edge cases). If you want to use a different package go ahead and use them but make sure that you understand what is going on very well. 

__Some helpful tutorials__:
* [Express.Js App With Passport.Js and Mongodb](https://medium.com/swlh/set-up-an-express-js-app-with-passport-js-and-mongodb-for-password-authentication-6ea05d95335c)
* [Implementing JSON Web Tokens & Passport.js in a JavaScript Application with React](https://itnext.io/implementing-json-web-tokens-passport-js-in-a-javascript-application-with-react-b86b1f313436)

### Week 5
Now that we have some knowledge of how JWT works, let's use it on our application for authentication.

* Create a basic authentication system where any users will be able to sign up using a full name, email, and a password. The users will later be authenticated with their email and password when they attempt to login to the site. Use JWT to authenticate your user.
(It is recommended to use popular existing packages like Passport.js for  authentication as they are thoroughly tested and cover lots of edge cases). If you want to use a different package go ahead and use them but make sure that you know how it's working.
* Ensure that only an authenticated user can review/edit a course in our application. Any user that is not logged in should be only able to view the reviews.

__Some helpful tutorials__:
* [Express.Js App With Passport.Js and Mongodb](https://medium.com/swlh/set-up-an-express-js-app-with-passport-js-and-mongodb-for-password-authentication-6ea05d95335c)
* [Implementing JSON Web Tokens & Passport.js in a JavaScript Application with React](https://itnext.io/implementing-json-web-tokens-passport-js-in-a-javascript-application-with-react-b86b1f313436)

**Bonus:**

Make sure that the users that sign up are valid college students. Send an email to a user's college email address to validate whether a user is from a certain college or not.

__Some helpful tutorials:__
[Sending emails with Node](https://stackabuse.com/how-to-send-emails-with-node-js/)

### Week 6
Now that we have the APIs in the server that handles all the authentication details, let's create some beautiful forms through which users can log in and sign up.

* Create two frontend pages that allow new users to signup and existing users to login.  (You could use Formik and Yup to make your life easier).
* Ensure that the theme(colors) of these pages are aligned with webpages that you created earlier. Be creative with your design. Take inspiration from Dribbble and Uplabs as before.


**Bonus:**

* Add a forgot password button that sends an email to users with a new verification code and redirects users to a new page that allows users to reset the password.
* Instead of Users adding a college by themselves, have the field pre-populated with all the colleges in the US. Use an external API to get a list of colleges so that the user can simply select a college from a dropdown. The users will then be taken to a college home page with its departments and its courses. The user will then be able to select the course as before and then view/edit it. (This activity requires a good amount of time investment, research, and data manipulation skills. If you have not finished any of the previous goals, please finish them and come to this bonus later.)

Some external API or data sources:
* [University Domain List](https://github.com/Hipo/university-domains-list/)
* [Universities Worldwide](https://github.com/endSly/world-universities-csv/)

 
