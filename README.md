# ✈️ Travel System

A high-fidelity, single-file travel planner PWA designed as a **live operational dashboard** for a multi-city European trip.

Built with zero dependencies, focused on performance, clarity, and real-time context.

---

## 🧠 Philosophy


 **data-driven system** that integrates:

- time
- location
- finance
- schedule
- real-world signals

The goal is to behave like a **living interface**

---

## ⚙️ Tech Stack

- HTML (single file)
- CSS (custom design system + glass UI)
- Vanilla JavaScript
- PWA (offline-capable)
- External APIs:
  - Weather
  - Currency (EUR → BRL)
  - Flight data
  - Events (Bandsintown)
  - Places (Google Places)

No frameworks. No build tools.

---

## 🧱 Architecture
index.html
├── UI (HTML)
├── Design System (CSS variables + tokens)
└── Logic (JS)
├── Store (central state)
├── Services (APIs)
├── Computed (derived data)
└── Render (UI updates)

### Data Flow

API → normalize → Store → computed → UI

Single source of truth: `Store`

---

## 🧩 Core Features

### 🏠 Home (Reactive Dashboard)

- Real-time clock (multi-timezone)
- Weather per active city
- Financial summary (BRL)
- Work window
- Live system feel (animations)

---

### 📅 Agenda

- Continuous timeline
- City-based color system
- Automatic day type:
  - Weekdays → work
  - Weekends → free
- Scroll-reactive UI
- Minimal visual noise

---

### 💰 Grana (Finance System)

- BRL-first dashboard
- Flight + hotel + expense aggregation
- MCP email parsing (Booking.com)
- Cost per day
- Animated totals
- Internal flights only (excludes Brazil flights)

---

### 🌆 Cena (Discovery Engine)

- Real-time events (Bandsintown)
- Local venues (Google Places)
- Vibe-based ranking system
- Schedule-aware suggestions

---

## 🎨 Design System

- True dark mode
- Glassmorphism (controlled usage)
- City-based color tokens
- Depth via opacity and blur
- Motion-first UI

---

## ⚡ Motion & Interaction

- Blinking clock colon (real-time feel)
- Timeline energy flow
- Animated financial values
- Staggered content reveal
- Scroll-based activation

---

## 📱 iOS App (No Developer Account)

The app can be wrapped into a native iOS container using `WKWebView`.

### Steps:

1. Open Xcode
2. Create iOS App (SwiftUI)
3. Embed WebView pointing to deployed URL
4. Run on device

---

### ⚠️ Limitations (Free Apple ID)

- App expires every 7 days
- Must reinstall or refresh
- Works only on your device

---

### Recommended Tools

- AltStore (auto-refresh apps)
- Sideloadly (manual install)

---

## 🚀 Deployment

Deployed via:

- Vercel

No build step required.

---

## 🧠 Performance Principles

- Avoid excessive `backdrop-filter`
- Limit continuous animations
- Use IntersectionObserver for visibility-based effects
- No full DOM re-renders
- GPU-safe transforms only

---

## 🧼 Known Constraints

- Single-file architecture limits scalability
- Heavy animations may impact iOS Safari
- External APIs depend on availability

---

## 🔮 Future Evolution

- React migration (component architecture)
- Native iOS version (Capacitor / SwiftUI hybrid)
- Smart recommendations (behavior learning)
- Offline-first data sync

---

## 🎯 Project Status

> Transitioning from “beautiful interface” → “reliable system”

Focus areas:

- stability
- performance
- consistency

---

## 👤 Author

Pedro Werner  
São Paulo, Brazil


## 💬 Final Note

This project explores the boundary between:

- interface  
- system  
- experience  

The goal is not to build more features.

The goal is to build something that **feels alive**.

