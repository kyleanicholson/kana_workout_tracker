# Program Notes
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
