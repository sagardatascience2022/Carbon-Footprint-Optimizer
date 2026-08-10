# Carbon Footprint Optimizer 🌍

[![Python](https://img.shields.io/badge/python-3.14-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/streamlit-supported-orange.svg)](https://streamlit.io/)
[![License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](#)

A clean and interactive Streamlit app for estimating CO₂ emissions in supply chain logistics. Enter route details, compare predicted emissions with formulaic estimates, and visualize delivery routes on a Folium map.

---

## 🚀 What it does

- Converts source/destination text into geolocation coordinates
- Requests driving route information using OpenRouteService
- Predicts CO₂ emissions using a pre-trained ML model
- Calculates fuel consumption and cost
- Displays an interactive route map with Folium
- Stores recent delivery predictions in a dashboard
- Allows export of individual delivery reports and dashboard data as CSV

## ✨ Why it’s useful

- Helps logistics planners estimate environmental impact quickly
- Supports highway-route optimization decisions
- Offers side-by-side model prediction and formula-based CO₂ results
- Supports quick scenario testing for different vehicle types, traffic, and weather

## 📦 Requirements

- Python 3.14
- `streamlit`
- `joblib`
- `folium`
- `streamlit-folium`
- `openrouteservice`
- `geopy`
- `pandas`
- `scikit-learn`

> All dependencies are listed in `requirements.txt`.

## 🛠️ Install

```bash
python -m pip install -r requirements.txt
```

## ▶️ Run locally

```bash
streamlit run streamlit_app.py
```

Then open the local Streamlit URL shown in the terminal.

## 🔧 Configuration

- `carbon_emission_model.pkl` contains the trained CO₂ prediction model.
- `streamlit_app.py` uses an OpenRouteService API key and OpenWeatherMap key for route and weather data.
- Update API keys in `streamlit_app.py` if you want to use your own credentials.

## 💡 Notes

- Requires network access for geocoding and route/weather APIs.
- The app is designed for quick prototype evaluation and dashboard exploration.

## 📁 Project files

- `streamlit_app.py` — main Streamlit app
- `requirements.txt` — project dependencies
- `carbon_emission_model.pkl` — trained emission prediction model
- `carbon_logistics_dataset.csv` — dataset used for training or reference

## 📝 License

This project is provided as-is. Update the license badge and section if you add a license file later.
