# squash_tabella_demo
Demo of Squash Tabella webapp
<img width="1526" height="771" alt="image" src="https://github.com/user-attachments/assets/f1713567-70e5-4e27-a1e6-ed83c672a2f9" />


🏸 Squash Leaderboard & Analytics Dashboard

Live Demo: Play the App Here
Source Code: View Repository
Overview

A full-stack web application developed to track, analyze, and visualize match data for a private squash league. This project replaces manual scorekeeping with a fully automated, cloud-synced solution. It demonstrates end-to-end data pipeline management, algorithmic feature engineering, and interactive data visualization.
✨ Key Features

    Algorithmic Ranking System: Implements a dynamic Elo rating system (using a K-factor of 32) that automatically calculates and updates player rankings based on match outcomes.  

    Cloud Backend Integration: Utilizes the Google Sheets API (via streamlit-gsheets) to seamlessly read, record, and update match data in real-time without requiring a traditional SQL database.  

    Interactive Data Visualization: Generates dynamic Elo rating history line charts using the Altair library, allowing users to track player progression over a timeline of matches.  

    Advanced Head-to-Head Analytics: Provides deep 1v1 rivalry statistics, calculating win rates, average point differentials, and "Match Stakes" (predicting potential Elo gains or losses prior to a match).  

    Outlier Detection: Automatically parses historical data to identify significant match events, highlighting "Biggest Blowouts" and close "Nail-biters".  

    In-App Data Management: Features an integrated data editor that allows users to directly modify and sync the records of the last 10 matches to the cloud backend.  

🛠️ Tech Stack

    Frontend & Framework: Streamlit, Python  

    Data Manipulation: Pandas  

    Data Visualization: Altair  

    Database / API: Google Sheets API (GSheetsConnection)  

🚀 How to Run Locally

To run this dashboard on your local machine, follow these steps:

    Clone the repository:
    Bash

    git clone https://github.com/ambrusfarkas/squash_tabella_demo.git
    cd squash_tabella_demo

    Install the required dependencies:
    (Ensure you have a requirements.txt file in your repo containing streamlit, pandas, altair, and st-gsheets-connection)
    Bash

    pip install -r requirements.txt

    Run the Streamlit app:
    Bash

    streamlit run app.py

📊 Why This Project Matters

While built for a recreational sports league, the underlying architecture mirrors enterprise data solutions. It involves ETL (Extract, Transform, Load) processes from a cloud source, custom algorithm development, and the creation of an interactive, user-facing dashboard designed to turn raw data into actionable insights.
