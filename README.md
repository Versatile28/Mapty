#  Mapty - Workout Tracking App

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
  - [Built with](#built-with)
  - [Description](#Description)
  - [System Design](#System-design)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

Mapty is a workout tracking app designed using HTML, CSS, and JavaScript. It integrates geolocation and local storage to provide a seamless experience for users to track their workouts. The app features a clean and responsive design with interactive maps.

### Screenshot

![](./screenshot/Screenshot%201.png)
![](./screenshot/Screenshot%202.png)
![](./screenshot/Screenshot%203.png)

### Links

- Live Site URL: [Live](https://versatile28.github.io/Mapty/)

### Built with

- Semantic HTML5 markup
- CSS basic properties
- Flexbox
- JavaScript
- Leaflet.js for map integration
- Geolocation API
- Local Storage API

### Description

Mapty enables users to log their workouts and track their fitness journey effectively. The app focuses on user-friendly interaction and real-time geolocation integration. It's perfect for individuals looking to log activities like running and cycling while associating them with specific locations.

- Features:

- Interactive Map: Displays the user's current location using geolocation.
- Workout Logging: Log workout details like distance, duration, and type (running or cycling).
- Dynamic Marker Placement: Adds workout markers on the map for logged activities.
- Persistent Data: Saves workout data locally to maintain state across sessions.
- Error Handling: Displays error messages for invalid data or geolocation issues.
- Responsive Design: Works seamlessly across devices, including mobile and desktop.

### System Design

The Mapty app's workflow is divided into the following stages:

### Page Load:

- The app fetches the user's current location using the Geolocation API.
- If successful, it renders the map centered on the user's location using Leaflet.js.

### Workout Loading:

- Previously logged workouts are retrieved from the browser's Local Storage and displayed on the map and as a list.

### User Interaction:

- Users click on the map to open a form for logging a new workout.
- After submitting the form, the new workout is displayed on the map (as a marker) and in the workout list.
- The data is then stored in Local Storage.
- Users can click on a workout in the list to move the map to its location.

### Persistent State:

- All workouts are stored in the browser's Local Storage, ensuring data is preserved even after the app is closed or refreshed.

### Error Handling:

- If geolocation fails, an error message is displayed to the user.
- Validation ensures only valid input data is accepted for workout details.

### Useful resources

- [MDN Web Docs](https://developer.mozilla.org/en-US/) - Every HTML and CSS properties and their details are available here.It helped me to learn about different properties from here.
- [CSS Tricks](https://css-tricks.com/) - An excellent site for learning about CSS, including tips, tricks, and best practices.

## Author

- Website - [Satyaki Pal](https://www.linkedin.com/in/sp2812)
