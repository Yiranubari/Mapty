# Mapty: Map Your Workouts

## Overview

**Mapty** is a simple, modern web application designed to help users track and visualize their running and cycling workouts directly on a map. By leveraging the user's geolocation and the powerful **Leaflet.js** library, Mapty allows you to log your activities, calculate key metrics like pace and speed, and see your fitness journey unfold geographically.

This project is a pure JavaScript application, focusing on object-oriented programming principles to manage workout data and application state.

## Features

*   **Geolocation:** Automatically detects and centers the map on the user's current location.
*   **Interactive Map:** Uses Leaflet.js to display an interactive map where users can click to log a new workout.
*   **Workout Logging:** Supports two distinct workout types:
    *   **Running:** Requires distance, duration, and cadence (steps per minute). Calculates **pace** (min/km).
    *   **Cycling:** Requires distance, duration, and elevation gain. Calculates **speed** (km/h).
*   **Data Persistence:** All logged workouts are stored locally in the browser's **Local Storage**, ensuring data is saved even after closing the application.
*   **Workout Visualization:** Workouts are displayed as markers on the map and listed in a sidebar with detailed information.
*   **Map Navigation:** Clicking a workout in the sidebar automatically moves the map view to the corresponding location.

## Technologies Used

| Category | Technology | Purpose |
| :--- | :--- | :--- |
| **Core** | HTML5, CSS3, JavaScript (ES6+) | Frontend structure, styling, and application logic. |
| **Mapping** | Leaflet.js | Open-source JavaScript library for interactive maps. |
| **Data** | Browser Local Storage | Persistent storage for workout data. |
| **APIs** | Geolocation API | To get the user's current geographical coordinates. |

## Getting Started

Mapty is a client-side application and does not require any backend setup or build process.

### Prerequisites

You only need a modern web browser (Chrome, Firefox, Edge, Safari) that supports the Geolocation API.

### Installation and Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Yiranubari/Mapty.git
    cd Mapty
    ```

2.  **Open the application:**
    Simply open the `index.html` file in your web browser.
    ```bash
    # Example command (may vary by OS)
    open index.html
    ```

3.  **Grant Location Access:**
    The browser will prompt you to allow access to your location. You **must** grant permission for the map to load correctly and for the application to function.

## Usage

1.  **Locate Yourself:** The map will automatically center on your current location.
2.  **Log a Workout:** Click anywhere on the map where you completed your workout.
3.  **Enter Details:** A form will appear in the sidebar. Select the workout type (Running or Cycling) and enter the required metrics (distance, duration, cadence/elevation gain).
4.  **Save:** Click the "OK" button to save the workout. It will appear as a marker on the map and a new entry in the sidebar.
5.  **View Details:** Click on a workout entry in the sidebar to instantly pan the map to that location.

## Project Structure

```
Mapty/
├── index.html          # Main application structure
├── style.css           # Application styling
├── script.js           # Core application logic (OOP, data handling, Leaflet integration)
├── icon.png            # Application favicon
├── logo.png            # Application logo
├── Mapty-flowchart.png # Project planning diagram
└── README.md           # This file
```

## Contributing

If you have suggestions for improvements or find a bug, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the repository for details.
