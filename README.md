# squash_tabella_demo
Demo of Squash Tabella webapp
<img width="1526" height="771" alt="image" src="https://github.com/user-attachments/assets/f1713567-70e5-4e27-a1e6-ed83c672a2f9" />


🏸 **Squash Leaderboard & Analytics Dashboard**

[Live Demo](https://squash-tabella-demo.streamlit.app/)

[Source Code](https://github.com/ambrusfarkas/squash_tabella_demo)

A full-stack web application developed to track, analyze, and visualize match data for a private squash league. This project replaces manual scorekeeping with a fully automated, cloud-synced solution. While built for a recreational sport, the underlying architecture mirrors enterprise data solutions, demonstrating end-to-end data pipeline management, custom algorithm development, and interactive data visualization.
✨ Key Features

    Algorithmic Ranking System: Implements a dynamic Elo rating system that automatically calculates and updates player rankings based on match outcomes[cite: 3].

    Cloud Backend Integration: Utilizes the Google Sheets API to seamlessly read, record, and update match data in real-time without requiring a traditional SQL database[cite: 3].

    Interactive Data Visualization: Generates dynamic Elo rating history line charts using the Altair library, allowing users to track player progression over a timeline of matches[cite: 3].

    Advanced Head-to-Head Analytics: Provides deep 1v1 rivalry statistics, calculating win rates, average point differentials, and predicting potential Elo gains/losses prior to a match[cite: 3].

    In-App Data Management: Features an integrated data editor that allows users to directly modify and sync recent match records to the cloud backend[cite: 3].

🛠️ Tech Stack

    Frontend & Framework: Python, Streamlit[cite: 3]

    Data Manipulation: Pandas[cite: 3]

    Data Visualization: Altair[cite: 3]

    Database Integration: Google Sheets API (streamlit-gsheets)
