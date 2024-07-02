# GPS Sales Tracker

A simple web application that tracks your GPS location and allows you to record sales at specific points. The application will notify you of previous sales when you revisit a location.

## Features

- Tracks GPS location using the Google Maps API.
- Allows users to record sales at specific locations.
- Notifies users of previous sales when they revisit a location.
- Uses `google.maps.marker.AdvancedMarkerElement` for markers.

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, etc.)
- A Google Cloud Platform account with the Google Maps JavaScript API enabled.

### Setting Up Google Maps API

1. Go to the [Google Cloud Console](https://console.cloud.google.com/).
2. Create a new project or select an existing project.
3. Navigate to the [Google Maps JavaScript API page](https://console.cloud.google.com/apis/library/maps-backend.googleapis.com).
4. Enable the API for your project.
5. Go to the [Credentials page](https://console.cloud.google.com/apis/credentials) and create an API key.
6. Restrict the API key to your domain for security.

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/gps-sales-tracker.git
    cd gps-sales-tracker
    ```

2. Open `index.html` in a text editor and replace `YOUR_API_KEY` with your actual Google Maps API key:
    ```html
    <script async defer src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap"></script>
    ```

3. Open `index.html` in your web browser.

### Usage

1. Allow location access when prompted by your browser.
2. The map will center on your current location.
3. Enter the sale amount in the input field and click "Record Sale" to save the sale at your current location.
4. The application will log sales and notify you of previous sales when you revisit a location.

### Project Structure

- `index.html`: The main HTML file that includes the map and the sale tracking functionality.
- `style.css`: Basic styling for the application.
- `script.js`: JavaScript code that handles the map and sales logic.

### Advanced Marker Element

The application uses `google.maps.marker.AdvancedMarkerElement` for markers. For more information on how to use this, refer to the [migration guide](https://developers.google.com/maps/documentation/javascript/advanced-markers/migration).

### Troubleshooting

- If the map does not load, check the browser console for errors.
- Ensure that the Google Maps JavaScript API is enabled in your Google Cloud Console.
- Verify that the API key is correctly added to `index.html`.
- Make sure your browser has permission to access your location.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Google Maps JavaScript API](https://developers.google.com/maps/documentation/javascript/overview)

