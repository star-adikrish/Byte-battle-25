
Given the weather api url "WEATHER_URL" and api key "API_KEY"
WEATHER_URL = "http://api.weatherapi.com/v1"
API_KEY = "API_KEY"

Scenario:

When the user selects a CityName and aqi check-box
then fetch the weather and aqi details from the weather api end-point "/current.json" using a GET HTTP call. Provide query params key=API_KEY&q=CityName&aqi=yes

This will return a JSON like
"""
{
    "location": {
        "name": "Bangalore",
        "region": "Karnataka",
        "country": "India",
        "lat": 12.9833,
        "lon": 77.5833,
        "tz_id": "Asia/Kolkata",
        "localtime_epoch": 1764931171,
        "localtime": "2025-12-05 16:09"
    },
    "current": {
        "last_updated_epoch": 1764930600,
        "last_updated": "2025-12-05 16:00",
        "temp_c": 25.3,
        "temp_f": 77.5,
        "is_day": 1,
        "condition": {
            "text": "Partly cloudy",
            "icon": "//cdn.weatherapi.com/weather/64x64/day/116.png",
            "code": 1003
        },
        "wind_mph": 12.1,
        "wind_kph": 19.4,
        "wind_degree": 69,
        "wind_dir": "ENE",
        "pressure_mb": 1017.0,
        "pressure_in": 30.03,
        "precip_mm": 0.03,
        "precip_in": 0.0,
        "humidity": 69,
        "cloud": 75,
        "feelslike_c": 26.8,
        "feelslike_f": 80.3,
        "windchill_c": 23.6,
        "windchill_f": 74.5,
        "heatindex_c": 25.4,
        "heatindex_f": 77.6,
        "dewpoint_c": 17.3,
        "dewpoint_f": 63.1,
        "vis_km": 6.0,
        "vis_miles": 3.0,
        "uv": 0.7,
        "gust_mph": 16.6,
        "gust_kph": 26.6,
        "air_quality": {
            "co": 336.85,
            "no2": 4.55,
            "o3": 99.0,
            "so2": 4.05,
            "pm2_5": 13.35,
            "pm10": 13.65,
            "us-epa-index": 1,
            "gb-defra-index": 2
        }
    }
}
"""