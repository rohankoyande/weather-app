# Weather App

## Overview

This Weather App allows users to check the current weather and forecast for different cities. The app provides options to choose between predefined cities or enter a custom city name. Users can also select the temperature unit (Celsius or Fahrenheit) and customize the background color.

### Features:
- **Weather Information**: Displays current weather conditions, including temperature, weather description, humidity, and wind speed.
- **5-Day Forecast**: Shows the weather forecast for the next 5 days, including temperature and weather description for each day.
- **User Customization**: Users can select the default city, temperature unit, and background color. These preferences are saved using `localStorage`, ensuring settings persist between sessions.
- **Settings Page**: Allows users to change their default city, temperature unit, and background color preferences.

## Files

### `index.html` - Main Weather App Page
This is the main page where the user can check the current weather and forecast, enter a city, and adjust the temperature unit and background color settings.

### `settings.html` - Settings Page
This page allows users to change the settings (city, temperature unit, background color). The settings are stored in `localStorage`, so they persist across sessions.

## Installation

To use this app:
1. Clone or download the repository to your local machine.
2. Open the `index.html` file in a web browser to use the app.


## Technologies Used
- **HTML**: For the structure of the app.
- **CSS**: For styling the app and making it responsive.
- **JavaScript**: For handling user interactions, fetching weather data from the OpenWeatherMap API, and storing preferences in `localStorage`.
- **OpenWeatherMap API**: Used for fetching real-time weather data and forecasts.

## How It Works

### 1. **Main Weather Page (`index.html`)**:
- Users can choose a city from a predefined list or type a city name manually.
- Users can select the temperature unit (Celsius or Fahrenheit) and change the background color.
- Upon selecting a city, the app fetches weather data from OpenWeatherMap using the provided API key and displays:
  - **Current Weather**: Temperature, weather description, humidity, wind speed.
  - **5-Day Forecast**: The temperature and weather conditions for the next 5 days.

### 2. **Settings Page (`settings.html`)**:
- Users can change the default city, temperature unit, and background color.
- The settings are saved in `localStorage` so they persist across sessions.

### 3. **API Integration**:
- The app uses the OpenWeatherMap API to fetch the current weather and forecast data. The `apiKey` variable in the script should be replaced with your own API key.
- The weather data is displayed dynamically based on the user's preferences.

## Example Use Cases
- **User wants to check the weather**: They can select a city from the dropdown or type in their own city. The current weather and 5-day forecast will be displayed.
- **User wants to customize settings**: They can go to the Settings page, change the city, temperature unit, and background color to their preference.

## Local Storage
Settings like the chosen city, temperature unit, and background color are stored in the browser's `localStorage`. This ensures the preferences are retained across page reloads and browser sessions.

## Customization Options
- **Temperature Unit**: Choose between Celsius (°C) and Fahrenheit (°F).
- **Background Color**: Choose from Light Blue, Light Green, or Yellow.
- **City**: Select from predefined cities or enter any other city.

## How to Use
1. Open the `index.html` file in your browser.
2. Select a city from the dropdown or type a custom city in the text input.
3. Select a temperature unit (Celsius or Fahrenheit).
4. Click the "Get Weather" button to fetch and display weather data.
5. Go to the Settings Page to change the default city, temperature unit, and background color.
6. The app will save your settings, so the next time you visit, your preferences will be retained.

## API Key
The app uses the OpenWeatherMap API to get weather data. You will need to replace the API key in the script section of the `index.html` file:

```js
const apiKey = "YOUR_API_KEY"; // Replace with your OpenWeatherMap API key


You can sign up for a free API key on the OpenWeatherMap website.
