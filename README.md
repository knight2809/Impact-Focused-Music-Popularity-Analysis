# Impact-Focused-Music-Popularity-Analysis
A data-driven exploratory data analysis (EDA) of Spotify tracks using Python to uncover the key audio features and trends that separate viral hits from low-performing songs

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Manipulation-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Data%20Visualization-ffffff?logo=python&logoColor=black)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-4C72B0?logo=python&logoColor=white)

## Project Overview
What makes a song go viral? This project conducts an in-depth **Exploratory Data Analysis (EDA)** on a dataset of over **114,000 Spotify tracks** spanning 114 different genres. By leveraging Python, Pandas, Matplotlib, and Seaborn, this analysis aims to identify the underlying audio features (such as danceability, energy, acousticness, and valence) that drive song popularity and separate chart-topping hits from low-performing tracks.

## Key Highlights & Contributions
* **Massive Dataset Analysis:** Processed and analyzed 114K+ Spotify tracks to identify the key audio features most strongly correlated with song popularity.
* **Robust Data Processing:** Executed rigorous data cleaning, handling missing values, and resolving duplicate track IDs (reducing the dataset to ~89K unique tracks while retaining peak popularity). 
* **Feature Engineering:** Engineered new variables, including converting track duration to minutes and creating categorical **Popularity Tiers** (`Low`, `Medium`, `High`, `Viral`) for better comparative analysis.
* **Advanced Visualizations:** Designed multi-layered visualizations including:
  * Correlation heatmaps of all audio features vs. popularity.
  * Density and scatter plots mapping key features against popularity tiers.
  * Popularity distributions by explicit content.
* **Viral Track Profiling:** Profiled the Top 20 viral songs across all 114 genres using specialized heatmaps to visualize the "audio fingerprint" of a hit.
* **Actionable Insights:** Extracted concrete, data-backed insights on the acoustic properties that distinguish viral hits from the rest of the pack.

## Dataset Details
The dataset contains 114,000 rows and 21 columns. Key features analyzed include:
* **Metadata:** `track_id`, `artists`, `track_name`, `track_genre`
* **Target Variable:** `popularity` (Score from 0-100)
* **Audio Features:** `danceability`, `energy`, `loudness`, `speechiness`, `acousticness`, `instrumentalness`, `liveness`, `valence`, `tempo`, `duration_ms` (engineered to `duration_min`), and `explicit`.

## Workflow & Methodology
1. **Data Cleaning & Overview:**
   - Loaded and inspected the dataset.
   - Dropped unnecessary index columns and handled missing values.
   - Deduplicated tracks appearing across multiple genres.
2. **Feature Engineering:**
   - Transformed milliseconds into minutes for better readability.
   - Segmented continuous popularity scores into 4 distinct tiers.
3. **Exploratory Data Analysis (EDA):**
   - Mapped the overall distribution of song popularity.
   - Investigated the overlap of songs across multiple genres.
   - Plotted correlation matrices to find linear relationships between audio metrics.
   - Compared the audio profiles of the top 20 most popular songs globally.

## Installation & Usage
To run this notebook locally, ensure you have Python installed along with the required libraries.
