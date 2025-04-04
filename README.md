# 🌧️ WeatherPy – Global Weather Data Analysis

## 🌍 Overview

This project collects and analyzes global weather data based on randomly generated geographic coordinates. Using the OpenWeatherMap API, it extracts current weather metrics and explores relationships between latitude and weather conditions using visualizations and statistical summaries.

---

## 🧰 Technologies Used

- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- SciPy
- OpenWeatherMap API

---

## 📁 Project Files

```
WeatherPy/
├── WeatherPy.ipynb            # Main notebook with weather data collection and analysis
├── output_data/               # Saved CSV files and visualizations
├── config.py                  # API key stored securely (excluded from repo)
└── README.md                  # Project documentation
```

---

## 🔄 Workflow Summary

1. **Generate Coordinates**
   - Randomly generate lat/lon pairs across the globe
   - Use `citipy` to find the nearest city

2. **Collect Weather Data**
   - Query OpenWeatherMap API for each city
   - Retrieve temperature, humidity, cloudiness, wind speed, etc.
   - Store results in a Pandas DataFrame

3. **Clean & Save Data**
   - Remove duplicates or incomplete data
   - Export clean dataset to CSV

4. **Visualizations**
   - Create scatter plots to examine:
     - Latitude vs. Temperature
     - Latitude vs. Humidity
     - Latitude vs. Cloudiness
     - Latitude vs. Wind Speed

5. **Statistical Analysis**
   - Split data into Northern and Southern Hemispheres
   - Run linear regression using SciPy for each relationship

---

## 📊 Sample Output

- Plots show trends such as warmer temps near equator
- Linear regression reveals correlation strengths
- Final report includes annotated plots and R-squared values

---

## 🚀 How to Run

1. Add your OpenWeatherMap API key to `config.py`:
```python
weather_api_key = "YOUR_API_KEY"
```

2. Run `WeatherPy.ipynb` in Jupyter:
```bash
jupyter notebook WeatherPy.ipynb
```

3. Output charts and data are saved to `output_data/`

> Note: You may hit API rate limits. Code includes `time.sleep()` delay.

---

## 📌 Future Improvements

- Automate daily weather pull and append to time series
- Visualize data on an interactive map using Plotly or Folium
- Add real-time weather alerts or forecast comparisons

---

**Author:** [Geo222222](https://github.com/Geo222222)  
**Focus:** Weather Data • API Automation • Exploratory Data Analysis

