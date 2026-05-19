# 🚗 RevCarData API & Datasets

[![Website](https://img.shields.io/badge/Website-revcardata.com-blue?style=for-the-badge&logo=google-chrome)](https://revcardata.com)
[![API Docs](https://img.shields.io/badge/OpenAPI-Documentation-brightgreen?style=for-the-badge&logo=swagger)](https://api.revcardata.com/docs)
[![Database](https://img.shields.io/badge/Database-5200%2B_Vehicles-orange?style=for-the-badge&logo=database)](https://revcardata.com)

**RevCarData** is the ultimate technical specifications database for over **5,200+ car models** globally. Our mission is to provide developers, startups, and automotive projects with clean, structured, and instantly accessible data via a lightning-fast REST API.

Whether you're building an EV routing app, an insurance comparison tool, a B2B SaaS platform, or an auto-parts e-commerce store, our API will save you months of complex web scraping.

---

## 🌟 Key Features
* **Massive Database:** 5,200+ unique vehicles, covering both Internal Combustion Engine (ICE) cars and the latest Electric Vehicles (EV).
* **Developer First:** Clean, fast, and highly predictable JSON responses.
* **Standardized:** Data is structured around the industry standard **YMME** (Year, Make, Model, Engine) format.
* **Premium Quality:** Constantly cleaned and verified for commercial production use.

---

## 🚀 Quick Start (Code Snippets)

To use the API, you simply need to pass your `X-API-Key` in the request headers. Get your API key at **[revcardata.com](https://revcardata.com)**.

### Python (Requests)
```python
import requests

url = "[https://api.revcardata.com/api/v1/vehicles](https://api.revcardata.com/api/v1/vehicles)"
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

fetch('[https://api.revcardata.com/api/v1/vehicles](https://api.revcardata.com/api/v1/vehicles)', options)
  .then(response => response.json())
  .then(response => console.log(response))
  .catch(err => console.error(err));
```

### cURL
```bash
curl -X GET "[https://api.revcardata.com/api/v1/vehicles](https://api.revcardata.com/api/v1/vehicles)" \
     -H "X-API-Key: YOUR_API_KEY"
```

---

## 🛣️ Endpoints Overview
Our infrastructure offers a modular approach to fetching automotive data. The basic flow:
1. **`/makes`** - Retrieve a list of all supported vehicle makes.
2. **`/models`** - Filter models by specific make and year.
3. **`/vehicles/{id}/premium`** - Fetch in-depth technical specs (EV ranges, battery capacity, horsepower, torque, dimensions, etc.).

> 👉 **[Test all endpoints in our interactive OpenAPI browser](https://api.revcardata.com/docs)**

---

## 💎 Pricing & Raw Datasets
We believe in fair pricing for both solo developers and enterprise teams. 

**Need the raw data?** If you don't want to use an API and prefer to download the entire physical database for machine learning, offline usage, or internal B2B systems, we sell complete, one-time CSV/JSON dataset exports.

Check out our website for SaaS checkout, API plans, and raw dataset downloads: **[revcardata.com](https://revcardata.com)**.

---

## 🛠️ Support & Contact
Are you missing a specific brand? Do you need a custom data solution, or have you encountered a technical issue? We are developers ourselves and we're here to help.

* **Website:** [revcardata.com](https://revcardata.com)
* **API Portal:** [api.revcardata.com/docs](https://api.revcardata.com/docs)
