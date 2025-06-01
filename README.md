# ETL-project
### Overview

This project implements an ETL (Extract, Transform, Load) pipeline to fetch, process, and visualize intraday stock price data for IBM using the Alpha Vantage API. The data is extracted in 5-minute intervals, transformed into a structured format, and loaded into a SQLite database. Dashboards are created using Dash and Plotly for real-time stock price visualization.

### Features





Extract: Fetches intraday (5-minute) stock data for IBM from the Alpha Vantage API.



Transform: Cleans the data by removing duplicates, handling missing values, and converting columns to numeric types. Adds calculated fields like Daily Change and Percentage Change.



Load: Stores the processed data in a SQLite database (stocks_data.db).



Visualization: Provides two interactive Dash dashboards:





A line plot of opening stock prices over time.



A combined line plot comparing closing prices and opening prices over time.

### Requirements

To run this project, install the following Python packages:





requests



pandas



openpyxl



sqlalchemy



dash



plotly

You can install them using pip:

pip install requests pandas openpyxl sqlalchemy dash plotly

### Usage





API Key: Replace the apikey value in the notebook (XO6PY6AABZ9SDAXI) with your own Alpha Vantage API key. Obtain one from Alpha Vantage.



Run the Notebook:





Open my_project_etl.ipynb in Jupyter Notebook or a compatible environment.



Execute the cells sequentially to:





Fetch data from the Alpha Vantage API.



Transform the data (cleaning, type conversion, and calculations).



Load the data into a SQLite database (stocks_data.db).



Launch two Dash dashboards for visualization.



Dashboards:





The first dashboard (port 8052) displays a line plot of opening stock prices.



The second dashboard (port 8051) shows a combined line plot of closing and opening prices.



Access the dashboards in your browser at http://127.0.0.1:8052 and http://127.0.0.1:8051.

### Project Structure





my_project_etl.ipynb: The main Jupyter Notebook containing the ETL pipeline and visualization code.



