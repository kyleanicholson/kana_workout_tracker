# Program Specifications

## Front End Specs
### Home Page (Dashboard)
* The home page will display a dashboard with a list of the user's recent workouts and performance data along with buttons to create new workouts or view historical workouts.
  - Performance Metrics Chart: The performance metrics chart would display the user's progress over time, showing how their performance has improved (or declined) over time for specific exercises.
  - Overall, the process for implementing graphs to display user workout data involves involve collecting and storing the data in the database, retrieving the data from the database, formatting it for use with a charting library (Chart.js or D3.js), and then displaying the graph to the user.
### Create Workout Page
The create workout page allows the user to create a new workout by selecting exercises and adding details such as the number of sets/reps, weight, and RPE.
### View Workout Page
Display details about a specific workout, including the exercises performed, the weights lifted, and the user's performance metrics.
### Exercise Selector
Allow the user to choose from a list of predefined exercises or add new ones to their workout.
### Performance 


## DB Structure
### User Model:
* username (string)
* email (string)
* password (string)
* workouts (array of ObjectIds referencing the Workout Model)
### Workout Model:
* name (string)
* date (Date)
* exercises (array of ObjectIds referencing the Exercise Model)
### Exercise Model:
* name (string)
description (string)
* sets (array of Objects)
* weight (number)
* reps (number)
* rpe (number, 1-10)

#### Details
To create a new workout, create a new instance of the Workout model and add it to the User's workouts array. To add exercises to the workout, you would create new instances of the Exercise model and add them to the workout's exercises array. To add sets to an exercise, you would push new Objects containing weight, reps, and rpe to the exercise's sets array.
