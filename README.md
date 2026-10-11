# Weatherline

A live weather dashboard built with JavaScript, Tailwind CSS, Node.js, MySQL, and Open-Meteo.

Features: global city search, current conditions, a 7-day forecast, hourly temperature/rain SVG charts, sorting, Celsius/Fahrenheit, and MySQL-saved cities. The app also has dedicated Compare Cities, Weather Insights, and Settings screens. Compare two searched locations side by side; review UV, humidity, wind, rain chance, and weekly highs/lows; save unit, theme, and auto-location preferences in this browser. The Open-Meteo APIs used here do not require an API key. The browser asks for device location on open; if allowed, weather loads for those coordinates. Denying permission keeps the Mumbai fallback, and the My location button lets you retry. Geolocation requires localhost during development or HTTPS when opened from another device.

Requirements: Node.js 18+ and MySQL 8 (or compatible).

## Run
1. Run schema.sql in MySQL Workbench or your MySQL client.
2. Copy .env.example to .env and enter the MySQL connection details.
3. Run npm install, then npm start in this folder.
4. Open http://localhost:3000.

Weather data and location search use the Open-Meteo Geocoding and Forecast APIs. The dashboard displays provider attribution.
