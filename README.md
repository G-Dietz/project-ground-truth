# 🌍 Project Ground Truth | Global Telemetry Dashboard

**A real-time visualization interface for monitoring expedition telemetry across 39 distinct geological and ecological landmarks.**

[**🔴 LIVE DEMO: Click here to view the Dashboard**](https://g-dietz.github.io/project-ground-truth/)

## 📖 Overview

**Project Ground Truth** is a multi-disciplinary expedition dashboard that correlates deep-time geological data with modern economic indicators. The application visualizes a global dataset spanning from the "Cradle of Agriculture" in Mexico to the ancient stromatolites of Australia.

The dashboard serves as the "Mission Control" interface, providing an interactive map and detailed data overlays for each waypoint on the expedition route.

## ✨ Key Features

* **Interactive Cartography:** A dynamic global map powered by **Leaflet.js** and CartoCDN dark-mode tiles.
* **Live Telemetry Panel:**
    * **Economic Indicators:** Real-time visualization of Inflation, GDP Growth, and Gini Coefficients using **Recharts**.
    * **Deep Time Visualization:** A logarithmic-scale gauge visualizing the geological age of the site (ranging from 0 to 4 Billion years).
    * **Biodiversity Index:** Estimated biological diversity scores.
* **Zero-Build Architecture:** Built using React and Babel standalone, requiring no build steps or node modules to run.

## 🛠️ Technology Stack

### Frontend (The Dashboard)
* **React 18:** Component-based UI logic.
* **Tailwind CSS:** Utility-first styling for the "Glassmorphism" UI.
* **Leaflet:** Interactive mapping library.
* **Recharts:** Data composition and chart rendering.

### Analytics (Offline Analysis)
* **Python:** For static data processing.
* **Pandas & Matplotlib:** For generating static analytics reports and trajectory plots.

## 📂 Project Structure

| File | Description |
| :--- | :--- |
| `index.html` | **The Main Application.** Contains the full React code, styles, and logic. Open this to view the dashboard. |
| `analytics.py` | A Python script that generates static charts (`.png`) and analyzes the dataset correlations. |
| `ground_truth_data.json` | The raw JSON dataset containing coordinates, economic stats, and field notes for all 39 locations. |

## 🚀 How to Run Locally

### 1. The Dashboard (Web)
Because this project uses a "Zero-Build" approach, you do not need `npm` or `node.js`.
1.  Clone or download this repository.
2.  Double-click `index.html` to open it in any modern web browser.
3.  **That's it!**

### 2. The Analytics Script (Python)
To generate the static analytics charts:
1.  Ensure you have Python installed.
2.  Install dependencies:
    ```bash
    pip install pandas matplotlib
    ```
3.  Run the script:
    ```bash
    python analytics.py
    ```
4.  Check the folder for the generated `ground_truth_dashboard_full.png`.

## 🌐 Deployment (GitHub Pages)

This project is deployed using GitHub Pages.
1.  Go to **Settings** > **Pages**.
2.  Select `main` branch as the source.
3.  The live link will be generated automatically.

---
*Mission Status: ACTIVE* 🟢