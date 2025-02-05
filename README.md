# WeatherPy & VacationPy

## Overview
This project leverages Python and various APIs to analyze weather patterns and suggest vacation destinations based on user-defined criteria. It consists of two main components:

1. **WeatherPy** - Performs weather data analysis and visualization.
2. **VacationPy** - Uses the analyzed weather data to suggest travel destinations and map nearby hotels.

---

## WeatherPy
### Description
WeatherPy pulls live weather data from the OpenWeatherMap API for randomly generated cities worldwide. The analysis includes:
- Temperature vs. Latitude
- Humidity vs. Latitude
- Cloudiness vs. Latitude
- Wind Speed vs. Latitude
- Linear regression for northern and southern hemispheres

### Technologies Used
- Python (Pandas, NumPy, Matplotlib, SciPy)
- OpenWeatherMap API
- Jupyter Notebook

### Steps
1. Generate random cities and their coordinates.
2. Fetch weather data using OpenWeatherMap API.
3. Clean and analyze the dataset.
4. Visualize the relationships between latitude and weather conditions.

---

## VacationPy
### Description
VacationPy takes the cleaned weather data from WeatherPy and filters cities based on user-preferred conditions (e.g., warm temperatures and clear skies). Then, it locates nearby hotels using the Geoapify API.

### Technologies Used
- Python (Pandas, Requests, hvPlot, Matplotlib)
- Geoapify API
- OpenStreetMap (hvPlot)
- Jupyter Notebook

### Steps
1. Load the cleaned weather dataset from WeatherPy.
2. Filter cities based on user-preferred weather conditions.
3. Use Geoapify API to find hotels near the selected destinations.
4. Plot the results on an interactive map.

---

## Setup Instructions
1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd WeatherPy-VacationPy
   ```
2. Install required Python libraries:
   ```sh
   pip install pandas numpy matplotlib requests scipy hvplot
   ```
3. Obtain API keys:
   - OpenWeatherMap API Key
   - Geoapify API Key
4. Store API keys in a separate file (`api_keys.py`):
   ```python
   weather_api_key = "YOUR_OPENWEATHERMAP_KEY"
   geoapify_key = "YOUR_GEOAPIFY_KEY"
   ```
5. Run the Jupyter Notebooks:
   ```sh
   jupyter notebook
   ```
6. Open `WeatherPy.ipynb` to run weather analysis.
7. Open `VacationPy.ipynb` to find vacation spots based on weather conditions.

---

## Results & Insights
- The data visualizations show how latitude influences temperature, humidity, cloudiness, and wind speed.
- Cities with favorable weather conditions were identified as potential vacation destinations.
- Nearby hotels were successfully mapped to aid in travel planning.

---

## Future Enhancements
- Integrate a user interface for input preferences.
- Expand the analysis to include additional climate factors.
- Improve hotel recommendations with more filters (e.g., ratings, price range).




