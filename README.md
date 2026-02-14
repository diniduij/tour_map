# Trenton 3D Tour Map

A lightweight CesiumJS application displaying Google Photorealistic 3D tiles over Trenton, New Jersey. The app provides an interactive map with a simple layer toggle UI for viewing the 3D tileset.

## Features

- **Google 3D Photorealistic Tiles** – High-quality 3D terrain and buildings
- **Interactive Layer Toggle** – Show/hide the 3D tiles using a checkbox
- **Terrain Integration** – Cesium World Terrain for elevation data
- **Responsive Design** – Works on desktop browsers

## Requirements

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection (CDN resources)
- No local dependencies—everything runs in-browser

## Installation & Usage

### Running Locally

1. Navigate to the `tour_map` folder in your terminal.
2. Start a local HTTP server:

   **Python 3:**
   ```bash
   python -m http.server 8000
   ```

   **Python 2:**
   ```bash
   python -m SimpleHTTPServer 8000
   ```

   **Node.js (http-server):**
   ```bash
   npx http-server
   ```

3. Open your browser and visit: [http://localhost:8000/](http://localhost:8000/)

## API Keys & Configuration

The application uses two API tokens:

1. **Cesium Ion Token** – For terrain and resources (embedded in `index.html`)
2. **Google 3D Tiles API Key** – For Photorealistic 3D tiles (embedded in `index.html`)

To use your own tokens:
- Replace the `Cesium.Ion.defaultAccessToken` value in `index.html`
- Replace the Google API key in the Cesium3DTileset URL

## Technologies

- [CesiumJS](https://cesiumjs.org/) – 3D mapping library
- [Google 3D Tiles](https://developers.google.com/maps/documentation/javascript/3dtiles) – 3D geospatial data
- Vanilla JavaScript – No build tools required

## License

This project is open source. Ensure compliance with Cesium and Google's terms of service.

## Credits

- Trenton, NJ geographic data
- CesiumJS development team
- Google Maps 3D Tiles
