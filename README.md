# 📈 Stock ETL Project
### 🌟 Overview
Welcome to the Stock ETL Project! This dynamic pipeline extracts intraday stock price data for IBM from the Alpha Vantage API, transforms it into a clean, structured format, and loads it into a SQLite database. Interactive dashboards built with Dash and Plotly bring the data to life, offering real-time insights into stock trends!
### ✨ Features

Extract: Pulls 5-minute interval stock data for IBM via the Alpha Vantage API.
Transform: Cleans data by removing duplicates and nulls, converts to numeric types, and calculates:
Daily Change: Close price - Open price
Percentage Change: (Close - Open) / Open * 100


Load: Stores processed data in a SQLite database (stocks_data.db).
Visualization: Two stunning, interactive dashboards:
📊 Line plot of opening prices over time.
📈 Combined line plot of closing vs. opening prices for trend analysis.



### 🛠️ Requirements
To dive in, install these Python packages:
pip install requests pandas openpyxl sqlalchemy dash plotly

### 🚀 Usage

API Key




Grab your free Alpha Vantage API key from Alpha Vantage. Replace the apikey value (XO6PY6AABZ9SDAXI) in my_project_etl.ipynb with yours.

Run the Notebook  
Open my_project_etl.ipynb in Jupyter Notebook or a similar environment.
Run cells in order to:
Fetch raw data from the API.
Clean and enhance the data with calculated metrics.
Save it to stocks_data.db.
Launch dazzling Dash dashboards!




Dashboards  
🌐 Opening Prices: A sleek line plot at http://127.0.0.1:8052.


🌐 Open vs. Close: A vibrant combined plot at http://127.0.0.1:8051.
Interact with the charts in your browser for real-time insights!



### 📂 Project Structure

my_project_etl.ipynb: Your all-in-one ETL and visualization script.
stocks_data.db: The SQLite database housing your transformed stock data.

### 📊 Data Source

API: Alpha Vantage TIME_SERIES_INTRADAY  
Symbol: IBM  
Interval: 5 minutes  
Fields: Open, High, Low, Close, Volume  
Derived Metrics: Daily Change, Percentage Change

### ⚠️ Notes

Ensure an active internet connection for API calls.
Alpha Vantage has rate limits—consider a premium key for heavy use.
Dashboards run locally on ports 8051 and 8052; confirm they’re available.
Sample data is from May 30, 2025. Tweak the API call for live updates!

### 📜 License
This project is licensed under the MIT License. Use, tweak, and share it freely!
### 🤝 Contributing
Love to see your ideas! Here’s how to contribute:

Fork this repo.
Create a branch for your feature or fix.
Submit a pull request with a clear rundown of your changes.

### 📬 Contact
Got questions? Open an issue on GitHub or ping the project maintainer. Let’s make this project shine! 🌟

Built with 💻 and a passion for data!
