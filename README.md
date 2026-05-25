# 🚗 RevCarData API & Datasets

[![Website](https://img.shields.io/badge/Website-revcardata.com-blue?style=for-the-badge&logo=google-chrome)](https://revcardata.com)
[![API Docs](https://img.shields.io/badge/OpenAPI-Documentation-brightgreen?style=for-the-badge&logo=swagger)](https://api.revcardata.com/docs)
[![Database](https://img.shields.io/badge/Database-86k%2B_Vehicles-orange?style=for-the-badge&logo=database)](https://revcardata.com)
[![Free Tier](https://img.shields.io/badge/Free_Tier-100_Req%2Fmo-success?style=for-the-badge)](https://revcardata.com/my-account)

**RevCarData** is the ultimate technical specifications database for over **86,835+ car models** globally. Our mission is to provide developers, startups, and automotive projects with clean, structured, and instantly accessible data via a lightning-fast REST API.

Whether you're building an EV routing app, an insurance comparison tool, a B2B SaaS platform, or an auto-parts e-commerce store, our API will save you months of complex web scraping and data cleaning.

---

## 🌟 Key Features
* **Massive Database:** 86,835+ unique vehicles, covering both Internal Combustion Engine (ICE) cars and the latest Electric Vehicles (EV).
* **Deep Specifications:** Includes MSRP pricing, precise dimensions, battery capacity (kWh), real-world EV ranges, horsepower, and torque.
* **Built for Speed:** Powered by FastAPI and Supabase, delivering highly predictable **<10ms latency** on standard queries.
* **Developer First:** Deeply nested JSON structures, industry-standard YMME format, and intelligent HATEOAS pagination out of the box.
* **Dropdown Helpers:** Ready-to-use endpoints to instantly populate your UI selectors (Years, Makes, Models, Trims, Body Types).

---

## 🆓 Free Developer Tier
We offer a **Free Test Tier (100 requests/month)** so you can evaluate the data structure and endpoints before upgrading. 
👉 **No credit card required.** Simply create an account at [revcardata.com](https://revcardata.com) and generate your Free Key in the API Dashboard.

---

## 🚀 Quick Start

To use the API, pass your `X-API-Key` in the request headers. 

### Python (Requests)
```python
import requests

url = "[https://api.revcardata.com/api/v1/vehicles?make=Toyota&year=2024](https://api.revcardata.com/api/v1/vehicles?make=Toyota&year=2024)"
headers = {
    "X-API-Key": "YOUR_API_KEY"
}

response = requests.get(url, headers=headers)
print(response.json())
```

### JavaScript (Fetch)
```javascript
const options = {
  method: 'GET',
  headers: {
    'X-API-Key': 'YOUR_API_KEY'
  }
};

fetch('[https://api.revcardata.com/api/v1/vehicles?make=Toyota&year=2024](https://api.revcardata.com/api/v1/vehicles?make=Toyota&year=2024)', options)
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(err => console.error(err));
```

### cURL
```bash
curl -X GET "[https://api.revcardata.com/api/v1/vehicles?make=Toyota&year=2024](https://api.revcardata.com/api/v1/vehicles?make=Toyota&year=2024)" \
     -H "X-API-Key: YOUR_API_KEY"
```

---

## 🛣️ Endpoints Overview
Our infrastructure offers a modular approach to fetching automotive data:

1. **`GET /api/v1/vehicles`** - Deep search functionality (filter by make, model, year, body style, fuel type, min HP, EV range, etc.).
2. **`GET /api/v1/vehicles/{id}/core`** - Retrieve fundamental specs (Engine type, displacement, transmission, drivetrain).
3. **`GET /api/v1/vehicles/{id}/premium`** - Fetch in-depth technical specs (Pricing, exact dimensions, EV battery metrics, acceleration).
4. **`GET /api/v1/makes` (and other helpers)** - Instantly retrieve unique lists for your frontend dropdowns (Makes, Models, Trims, Transmissions, Fuel Types).

> 👉 **[Test all endpoints in our interactive OpenAPI browser](https://api.revcardata.com/docs)**

---

## 💎 Pricing & Raw Datasets
We believe in fair pricing for both solo developers and enterprise teams. 

**Need the raw data?** If you don't want to use an API and prefer to download the entire physical database for machine learning, offline usage, or internal B2B systems, we sell complete, one-time CSV/JSON dataset exports.

Check out our website for SaaS checkout, API plans, and raw dataset downloads: **[revcardata.com/pricing](https://revcardata.com/pricing)**.

---

## 🛠️ Support & Contact
Are you missing a specific brand? Do you need a custom data solution, or have you encountered a technical issue? We are developers ourselves and we're here to help.

* **Website:** [revcardata.com](https://revcardata.com)
* **API Portal:** [api.revcardata.com/docs](https://api.revcardata.com/docs)
