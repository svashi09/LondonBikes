# LondonBikes
London Bike Rides - Data Analytics &amp; Visualisation | Python, Jupyter, Tableau

LondonBikes 🚴‍♀️

Analyze, visualize, and derive insights from London’s bike-sharing data using Python and Tableau.

📋 Project Overview

The LondonBikes project merges trip logs, weather, and date/time information to investigate usage trends in London’s public bike-share system. By cleaning and transforming the data, generating features like moving averages and weather flags, and visualizing results in Tableau, the project uncovers daily/time-based patterns and weather-driven changes in usage.

🧰 Tech Stack
	•	Python for data cleaning, aggregation, and analysis
	•	Jupyter Notebook – for interactive analysis and exploration
	•	Tableau – for building interactive dashboards (total rides time-series, 14-day moving average, temperature–wind heatmap)

⚙️ Key Features
	•	Data cleaning: formatting, handling missing data, feature engineering
	•	Time-based breakdown: daily, hourly, weekday vs weekend
	•	Computed moving averages to smooth trends
	•	Weather integration: identified usage patterns tied to temperature and wind speed
	•	Interactive dashboard summarizing insights and trends

📊 Example Insights
	•	Highest ride volumes observed in spring months, with clear weekday commute peaks
	•	Moderate temperatures (12–15 °C) and lower wind speeds significantly boost ridership
	•	Periods of leisure rides during pleasant weather, not just commuting

🛠 Installation & Setup
	1. Clone this repository:
     git clone https://github.com/svashi09/LondonBikes.git

  2. Install Python dependency:
     pip install pandas numpy matplotlib seaborn

  3. Launch the analysis notebook:
     jupyter notebook LondonBikeAnalysis.ipynb

  4. Open the Tableau dashboard (LondonBikeDashboard.twb or .twbx) in Tableau Desktop or Public.

📁 Data
	•	london_merged.csv
  "timestamp" - timestamp field for grouping the data
  "cnt" - the count of a new bike shares
  "t1" - real temperature in C
  "t2" - temperature in C "feels like"
  "hum" - humidity in percentage
  "wind_speed" - wind speed in km/h
  "weather_code" - category of the weather
  "is_holiday" - boolean field - 1 holiday / 0 non holiday
  "is_weekend" - boolean field - 1 if the day is weekend
  "season" - category field meteorological seasons: 0-spring ; 1-summer; 2-fall; 3-winter.

  "weathe_code" category description:
  1 = Clear ; mostly clear but have some values with haze/fog/patches of fog/ fog in vicinity 2 = scattered clouds / few clouds 3 = Broken clouds 4 = Cloudy 7 = Rain/     light Rain shower/ Light rain 10 = rain with thunderstorm 26 = snowfall 94 = Freezing Fog
