# Hotels API — Free Hotel Data API for Developers

Access **1M+ hotels worldwide** with GPS coordinates, ratings and amenities.  
Fast, reliable **REST API** designed for developers.  
**Free plan available**, no credit card required.

🌍 200+ countries  
⚡ <100ms average response time  
🧰 Amenities & advanced filters  
🔑 Simple API key authentication  

Website: https://hotels-api.com

---

## What is Hotels API?

Hotels API provides **clean, structured and up-to-date hotel data** for developers building travel apps, hotel search engines, maps, or internal tools.

This is a **data API**, not a booking engine.  
No reservations, no commissions — just hotel information.

---

## Features

- 🏨 **1,000,000+ hotels**
- 🌍 Coverage in **200+ countries**
- 📍 GPS coordinates (latitude & longitude)
- ⭐ Hotel ratings
- 🧰 Amenities per hotel (wifi, parking, pets, shuttle, pool, spa, etc.)
- 🔎 Advanced search & filters
- ⚡ Fast responses (<100ms)
- 📦 Clean JSON responses
- 🔐 API key authentication

---

## Use Cases

- Travel & accommodation websites  
- Hotel search engines  
- Map & geo-location apps  
- Travel comparison platforms  
- Data enrichment & internal tools  
- MVPs & prototypes  

---

## Authentication

All requests require an API key sent via header:

X-API-KEY: YOUR_API_KEY

Get a free API key:  
https://hotels-api.com/register

---

## Search Hotels by City & Amenities

Request:

GET /api/hotels/search?city=Barcelona&country=Spain&amenities=wifi,parking&limit=2  
Host: hotels-api.com  
X-API-KEY: YOUR_API_KEY

---

## Example Response

{
  "hotels": [
    {
      "id": 12345,
      "name": "Hotel Barcelona Center",
      "city": "Barcelona",
      "country": "Spain",
      "countryCode": "ES",
      "address": "Carrer de Balmes, 123, 08007",
      "rating": 4,
      "latitude": 41.3851,
      "longitude": 2.1734,
      "amenities": ["wifi", "parking", "restaurant", "bar"]
    }
  ]
}

---

## Search Hotels by Coordinates (Geo Search)

GET /api/hotels/nearby?lat=41.3851&lng=2.1734&radius=2000&limit=5  
Host: hotels-api.com  
X-API-KEY: YOUR_API_KEY

---

## Available Filters

| Parameter    | Description |
|-------------|------------|
| city        | City name |
| country     | Country name |
| countryCode | ISO country code |
| min_rating  | Minimum hotel rating |
| amenities   | Comma-separated amenities |
| lat         | Latitude |
| lng         | Longitude |
| radius      | Search radius (meters) |
| limit       | Number of results |

---

## Pricing

| Plan | Requests / Month | Price |
|------|------------------|-------|
| Free | 500 | $0 |
| Pro  | 250,000 | $39/month |
