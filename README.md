# Netflix Content Analytics Project

## Project Overview
This data analytics project analyzes the Netflix dataset (8,807 titles from Kaggle) to uncover trends in genres, release years, countries, and ratings. It uses Python for data processing, SQL for querying, machine learning for predictions, and Plotly for interactive visualizations. Ideal for streaming strategy insights (e.g., top genres in India).

**Problem Statement**: How can Netflix optimize content based on historical data? Key findings: Dramas dominate (24% of library); newer releases predict lower average ratings (mature content trend).

**Skills Demonstrated**:
- Data Cleaning & EDA (Pandas, NumPy)
- SQL Queries (SQLite)
- Predictive Modeling (Scikit-learn Linear Regression)
- Interactive Visualizations (Plotly)
- Ready for Dashboarding (e.g., Tableau import)

## Dataset
- Source: [Netflix Movies and TV Shows (Kaggle)](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- Columns: show_id, type, title, director, cast, country, date_added, release_year, rating, duration, listed_in, description
- Shape: 8,807 rows × 12 columns

## Setup Instructions
1. **Environment**: Python 3.8+ with Anaconda (recommended).
2. **Install Dependencies**: Run `pip install -r requirements.txt` (see below).
3. **Download Dataset**: Place `netflix_titles.csv` in the project folder (from Kaggle).
4. **Run the Notebook**: Open `netflix_analysis.ipynb` in Jupyter Notebook (`jupyter notebook`).
   - Kernel > Restart & Run All (takes ~2 min).
5. **Outputs Generated**:
   - `netflix.db`: SQLite database for SQL queries.
   - Plot files: `genre_pie.png/html`, `release_trend.png/html`, `country_heatmap.png/html` (interactive in browser).
6. **Explore SQL**: Open `netflix.db` with [DB Browser for SQLite](https://sqlitebrowser.org/) or run queries in the notebook.

## Key Results & Insights
- **Top Genres**: Dramas (2,414 titles, 24%), Comedies (1,554, 16%), Documentaries (1,540, 15%).
- **Release Trends**: Surge in content post-2015; peak ~2020 (pandemic effect?).
- **Regional Preferences**: US leads (3,021 titles); India strong in 'Mature' ratings.
- **ML Prediction**: Simple Linear Regression (R²=0.072) predicts ~1.87/5 rating for a 2024 Drama (trend toward mature content).
- **Visuals**: See attached PNGs/HTMLs—e.g., pie chart shows genre distribution; line chart tracks yearly releases.

## Files Included
- `netflix_analysis.ipynb`: Main Jupyter Notebook (analysis code).
- `netflix_titles.csv`: Raw dataset.
- `netflix.db`: Generated SQLite database.
- `extra_sql_queries.sql`: Advanced SQL examples.
- Plot outputs: PNG images and HTML interactives.
- `requirements.txt`: Library dependencies.

## Next Steps / Extensions
- Import to Tableau/Power BI for interactive dashboard.
- Advanced ML: Use Random Forest or add features like cast popularity.
- API Integration: Pull live Netflix data via unofficial APIs.
- Deployment: Host on Streamlit/Heroku for a web app.

## Author
Divyanshu Rai 



