# mapty-workout-tracker

A responsive geolocation-based web application to map, log, and analyze running and cycling workouts using the Leaflet interactive map library.

## Project Overview

`mapty-workout-tracker` utilizes the browser's Geolocation API along with the Leaflet open-source JavaScript library to allow athletes and fitness enthusiasts to log running and cycling activities directly onto an interactive map. Workouts are persisted in the browser's `localStorage` so sessions are preserved across visits.

## Features

- **Geolocation Mapping**: Automatically centers the interactive map on the user's current geographic coordinates.
- **Interactive Workout Logging**: Click anywhere on the map to log a new workout with custom parameters.
- **Activity Types**:
  - **Running**: Tracks distance, duration, cadence, and automatically calculates pace (min/km).
  - **Cycling**: Tracks distance, duration, elevation gain, and calculates speed (km/h).
- **Persistent Storage**: Saves all workout data locally in the browser (`localStorage`).
- **Interactive Workout List**: Clicking on any logged workout pans and smoothly animates the map directly to the corresponding GPS coordinates with an active popup.

## Prerequisites

- A modern web browser supporting the HTML5 Geolocation API and ES6+ JavaScript.
- An active internet connection for Leaflet map tiles (OpenStreetMap / CartoDB).

## Installation/Build

No compilation or build tooling is required.

1. Clone the repository:
   ```bash
   git clone https://github.com/AntonioHellin/Mapty_app.git
   cd Mapty_app
   ```

2. Serve locally using any static web server:
   ```bash
   npx serve .
   ```

## Usage

1. Open `index.html` in your web browser.
2. Grant permission when the browser requests access to your location.
3. Click anywhere on the map to open the workout entry form.
4. Select the activity type (Running or Cycling), enter the details, and press `Enter` to record the workout.
5. Click on any workout card in the sidebar to center the map on that workout.
