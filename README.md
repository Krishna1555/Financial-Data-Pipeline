
# Financial Data Pipeline & Quality Monitor

A Python project that checks financial data for errors, cleans it, stores it in a database, and displays the results on a simple dashboard.

## About the Project

This project helps process and validate financial data before it is used for analysis.

It works with three types of data: market prices, portfolio positions, and transactions. It checks for missing values, duplicates, and incorrect data before cleaning and storing the results in an SQLite database.

The dashboard is built using Streamlit and shows pipeline status and data quality results.

## Features

- Loads financial data from CSV files.
- Checks for missing values, duplicates, and incorrect entries.
- Uses YAML files to manage validation rules.
- Cleans data and adds useful calculated columns.
- Stores processed data in SQLite.
- Displays results using a Streamlit dashboard.

## Tech Stack

- Python
- Pandas
- SQLite
- SQLAlchemy
- Streamlit
- Plotly
- PyYAML
- APScheduler

## How to Run

Clone the repository and install the required packages:

```bash
git clone <YOUR-REPOSITORY-URL>
cd <YOUR-REPOSITORY-NAME>
pip install -r requirements.txt
```

Generate sample data:

```bash
python scripts/generate_sample_data.py
```

Start the dashboard:

```bash
streamlit run app.py
```

Open the local URL shown in your terminal and click **Run Now** to run the pipeline.

## What I Learned

- Working with financial datasets using Python and Pandas.
- Cleaning and validating data.
- Storing data in an SQLite database.
- Building a dashboard with Streamlit.
- Handling errors and working with background jobs.
