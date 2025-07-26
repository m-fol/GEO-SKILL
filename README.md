# 🌲 Mapping Biodiversity and Human Impact in Greek Forests 🌲

<p align="center">
  <img src="https://github.com/user-attachments/assets/6b652bd3-e9f8-44c0-ac71-a0e642cb8abe" 
       width="926" 
       height="351" 
       alt="image" />
</p>

**Forest Risk Explorer** is a web-based GIS application that visualizes forest health across Greece using Sentinel-2 NDVI data, protected biodiversity zones, and human activity layers informed by ESCO skill categories. Designed with the context of Earth Observation (EO) and the European Space Agency (ESA) in mind, this tool demonstrates how remote sensing and occupational data can be combined to explore environmental change and socio-economic impact.

---

## 🎯 Objectives

- Monitor forest degradation trends in Greece from 2017–2024 using NDVI indices
- Overlay critical biodiversity hotspots such as Natura 2000 zones
- Integrate human activity zones related to forestry, agriculture, and conservation using simulated ESCO data
- Provide an intuitive, browser-based GIS experience using Leaflet.js and open geospatial standards

---

## 📂 Project Structure

```
forest-risk-explorer/
├── index.html              # The main interactive map app
└── data/                   # GeoJSON files used for dynamic layers
    ├── ndvi_2020.geojson
    ├── ndvi_2021.geojson
    ├── ndvi_2022.geojson
    ├── biodiversity.geojson
    └── esco.geojson
```

---

## 🗺️ Data Sources & Assumptions

- **NDVI layers** were generated using Sentinel-2 SR data from the Copernicus program via Google Earth Engine. Each file contains simplified mock polygons simulating vegetation health.
- **Biodiversity zones** are based on public Natura 2000 protected areas and represent ecologically sensitive forest regions.
- **ESCO skill areas** were derived using OpenStreetMap land use data and manually assigned ESCO skill tags such as Forestry and Agricultural Management.

All mock data was generated to reflect realistic spatial distributions and thematic patterns.

---

## 💻 How to Run

### Option 1: Local (No Server Needed)
Just open `index.html` in your browser, and ensure the `/data/` folder is in the same directory.

### Option 2: Using Python HTTP Server
```bash
cd forest-risk-explorer
python3 -m http.server
```
Then visit: [http://localhost:8000](http://localhost:8000)

### Option 3: Deploy to GitHub Pages
1. Push this repo to GitHub
2. Enable GitHub Pages in **Settings → Pages**
3. Set source to `main` and folder to `/ (root)`

---

## 📚 Academic Relevance

This application demonstrates the practical intersection of:
- **Remote sensing & EO data processing** (NDVI, Sentinel-2)
- **Spatial biodiversity conservation**
- **Skill sector geospatial mapping using ESCO and land use**
- **Open-source GIS technology** (Leaflet.js, GeoJSON, OSM)

It is suitable for research, policy exploration, ESA EO training projects, and academic presentations on sustainability, environmental monitoring, and geospatial web applications.

---

## 👨‍🔬 Author

**Forest Risk Explorer** was developed for educational and research purposes in alignment with the European Space Agency’s educational initiatives. It may serve as a basis for further expansion into real-time EO monitoring dashboards, occupational analysis systems, or forest policy decision support tools.

---
