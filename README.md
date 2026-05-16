Smart City Weather (HK)

Modern, mobile-first weather dashboard for Hong Kong and beyond.

A Hong Kong weather dashboard that provides real-time conditions, hourly forecasts, and 7-day trends. The frontend adopts a glassmorphism design with responsive layouts, while the backend (Node.js/Express) aggregates data from the Open-Meteo API with caching, rate-limiting, and secure middleware.

This project serves as a portfolio showcase of my full-stack development skills, combining clean UI, API integration, and deployment on Render.

✨ Features

User Features

Real-time conditions: temperature, feels-like, humidity, wind speed, weather code

24-hour forecast: temperature + precipitation (Chart.js mixed line/bar chart)

7-day forecast: min/max temperatures, precipitation, and weather icons

Input city names or raw coordinates (22.3,114.17)

Default view: Central, Hong Kong (configurable in .env)

Responsive UI with dark, glass-like design

System Features

REST API: /api/weather?lat=...&lon=...&timezone=...

Caching: Node-Cache to reduce API calls

Rate Limiting: prevent misuse with express-rate-limit

Security: helmet headers, CORS configuration

Logging: HTTP logs via morgan

🧑‍💻 My Contributions

Designed and implemented Express routes and weather API adapter

Transformed raw Open-Meteo JSON into frontend-friendly data structures

Built the frontend using HTML, CSS, and vanilla JS with responsive layouts and gradient design

Integrated Chart.js for interactive temperature/precipitation charts

Deployed on Render, configured environment variables for production

Focused on maintainability: modular JS, .env support, reusable components

🧰 Tech Stack

Frontend

HTML5, CSS3 (Glassmorphism, gradients, responsive design)

Vanilla JavaScript

Chart.js

Backend

Node.js + Express

Axios (fetching weather data)

Node-Cache

express-rate-limit, helmet, cors, morgan

dotenv

Deployment

Render (Web Service)

GitHub (source control)

🚀 Getting Started
Prerequisites

Node.js >= 18

Render (or any Node.js-capable hosting platform)

Environment Variables

Create a .env file in the project root:

PORT=3000
TIMEZONE=Asia/Hong_Kong
DEFAULT_LAT=22.302711
DEFAULT_LON=114.177216

Local Setup
# Clone the repository
git clone https://github.com/peilin-web/smart-city-dashboard.git
cd smart-city-dashboard

# Install dependencies
npm install

# Start the server
npm start

# Visit in browser
http://localhost:3000

🔌 API Endpoints

Health Check
GET /api/weather/test
Response: { "message": "Weather API is running ✅" }

Weather Data
GET /api/weather?lat=<number>&lon=<number>&timezone=<IANA TZ>

🖼️ UI Highlights

Glassmorphism cards with blur and transparency

Gradient backgrounds for a modern aesthetic

Interactive charts with tooltips and combined line/bar visualization

Mobile-first responsive design with adaptive fonts and layouts

☁️ Deployment on Render

Create a new Web Service and link this repo

Select Node as the language

Build Command: npm install

Start Command: npm start

Add environment variables from .env

Deploy to receive a public link

🗺️ Roadmap

Add city name geocoding for coordinates

User accounts with saved cities and search history

Unit switching (°C/°F, mm/in)

Progressive Web App (PWA) support

CI/CD pipeline with automated deployments

🙏 Acknowledgements

Weather data from Open-Meteo

Data visualization by Chart.js

📄 License

For portfolio and educational purposes only.


