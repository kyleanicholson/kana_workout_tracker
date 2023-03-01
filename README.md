# kana_workout_tracker
The purpose of this project is to build a workout tracker web application using Node.js, Express, and MongoDB. The application will allow users to create and log workouts, as well as view their workout history.

At a high level, the application will be executed by first setting up the server using Express, connecting to a MongoDB database, and setting up the necessary API routes to handle user authentication and workout creation/logging. The application will also use EJS templates to render views to the user, and implement client-side JavaScript to handle user interaction.

In order to allow users to create and log workouts, the application will utilize Mongoose to define and interact with three models: Exercise, Workout, and User. The Exercise model will store details about individual exercises, while the Workout model will contain a collection of exercises and a reference to the user who created it. The User model will store user authentication information, as well as a collection of workouts.

The application will also include user authentication and authorization, implemented using Passport.js and JSON Web Tokens (JWTs). When a user logs in, a JWT will be generated and stored on the client-side, which will allow the user to access protected routes that require authentication.

Overall, the project will be a full-stack web application that utilizes Node.js, Express, MongoDB, Mongoose, EJS, client-side JavaScript, Passport.js, and JWTs to create a functional workout tracker application with user authentication and authorization.
