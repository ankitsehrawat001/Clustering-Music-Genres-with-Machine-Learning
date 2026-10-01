# Sonic Atlas

Sonic Atlas is a music intelligence dashboard built with Python and Streamlit. It analyzes a Spotify-style music dataset, explores clustering patterns, and predicts which music segment a given song is most likely to belong to based on audio features.

## Project Overview

This project uses a music dataset containing attributes such as:

- Title
- Artist
- Top Genre
- Year
- BPM
- Energy
- Danceability
- Loudness
- Liveness
- Valence
- Acousticness
- Speechiness
- Popularity
- Music Segments

The app visualizes this data through interactive charts and provides a machine learning-based prediction interface for song segment classification.

## Features

- Interactive Streamlit dashboard
- Genre and year filtering
- KPI summary cards
- Trend analysis over time
- Scatter plots and box plots
- Correlation heatmap
- Music segment prediction using KNN classifier
- Data preview table

## Tech Stack

- Python
- Streamlit
- Pandas
- Plotly
- Scikit-learn
- NumPy

## Folder Structure

```bash
.
├── app.py
├── spotify_clustered_output.csv
├── requirements.txt
├── README.md
└── .venv/
```

## Setup

1. Open the project folder in your terminal.
2. Create and activate a virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

3. Install dependencies:

```powershell
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

## Run the App

```powershell
streamlit run app.py
```

Then open the local URL shown in the terminal, usually:

```text
http://localhost:8501
```

## Model Information

The prediction logic uses a K-Nearest Neighbors (KNN) model trained on selected audio features like BPM, Energy, Danceability, Valence, Popularity, and Year.

## Dataset

The app uses the file:

```bash
spotify_clustered_output.csv
```

This dataset has already been clustered and includes a `Music Segments` column for segment analysis.

## Notes

- The dashboard is designed for experimentation and visualization.
- The app can be extended with more advanced clustering or recommendation features in the future.

## License

This project is for educational and portfolio use.
