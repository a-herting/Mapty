# Mapty

Introductory project that demonstrates object oriented programming, along with other features like geolocation and utilizing local storage to store app information locally. 

The Mapty app displays a map and records the location the user selects on the map along with details about the workout (running or cycling, distance, duration, elevation, pace or cadence).

In the script.js file, we have the app class defined with the following constructor methods: getPosition and getLocalStorage. Inside of the class, we use the following key methods:

 - **_getPosition** ( ): Method used for capture user workout location via geolocation. 
 - **_loadMap** (position): Method used for loading the map with a marker for each recorded workout. 
- **_newWorkout** (position): Method used for creating a new workout by first capturing the form data (type, distance, duration, coordinates). Based upon the type of the workout determines if cadence or elevation gain are displayed. We then set the workout variable to be an object of the class specified (cycling or running). The new workout is pused to the wokrout array and is rendered in the list UI to the left of the page and as a marker on the map. 
