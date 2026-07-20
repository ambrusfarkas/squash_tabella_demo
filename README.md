# 🏸 Squash Tabella

**A leaderboard & analytics dashboard for a private squash league** — built with Streamlit, powered by a live Elo rating engine and synced to Google Sheets in real time.

![Squash Tabella dashboard preview](https://github.com/user-attachments/assets/f1713567-70e5-4e27-a1e6-ed83c672a2f9)
<img width="1472" height="757" alt="image" src="https://github.com/user-attachments/assets/bd871887-dd07-4c9a-acdc-44bae45d9dce" />


[**🔴 Live Demo**](https://squash-tabella-demo.streamlit.app/) · [**Source Code**](https://github.com/ambrusfarkas/squash_tabella_demo)

---

## Overview

Squash Tabella replaces manual scorekeeping with a fully automated, cloud-synced dashboard. Built for a recreational league, it mirrors the architecture of enterprise data tools — an end-to-end pipeline covering data ingestion, custom algorithms, and interactive visualization.

## ✨ Features

- **🔮 Dynamic Elo Ratings** — automatically recalculates rankings after every match
- **☁️ Cloud-Synced Backend** — reads and writes match data live via the Google Sheets API (no SQL database needed)
- **📈 Elo History Charts** — interactive Altair line charts tracking player progression over time
- **⚔️ Head-to-Head Analytics** — win rates, point differentials, and predicted Elo swings for any 1v1 matchup
- **📝 In-App Data Editing** — add or correct recent matches directly from the dashboard, synced instantly

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend / App | [Streamlit](https://streamlit.io/) |
| Data Manipulation | [Pandas](https://pandas.pydata.org/) |
| Visualization | [Altair](https://altair-viz.github.io/) |
| Backend / Storage | Google Sheets API ([streamlit-gsheets](https://github.com/streamlit/gsheets-connector)) |

## 🚀 Getting Started

```bash
git clone https://github.com/ambrusfarkas/squash_tabella_demo.git
cd squash_tabella_demo
pip install -r requirements.txt
streamlit run app.py
```

You'll need a Google Sheet connected via `streamlit-gsheets` — see [Streamlit's GSheets connection docs](https://docs.streamlit.io/develop/tutorials/databases/private-gsheet) for setup.

## 📄 License

MIT
