# Weather & Air Quality Checker 🌤️

A modern web application that provides real-time weather and air quality information for any city or airport code worldwide.

## Features ✨

- **Global Coverage**: Get weather data for any city name or airport code worldwide
- **Real-time Weather**: Current temperature, humidity, wind speed, pressure, and visibility
- **Air Quality Index**: Comprehensive AQI data including PM2.5, PM10, CO, NO2, O3, SO2
- **Search History**: Track your recent weather searches
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Multi-page Interface**: Home, About, Contact, and Blog sections

## Usage 🚀

1. Enter any city name (e.g., "Mumbai", "New York") or airport code (e.g., "LAX", "DEL")
2. Check the "Include Air Quality" option to get AQI data
3. Click "Get Weather Data" or press Enter
4. View detailed weather and air quality information

## API Integration 🔌

The application uses the WeatherAPI service:

- **Base URL**: `https://api.weatherapi.com/v1`
- **Endpoint**: `/current.json`
- **Parameters**: `key`, `q` (city/airport), `aqi` (yes/no)

## Project Structure 📁

```
├── index.html          # Main HTML file
├── styles.css          # Styling
├── weather.js          # Weather application logic
├── config.js           # API configuration
├── .github/workflows/  # GitHub Actions deployment
└── README.md           # This file
```

## Deployment 🚀

### GitHub Secrets Setup

1. Go to your GitHub repository
2. Navigate to **Settings** > **Secrets and variables** > **Actions**
3. Add a new repository secret:
   - **Name**: `API_KEY`
   - **Value**: Your WeatherAPI key

### Local Development

For local development, replace `your-api-key-here` in `config.js` with your actual WeatherAPI key.

## Technologies Used 💻

- HTML5
- CSS3
- Vanilla JavaScript
- WeatherAPI
- GitHub Actions
- GitHub Pages

## Team 👥

**Super 4 Team** - NPS East
- Krishna Agrawal - Lead Developer
- Sri Krishna & Darsh Goyal - Hardware Development
- Tanay Acharya - Visual Communications

---

*© 2025 NPS East. All rights reserved. | Powered by Super 4*