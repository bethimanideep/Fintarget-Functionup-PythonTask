# OLHC Data and Moving Averages Calculator
## Overview

OLHC Data and Moving Averages Calculator is a Python script that connects to a WebSocket to fetch live data for financial instruments (Nifty, Banknifty, Finnifty) and calculates Open, Low, High, Close (OLHC) data for each minute. It also computes the Simple Moving Average (SMA) for the Close prices using a window size of 3. The script saves OLHC data and moving averages to CSV files for further analysis.

# Technologies
- Python
- Websockets

# Installation
## windows
 ```bash
git clone https://github.com/bethimanideep/Fintarget-Functionup-PythonTask
cd Fintarget-Functionup-PythonTask
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python app.py
   ```
## linux
 ```bash
git clone https://github.com/bethimanideep/Fintarget-Functionup-PythonTask
cd Fintarget-Functionup-PythonTask
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python3 app.py
   ```

## WebSocket Connection

The script establishes a WebSocket connection to the provided URL (wss://functionup.fintarget.in/ws?id=fintarget-functionup) to receive live data for financial instruments.

## OLHC Data Calculation

OLHC data, representing Open, Low, High, Close prices, is calculated for each minute. The script stores this data in a CSV file named "olhc_data.csv" for further reference.

## Moving Averages Calculation

Moving Averages (SMA) are computed for the Close prices with a window size of 3. The moving averages data is saved separately for each instrument (Nifty, Banknifty, Finnifty) in CSV files (e.g., "moving_averages_Nifty.csv").
