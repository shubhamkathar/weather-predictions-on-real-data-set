🌤️ Delhi Climate Forecast and Analysis 📊

This project explores and forecasts the climate of Delhi using historical weather data. The project includes data visualization, time series forecasting with Prophet, and interactive user input for custom weather predictions.

📁 Dataset
File used: DailyDelhiClimateTrain.csv
Columns include:

date: Date of observation

meantemp: Mean temperature (°C)

humidity: Humidity level

wind_speed: Wind speed

meanpressure: Atmospheric pressure

🛠️ Libraries Used
pandas, numpy: Data manipulation

matplotlib, seaborn: Data visualization

plotly.express: Interactive visualizations

prophet: Forecasting model

datetime: Date manipulation

📈 Visual Explorations

Line Graphs (Plotly):

Mean Temperature, Humidity, and Wind Speed trends over time

Scatter Plot:

Relationship between humidity and temperature (with trendline)

Year-wise Monthly Trends:

Temperature change over years using Seaborn line plots

🔮 Forecasting with Facebook Prophet

Data formatted for Prophet with:

ds → Date

y → Mean temperature

Forecast generated for 365 future days

Humidity used as an external regressor to improve forecast accuracy

📅 User-Specific Prediction

User inputs a future date (e.g., 2024-03-31)

The model predicts:

Mean temperature (yhat)

Lower and upper bounds (yhat_lower, yhat_upper)

Predicted humidity (based on input or default)

🌡️ Weather Description Engine

Converts numerical predictions into understandable weather descriptions:

Temperature: Mild, Warm, Hot, etc.

Humidity: Dry, Moderately Humid, etc.

Example:

yaml
Copy
Edit
Predicted temperature for 2024-03-31 : 28.5°C
Predicted humidity for 2024-03-31 : 50
Description: Temperature: 28.5°C (Warm), Humidity: 50 - Very humid

▶️ How to Run
Ensure you have Python 3.7+ installed.
Install dependencies:
bash
Copy
Edit
pip install pandas numpy matplotlib seaborn plotly prophet
Run the script:

bash
Copy
Edit
python your_script_name.py
Enter a future date when prompted to get predictions.

📌 Notes
The Prophet model can be enhanced by using more regressors (wind_speed, pressure).
Forecasts are approximate and depend on historical data trends.
Date formatting and feature extraction (year, month) are used for seasonal analysis.

📊 Output Samples
Line and scatter plots open in an interactive Plotly window.
Console output includes forecasted temperature and humidity for any date provided by the user.

👨‍💻 Author
Shubham Kathar
Data Science & Python Developer | Climate Analytics Enthusiast
