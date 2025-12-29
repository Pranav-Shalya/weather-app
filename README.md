🌦️ Weather Forecast Web App

A modern weather forecasting web application that fetches real-time weather data based on the user’s current location and displays current, hourly, and daily forecasts using a clean and interactive UI.

📌 Project Overview

The Weather App uses the Open-Meteo API to retrieve accurate weather information such as temperature, wind speed, precipitation, and weather conditions. The application automatically detects the user’s location using the browser’s Geolocation API and dynamically updates the UI using JavaScript DOM manipulation.

This project demonstrates API integration, asynchronous JavaScript, modular code structure, and frontend build tooling using Vite.

🎯 Problem Statement

Users often need quick and accurate weather information without manually entering their location.

The goal of this project was to:

Automatically detect user location

Fetch real-time weather data

Display current, hourly, and daily forecasts

Present the data in a clean, user-friendly interface

🧠 What I Built

Current weather section (temperature, wind speed, precipitation)

Hourly weather forecast

Daily weather forecast

Weather icons mapped to weather codes

Error handling for location access and API failures

🛠️ Tech Stack & Tools

Technology	Usage

HTML	Structure of the web app

CSS	Styling and layout

JavaScript (ES6+)	Core logic, DOM manipulation

Axios	API requests

Vite	Development server & bundler

Open-Meteo API	Weather data source

Geolocation API	Fetch user’s location

📂 Project Structure

weather-app/
│
├── index.html
├── main.js
├── weather.js
├── iconMap.js
├── style.css
├── icons/
│   └── *.svg
├── package.json
└── README.md

🔄 How the App Works (Implementation Flow)

Location Access

The app requests the user’s geographical coordinates using navigator.geolocation.

API Request

Latitude, longitude, and timezone are passed to the Open-Meteo API using Axios.

Data Parsing

Raw JSON response is parsed into:

Current weather

Hourly forecast

Daily forecast

DOM Manipulation

Weather data is dynamically inserted into the UI using querySelector and data attributes.

Icon Mapping

Weather codes from the API are mapped to corresponding SVG icons.

Error Handling

Alerts are shown if location access fails or the API request errors out.

📊 Key Features

Automatic location detection

Real-time weather updates

Modular JavaScript architecture

Clean UI rendering with reusable templates

Lightweight and fast using Vite

⚠️ Challenges Faced & Solutions

1. JavaScript File Not Loading

Problem:
Main JavaScript file wasn’t executing.

Solution:
Used <script type="module" src="main.js"></script> in index.html.

2. API Data Not Displaying

Problem:
Raw API data structure was complex.

Solution:
Created separate parsing functions (parseCurrentWeather, parseHourlyWeather, parseDailyWeather) to clean and format data.

3. Icon Mapping Issues

Problem:
Weather codes didn’t directly match icons.

Solution:
Implemented a Map() structure to link weather codes to icon names.

4. CORS & Build Issues

Problem:
Browser restrictions when running locally.

Solution:
Used Vite dev server, which handles module loading and CORS smoothly.

📈 Business / Practical Impact

Provides instant weather insights with minimal user effort

Demonstrates real-world API usage

Easily extendable to mobile apps or backend integration

Can be enhanced with caching, favorites, and alerts

🚀 Future Enhancements

Search weather by city name

Save favorite locations

Add weather alerts

Dark mode UI

Backend proxy for API security

🧩 How This Project Relates to the Role

This project showcases my ability to:

Work with REST APIs

Handle asynchronous JavaScript

Build modular frontend applications

Debug real-world issues

Deliver user-focused solutions

It directly aligns with Frontend / Web / Software Engineering internship roles.

▶️ How to Run Locally
npm install
npm run dev
