# Weather Dashboard

A responsive weather dashboard built with HTML, CSS, and vanilla JavaScript. It uses the Fetch API and `async/await` to retrieve city coordinates and current weather data from the public Open-Meteo APIs.

## Features

- Search for weather by city name.
- Displays temperature, humidity, wind speed, apparent temperature, and conditions.
- Parses nested JSON responses.
- Handles invalid city names, HTTP failures, and unexpected API responses.
- Responsive layout for phones and desktops.
- No API key required.

## Files

- `index.html` — page structure and dashboard elements.
- `style.css` — responsive visual styling.
- `script.js` — geocoding, weather requests, JSON parsing, rendering, and error handling.

## Run the project

1. Extract the ZIP file.
2. Open the `weather_dashboard_project` folder.
3. Open `index.html` in a modern browser with an internet connection.

If your browser blocks requests when opening a local file, run a simple local server from the project folder:

### Python

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

### Visual Studio Code

Install the **Live Server** extension, right-click `index.html`, and choose **Open with Live Server**.

## API endpoints used

- Geocoding: `https://geocoding-api.open-meteo.com/v1/search`
- Forecast/current conditions: `https://api.open-meteo.com/v1/forecast`

Open-Meteo's public API is used without an API key for this educational project. Please check its current terms and usage limits before deploying for production.

## Assignment concepts demonstrated

- `fetch()` for network requests
- `async` / `await`
- `try` / `catch` / `finally`
- HTTP status checking with `response.ok`
- JSON parsing with `response.json()`
- Reading nested JSON objects
- Dynamic DOM updates
- Search form handling and input validation
