**ETL Pipeline Project**

Overview:
This project is a simple ETL (Extract, Transform, Load) pipeline built using Python. The pipeline extracts weather data from the OpenWeather API, processes it, and stores it in a local SQLite database.

Features:
Extract: Fetches real-time weather data from the OpenWeather API for a given city.
Transform: Processes the data to extract relevant fields like temperature, weather description, and timestamps.
Load: Stores the transformed data in a local SQLite database (weather_data.db).

Prerequisites:

To run this project, you will need

1. Python 3.7+ installed.
2. An API key from OpenWeather.

**Setup Instructions:
1. Clone the repository:

git clone https://github.com/Vishal44319/ETL-Pipeline.git
cd ETL-Pipeline

3. Create a virtual environment and install dependencies:

python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt

3. Set your OpenWeather API key in the etl_pipeline.py file.

4. Run the ETL pipeline:

python etl_pipeline.py

**How It Works

Extract:
The pipeline uses the OpenWeather API to request current weather data for the specified city.

Transform:
The raw data from the API is filtered, keeping only necessary information such as temperature, weather conditions, and date.

Load:
The processed data is inserted into an SQLite database, where each row represents a snapshot of the weather data at a specific time.
