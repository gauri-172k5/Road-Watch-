# ROADWATCH – Road Condition Monitoring System

> **"Monitor Roads. Report Damage. Improve Infrastructure."**

ROADWATCH is a complete, modern, professional, and fully interactive smart-city road infrastructure monitoring and maintenance web platform. Built as a high-performance **Frontend-Only** application using **HTML5, CSS3, and modern ES6+ JavaScript**, ROADWATCH uses browser **LocalStorage** as a relational client-side database to demonstrate end-to-end civic complaint management and highway authority operations.

---

## 📂 Project Structure

```
ROADWATCH/
│
├── index.html            # Public Landing Page & Citizen Portal
├── dashboard.html        # Municipal Operations Command Center
├── report.html           # Road Damage Intake Form (GPS + Multi-Photo Upload)
├── map.html              # Interactive GIS Map (Leaflet.js + OpenStreetMap)
├── tracking.html         # Live Complaint Tracking & Progress Stepper
├── maintenance.html      # Maintenance Task Management & Crew Dispatch
├── workers.html          # Field Worker Management & Simulated Worker Terminal
├── comparison.html       # Before & After Quality Assurance & Verification
├── sensors.html          # IoT Road Vibration & IRI Telemetry (Demo Module)
├── drone.html            # Drone Aerial Inspection & Photogrammetry Surveys
├── reports.html          # Analytics, Visual Breakdowns & CSV Data Export
├── notifications.html    # Operational Notifications & Alert Feed
├── profile.html          # Officer Profile & LocalStorage Demonstration Reset
│
├── css/
│   ├── style.css         # Master design system, variables, sidebar, buttons, modals
│   ├── dashboard.css     # Metric KPI cards, Chart.js containers, stepper, diff viewers
│   ├── forms.css         # Form controls, geolocation card, dropzones, filters
│   └── responsive.css    # Breakpoints for desktop, tablet, and mobile offcanvas
│
├── js/
│   ├── storage.js        # Centralized LocalStorage data engine, seed generator, compression
│   ├── main.js           # Unified sidebar navigation, live clock, toasts, counters
│   ├── dashboard.js      # Dynamic statistics, Chart.js graphs, critical alerts
│   ├── report.js         # Geolocation API integration, image compression, validation
│   ├── map.js            # Leaflet map pins, severity colors, search, user locator
│   ├── tracking.js       # Live progress stepper, complaint lookup, rejection handling
│   ├── maintenance.js    # Task assignment modal, priority rules, overdue checks
│   ├── workers.js        # Worker roster, availability tracking, simulated field mode
│   ├── comparison.js     # Side-by-side QA image viewer, administrative verification
│   ├── sensors.js        # Vibration RMS & IRI line charts, simulated spike trigger
│   ├── drone.js          # Aerial survey scheduler, damage linking, summaries
│   ├── reports.js        # Analytics KPI cards, polar charts, CSV file generator
│   └── notifications.js  # Read/unread feeds, clearance, quick-action routing
│
└── assets/
    ├── icons/            # SVG vector icons & favicon
    └── images/           # Lightweight SVG vector assets (potholes, cracks, workers)
```

---

## ⚡ Quick Start with VS Code Live Server

1. Open this folder (`road monitering`) in **VS Code**.
2. If not already installed, install the **Live Server** extension (by Ritwick Dey).
3. Right click on `index.html` (in root or inside `ROADWATCH/`) and select **"Open with Live Server"**.
4. The browser will open the application at:
   ```
   http://127.0.0.1:5500/ROADWATCH/index.html
   ```

*You can also directly double click `ROADWATCH/index.html` in Windows File Explorer.*

---

## 🔄 End-to-End Workflow Demonstration

1. **Citizen Files Damage Report (`report.html`)**:
   - Automated GPS geolocation via browser API (with city center fallback).
   - Multi-image upload with client-side canvas compression.
   - Generates unique complaint ID (`RW-YYYY-XXXX`).

2. **Operations Dashboard & Triage (`dashboard.html`)**:
   - Live KPI cards update dynamically from LocalStorage.
   - Chart.js graphs show damage type distributions, severity ratios, and monthly trends.
   - Critical damage alerts trigger immediately for high-severity hazards.
   - One-click complaint approval generates linked maintenance task.

3. **Spatial GIS Map (`map.html`)**:
   - Interactive OpenStreetMap via Leaflet.js.
   - Dynamic color-coded pins: **Red** (High Severity), **Orange** (Medium), **Green** (Low).
   - Real-time search and damage category filtering.

4. **Maintenance & Worker Dispatch (`maintenance.html` & `workers.html`)**:
   - Assign specialists, set repair deadlines, and adjust priorities (Urgent / Normal / Low).
   - Overdue warnings highlight automatically when deadlines pass.
   - Field worker demo mode allows updating task states from *Pending* to *In Progress*.

5. **Before & After Repair Quality Verification (`comparison.html`)**:
   - Side-by-side photo comparison of original damage and completed patch.
   - Upload after-repair photo and apply official engineering verification.
   - Marks complaint and maintenance task as *Completed*.

6. **Citizen Tracking (`tracking.html`)**:
   - Search by complaint ID.
   - Visual 6-stage progression timeline stepper.
   - Displays assigned crew and completion evidence.

7. **Smart Monitoring Prototyping (`sensors.html` & `drone.html`)**:
   - Clearly labeled IoT sensor telemetry with live vibration and International Roughness Index (IRI) charts.
   - Interactive vibration anomaly simulation button.
   - Drone aerial inspection flight scheduler and photogrammetry record.

8. **Analytics & Notifications (`reports.html` & `notifications.html`)**:
   - Area density analysis and category percentages.
   - One-click CSV dataset export and print-ready stylesheet.
   - Interactive notification feed with unread counter badges.
