# 🍱 Surplus Food Portal

> **Connecting Surplus Food Donors with Local NGOs in Real-Time.**

An end-to-end web platform built to minimize food waste and eliminate hunger. Surplus Food Portal enables restaurants, hotels, events, and individuals to list excess edible food, which is instantly mapped and broadcast to verified NGOs for quick pickup and safe redistribution.

---

## 🚀 Key Features

* **Real-Time Dynamic Matching:** Integrated with WebSockets (`Socket.IO`) to instantly broadcast new food listings to active NGOs without refreshing.
* **Interactive Geo-Location Mapping:** Built with `React-Leaflet` and `OpenStreetMap (Nominatim API)` for precision pinpoints, reverse geocoding, and draggable location markers.
* **Role-Based Workflows:** Distinct dashboard views and features custom-tailored for **Donors** (Restaurants, Households, Events), **NGOs**, and **Admins**.
* **One-Click Claiming:** Streamlined claim pipeline allowing NGOs to quickly reserve food posts and coordinate pickup routes.
* **Dynamic Search & Filtering:** Filter active food listings by location text match, donor, or real-time map distance.

---

## 🛠️ Tech Stack

### **Frontend**
* **Framework:** React.js
* **Styling:** Tailwind CSS
* **Mapping:** Leaflet.js, React-Leaflet
* **HTTP & Real-Time:** Axios, Socket.IO Client

### **Backend**
* **Runtime:** Node.js, Express.js
* **Real-Time Server:** Socket.IO
* **Geocoding:** OpenStreetMap (Nominatim API)
* **Database:** MongoDB (Geospatial Queries & Indexing)

---

## 📂 Repository Structure

```text
surplus-food-portal/
├── client/                 # React Frontend Application
│   ├── public/
│   └── src/
│       ├── assets/         # Dynamic assets & logos
│       ├── App.js          # Main Application Component & Socket Listeners
│       └── index.js
│
├── server/                 # Node.js / Express Backend Engine
│   ├── models/             # Database Schemas (Food, User)
│   ├── routes/             # REST API Routes (Auth, Food CRUD, Claim)
│   ├── server.js           # Express App & Socket.IO Initialization
│   └── .env
│
└── README.md
