# Real-Time Transaction Anomaly Detection

This project monitors transaction data to detect anomalies and send real-time email alerts. Using historical data, we set thresholds and process incoming data to identify and report anomalies.

## Files
- **transactions_1.csv**: Historical transaction data for day 1.
- **transactions_2.csv**: Historical transaction data for day 2.
- **checkout_1.csv**: Historical data of sales on POS 1.
- **checkout_2.csv**: Historical data of sales on POS 2.
- **alert.ipynb**: Jupyter Notebook with code for real-time monitoring and email alerts.
- **anomalies.ipynb**: Jupyter Notebook for detecting anomalies in historical data.

## Setup
1. Clone this repository. 
2. Install all dependencies:
   ```sh
   pip install pandas smtplib

## Usage

1. Detect anomalies in historical data:
-  Use **`anomalies.ipynb`** to load and analyze data from **`checkout_1.csv`** and **`checkout_2.csv`** to find anomalies.

2. Analyze historical data and calculate thresholds:
- Use **`alert.ipynb`** to load data from **`transactions_1.csv`** and **`transactions_2.csv`**.
- Calculate thresholds based on historical data.
- Set up email alert functions to signal if transaction statuses exceed specified thresholds.

## How It Works

1. **anomalies.ipynb**:
- Load and prepare data from **`checkout_1.csv`** and **`checkout_2.csv`**.
- Detect anomalies based on predefined rules or thresholds.

2. **alert.ipynb**:
- Load and prepare data from **`transactions_1.csv`** and **`transactions_2.csv`**.
- Calculate thresholds for anomaly detection.
- Continuously process incoming transactions and detect anomalies.
- Send email alerts when anomalies exceed thresholds.
