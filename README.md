# 🏸 Squash Tabella

**A leaderboard & analytics dashboard for tracking casual squash matches with friends** — built with Streamlit, powered by a live Elo rating engine and synced to Google Sheets in real time.

![Squash Tabella dashboard preview](https://github.com/user-attachments/assets/f1713567-70e5-4e27-a1e6-ed83c672a2f9)
<img width="1519" height="770" alt="image" src="https://github.com/user-attachments/assets/e431ecf9-d992-4a8c-9658-d113cf414fa9" />

[**🔴 Live Demo**](https://squash-tabella-demo.streamlit.app/) · [**Source Code**](https://github.com/ambrusfarkas/squash_tabella_demo)

---

## Overview

Squash Tabella replaces manual scorekeeping with a fully automated, cloud-synced dashboard for tracking matches between friends. It's a small project, but the underlying architecture mirrors enterprise data tools — an end-to-end pipeline covering data ingestion, custom algorithms, and interactive visualization.

## 💡 Motivation

I wanted a simple way to track our matches and see who's actually improving, but couldn't find an existing app that was free, easy to use, synced across devices, and had a proper Elo system with head-to-head stats — most tools on the market are either sport-specific league managers or paid, over-engineered platforms. So I built my own, with a few extras along the way:

- Fully customizable, tweakable ranking/Elo logic
- A secure backend (Google Sheets) with no risk of data loss from local corruption

## ✨ Features

- **Dynamic Elo Ratings** — automatically recalculates rankings after every match
- **Cloud-Synced Backend** — reads and writes match data live via the Google Sheets API (no SQL database needed)
- **Elo History Charts** — interactive Altair line charts tracking player progression over time
- **Head-to-Head Analytics** — win rates, point differentials, and predicted Elo swings for any 1v1 matchup
- **In-App Data Editing** — add or correct recent matches directly from the dashboard, synced instantly

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
