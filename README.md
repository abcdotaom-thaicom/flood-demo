# Flood Inspection Map

A web-based application for visualizing and inspecting flood analysis data. This tool allows users to search for specific activity IDs, view inspection points on a map, and access detailed information including satellite imagery and model results.

## Features

- **Interactive Map**: Built with [Leaflet.js](https://leafletjs.com/), featuring Google Maps Hybrid tiles for clear satellite and road visibility.
- **Search Functionality**: Quickly find specific inspection points by entering an "Activity ID" on the landing page.
- **Detailed Inspection**: Click on map markers to view comprehensive details in a bottom sheet:
    - Activity ID and Confirmation Status
    - Model Result Text
    - Address and Planting/Harvesting Dates
    - Satellite Image Preview (with full-screen modal)
- **Navigation Integration**: Direct links to Google Maps for navigation and location search.
- **Responsive Design**: Optimized for both desktop and mobile devices.

## Technologies Used

- **HTML5 & CSS3**: Semantic structure and modern styling (using CSS Variables and Flexbox/Grid).
- **JavaScript (ES6+)**: Core logic for map interaction and data handling.
- **Leaflet.js**: Open-source JavaScript library for mobile-friendly interactive maps.
- **Google Maps Tiles**: Used as the base map layer (Hybrid view).

## Project Structure

- `index.html`: The landing page containing the search interface and a background map overview.
- `map.html`: The main map application where users can interact with inspection points.
- `output_png1/`: Directory containing the data file (`flood_analysis_data.json`) and associated images.
- `preview_...html`: An external HTML preview file linked from the main page.

## Getting Started

### Prerequisites

This is a static web application. You don't need a backend server to run it locally for basic testing, although using a local server is recommended to avoid CORS issues with fetching JSON data.

### Installation & Usage

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/attawutnp/website-demo.git
    cd website-demo
    ```

2.  **Run the application**:
    - **Option A (Recommended)**: Use a simple HTTP server (e.g., Python, VS Code Live Server).
        - Python 3: `python -m http.server`
        - Then open `http://localhost:8000` in your browser.
    - **Option B**: Open `index.html` directly in your browser (Note: This might block loading the JSON data due to browser security policies).

3.  **Explore**:
    - Enter an Activity ID in the search box or click "View Flood Preview".
    - Interact with markers on the map to see details.

## License

[MIT](LICENSE)
