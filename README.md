# 🏰 PuneGo — Pune Travel Companion & Smart Mobility Platform

A web travel companion application built for **Pune, Maharashtra**, fulfilling all functional and non-functional requirements specified in the **Pune Travel App ("PuneGo") PRD Version 1.0**.

---

## 🌟 Key Features & Modules

### 1. 🧭 Discover Hub (`src/components/discover/`)
- **6 Curated Categories**: Heritage & Forts, Nature & Lakes, Food & Cafes, Shopping & Hubs, Nightlife & Lounges, and Offbeat & Culture.
- **Rich Landmark Metadata**: Shaniwar Wada, Sinhagad Fort, Aga Khan Palace, Dagdusheth Halwai Ganpati, Cafe Vaishali / FC Road, Panshet Dam, Balewadi High Street, Phoenix Marketcity, Raja Dinkar Kelkar Museum, Vetal Tekdi, Katakirrr Misal, Khadakwasla Dam, and more.
- **Filters**: Free entry toggle, Zone selector (Central Pune, Koregaon Park, Kothrud, Hinjewadi, Outskirts), time duration, and sort by rating/time/tariff.
- **Audio Guides**: Real-time Marathi pronunciation for every spot using HTML5 Web Speech API.
- **Dynamic Climate Alerts**: Live monsoon trekking advisories for Sahyadri forts.

### 2. 🗺️ Interactive City Map (`src/components/map/`)
- Built with **Leaflet** and OpenStreetMap tiles.
- Custom colored marker pins per category + Pune Metro station pins.
- **Itinerary Route Path**: Dynamic dashed connector line visualizes consecutive stop routes for any day.
- Interactive popups with thumbnails, price badges, and one-click "+ Add to Trip" or "View Details".

### 3. 📅 Smart Itinerary Planner (`src/components/itinerary/`)
- **Multi-Day Planning**: Create, edit, rename, and organize multi-day trips (Day 1, Day 2, Day 3+).
- **Auto Travel Time & Fare**: Automatically computes travel distance (km) and estimated transit time / auto meter fare between consecutive stops.
- **Daily Budget Estimator**: Computes entrance ticket totals + estimated transit costs + food/misal allowance.
- **AI Itinerary Generator**: One-click prompt presets (Classic Heritage, Monsoon Trekkers, Executive Business) and free-text AI generation.
- **Print / PDF Export & WhatsApp Sharing**: Clean print preview with scannable QR verification and pre-formatted WhatsApp trip itineraries.

### 4. 🚇 Multi-Modal Transport Hub (`src/components/transport/`)
- **Pune Metro Route Planner (Maha Metro)**: Purple Line (Line 1: PCMC to Swargate) and Aqua Line (Line 2: Vanaz to Ramwadi) with Civil Court Interchange guidance, station facilities, fare matrix (₹10–₹35), and travel times.
- **Auto & Cab Comparator**: Pune RTO calibrated meter formula (Base ₹25 first 1.5km + ₹17/km) vs Ola Auto, UberGo, and Rapido bike taxi with direct app deep-links.
- **PMPML City Buses**: Search bus routes (e.g. Route 100 to Hinjewadi, Route 174 to Sinhagad, Route 148 to Airport) with timings and frequencies.

### 5. 🎫 Travel Passes & Digital QR Ticketing (`src/components/bookings/`)
- **PRD Section 14 Plans**:
  - *Solo Explorer* (1 Person — ₹799)
  - *Duo Plan* (2 People — ₹1,449)
  - *Family / Small Group* (3–5 People — ₹2,999)
  - *Large Group* (6–10 People — ₹5,499)
  - *Custom / Corporate* (10+ People)
- **Active Promo Codes**: `EARLYBIRD15` (15% off), `WEEKDAY20` (20% off), `STUDENT10` (10% off), `GROUP10` (10% off), `FESTIVAL2026` (₹500 off).
- **Experience Add-ons**: Guided Old Pune Heritage Walk, Sinhagad Nature Trek, and Puneri Food Tasting Trail.
- **Scannable QR Digital Pass**: Instant QR code generation with offline caching and printable ticket layout.

### 6. 🗣️ Local Guide, Marathi Phrasebook & SOS (`src/components/local/`)
- **Interactive Marathi Phrasebook**: 12+ conversational phrases categorized by Greetings, Auto/Transport, Food Ordering, Shopping, and Directions with Web Speech audio pronunciation.
- **Pune Festivals Calendar**: Ganeshotsav (5 Manache Ganpati & Dhol Tasha), Sawai Gandharva classical festival, and Palkhi Sohala with live traffic impact alerts.
- **Safety & Emergency Hub**: One-tap phone dialers for Pune Police (112), Women Helpline (1091), Sassoon Trauma, Ruby Hall Clinic, and MTDC Tourist assistance.

### 7. 🌐 Tri-Lingual Localization & Offline Support
- Instant language toggle: **English**, **मराठी (Marathi)**, and **हिंदी (Hindi)**.
- Multi-currency conversion: **₹ INR**, **$ USD**, and **€ EUR**.
- Persistent local storage for favorites, custom multi-day itineraries, and booked passes.

---

## 🛠️ Tech Stack

- **Framework**: React 19 + TypeScript + Vite 8
- **Styling**: Tailwind CSS v4 + Plus Jakarta Sans & Outfit fonts
- **Maps**: Leaflet
- **Icons**: Lucide React
- **Digital Passes**: QRCode & Canvas Confetti

---

## 🚀 Getting Started

### Development
```bash
npm install
npm run dev
```

### Production Build
```bash
npm run build
npm run preview
```

