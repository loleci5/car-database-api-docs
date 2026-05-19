🚗 RevCarData API Documentation
Welcome to the RevCarData API!
RevCarData is the ultimate technical specifications database for over 5,200+ car models globally. Our mission is to provide developers, startups, and automotive projects with clean, structured, and instantly accessible data via a lightning-fast REST API.
Whether you're building an EV routing app, an insurance comparison tool, a B2B SaaS platform, or an auto-parts e-commerce store, our API will save you months of complex web scraping.
🌟 Key Features
Massive Database: 5,200+ unique vehicles, covering both Internal Combustion Engine (ICE) cars and the latest Electric Vehicles (EV).
Developer First: Clean, fast, and highly predictable JSON responses.
Standardized: Data is structured around the industry standard YMME (Year, Make, Model, Engine) format.
Premium Quality: Constantly cleaned and verified for commercial production use.
🔑 Getting Started (Authentication)
Because we provide our API through the RapidAPI infrastructure, authentication is completely painless. Simply include your unique RapidAPI key with every request to our endpoints.
Required HTTP Headers:

HTTP


X-RapidAPI-Key: YOUR_UNIQUE_RAPIDAPI_KEY
X-RapidAPI-Host: revcardata.p.rapidapi.com


(You will receive this key automatically once you subscribe to one of our plans in the Pricing tab).
🛣️ Endpoints Overview
Our infrastructure offers a modular approach to fetching automotive data. (Check the Endpoints tab for exact parameters and to test requests directly in your browser). The basic flow:
/makes - Retrieve a list of all supported vehicle makes.
/models - Filter models by specific make and year.
/vehicles/{id} - Fetch in-depth technical specs (EV ranges, battery capacity, horsepower, torque, dimensions, etc.).
💎 Pricing & B2B Solutions
We believe in fair pricing for both solo developers and enterprise teams. Our API offers subscription tiers that scale with your usage on RapidAPI.
Need the raw data? If you don't want to use an API and prefer to download the entire physical database for machine learning, offline usage, or internal B2B systems, we sell complete, one-time CSV/JSON dataset exports.
Check out our website for SaaS checkout and raw dataset downloads: revcardata.com.
🛠️ Support
Are you missing a specific brand? Do you need a custom data solution, or have you encountered a technical issue? We are developers ourselves and we're here to help.
Official Website: revcardata.com
OpenAPI Documentation: api.revcardata.com/docs
