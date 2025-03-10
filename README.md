# python-api-challenge

## Weather and Vacation Analysis

## Overview
This project explores the relationship between weather patterns and latitude using Python, APIs, and data visualization techniques. By analyzing weather data from over 500 cities worldwide, we can observe how temperature, humidity, wind speed, and cloudiness vary with distance from the equator. The project consists of two main parts:

1. **WeatherPy**: Analyzing and visualizing weather trends.
2. **VacationPy**: Using weather data to identify ideal vacation destinations.

## Technologies Used
- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- SciPy
- Requests (API calls)
- Geoapify API
- OpenWeatherMap API
- Citipy
- geoViews

---

## Part 1: WeatherPy
In this section, we collect and visualize weather data from different cities using APIs and data science techniques.

### Steps:
1. **Retrieve Weather Data:**
   - Use the OpenWeatherMap API to obtain weather data for randomly generated cities.
   - Generate latitude and longitude coordinates using the Citipy library.
2. **Create Scatter Plots:**
   - Latitude vs. Temperature
   - Latitude vs. Humidity
   - Latitude vs. Cloudiness
   - Latitude vs. Wind Speed
3. **Linear Regression Analysis:**
   - Separate data into Northern and Southern Hemispheres.
   - Compute linear regression for each variable.
   - Display regression line, formula, and R-squared values.
4. **Interpret Findings:**
   - Explain observed trends and correlations between latitude and weather variables.

---

## Part 2: VacationPy
In this section, we use weather data to help identify potential vacation destinations based on ideal weather conditions.

### Steps:
1. **Create a City Map:**
   - Visualize all cities on a map with humidity levels affecting point sizes.
2. **Filter for Ideal Vacation Conditions:**
   - Define criteria (e.g., temperature range, wind speed, cloudiness) to filter cities.
   - Store filtered cities in a new DataFrame (`hotel_df`).
3. **Find Nearby Hotels:**
   - Use the Geoapify API to locate hotels within 10,000 meters of each selected city.
   - Store hotel names and country information.
4. **Generate a Vacation Map:**
   - Display selected vacation spots with hotel details in hover messages.

---

## Installation and Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repository/weather-vacation-analysis.git
   cd weather-vacation-analysis
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Obtain API keys from:
   - [OpenWeatherMap](https://openweathermap.org/api)
   - [Geoapify](https://www.geoapify.com/)
4. Store API keys in a `.env` file or within the notebook as variables.
5. Run Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
6. Open and execute `WeatherPy.ipynb` and `VacationPy.ipynb`.

---

## Results and Insights
- The analysis confirms that temperature has a strong correlation with latitude, decreasing as we move away from the equator.
- Humidity, wind speed, and cloudiness show weaker correlations but still exhibit distinct trends.
- The vacation map successfully highlights cities with ideal weather and nearby hotels, demonstrating a practical application of weather data analysis.

---

## Author
Brian Hart  
University of Texas Austin - Data Visualization and Analysis Bootcamp  

---

## License
This project is for educational purposes and follows standard open-source licensing. Feel free to use and modify for learning purposes.
