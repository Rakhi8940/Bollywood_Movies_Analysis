
Markdown
<p align="center">
  <img src="https://github.com/user-attachments/assets/bd34176f-85c1-437c-b447-ee3b6c2d070c" width="900" alt="Bollywood Movie Analysis Banner" style="margin: 12px 0; border-radius: 18px; background: #fff; box-shadow: 0 4px 16px rgba(0,0,0,0.12); padding: 0;">
</p>

# 🎬 Bollywood Movie Analysis

Bollywood Movie Analysis is a data analytics project that explores trends, patterns, and insights from Bollywood movie datasets using Python. It leverages powerful libraries like NumPy, Pandas, Matplotlib, and Seaborn to perform data cleaning, analysis, and visualization.

## 🎯 Objective

- Analyze Bollywood movie data to uncover trends and insights
- Perform data cleaning and preprocessing for accurate analysis
- Visualize relationships between budget, revenue, and audience engagement
- Identify factors influencing movie success (ROI, release timing, genre, etc.)
- Build strong foundational skills in data analytics using Python

## 📊 Dataset Description

| Feature | Description |
|---------|-------------|
| SINo | Unique identifier for movies |
| ReleaseDate | Movie release date |
| MovieName | Name of the movie |
| ReleaseTime | Release period (LW, FS, HS, N) |
| Genre | Type of movie (Action, Comedy, etc.) |
| Budget | Production budget |
| BoxOfficeCollection | Total earnings |
| YoutubeViews | Trailer views |
| YoutubeLikes | Trailer likes |
| YoutubeDislikes | Trailer dislikes |

## 🛠️ Technologies Used

- **Python** - Programming Language
- **NumPy** - Numerical computations
- **Pandas** - Data manipulation
- **Matplotlib** - Data visualization
- **Seaborn** - Advanced visualization

## 🧑‍💻 Project Workflow

```python
# Importing libraries
import numpy as np
import pandas as pd
from matplotlib import pyplot as plt
import seaborn as sns

# Reading dataset
df = pd.read_csv('bollywood.csv')

# Preview dataset
df.head()
📈 Key Analysis & Insights
📌 Dataset Overview
Total records: 149 movies
📌 Release Time Analysis
Most movies released during Normal period
Least during Long Weekend
📌 Genre Insights
Festive Season leaders: Thriller & Drama
Action genre dominates YouTube views
📌 Yearly Trends
Highest movie releases: 2014
Followed closely by: 2013
📌 High Budget Trends
Movies with budget ≥ 30 crore mostly released in February
📌 ROI (Return on Investment)
Best ROI observed during:

Long Weekend (1.12)
Festive Season (0.97)
Top flop movies (lowest ROI):

Gangoobai
Bandook
Sona Spa
Rajdhani Express
Kya Dilli Kya Lahore
Satya 2
Purani Jeans
Samrat & Co.
Heartless
Kaanchi
📌 Correlation Insights
Box Office vs YouTube Likes: Positive correlation (0.68)
Strong correlation between:
Youtube Views
Youtube Likes
Youtube Dislikes
📊 Visualizations
📦 Genre vs YouTube Views
Python
sns.boxplot(x='Genre', y='YoutubeViews', data=df)
🔥 Correlation Heatmap
Python
sns.heatmap(df[['Budget','BoxOfficeCollection','YoutubeViews','YoutubeLikes','YoutubeDislikes']].corr(), annot=True)
📊 Year vs Box Office Collection
Python
sns.barplot(x='Year', y='BoxOfficeCollection', hue='Genre', data=df, ci=None)
🎯 Movies per Year
Python
sns.countplot(x='Year', data=df)
📉 Budget Distribution
Python
sns.displot(x='Budget', data=df, kind='kde', hue='Genre')
👍 Likes vs 👎 Dislikes Comparison
Python
compare.plot.bar()
🔌 Example Use Cases
Predicting movie success based on budget & engagement
Understanding audience behavior via YouTube metrics
Identifying best release periods for maximum ROI
Genre-based performance comparison
📁 Project Structure
Code
Bollywood-Movie-Analysis/
├── data/
│   └── bollywood.csv
├── notebooks/
│   └── analysis.ipynb
├── scripts/
│   └── analysis.py
├── visuals/
│   └── plots.png
├── README.md
└── requirements.txt
📝 Getting Started
[Add installation and setup instructions here]

🧠 Future Improvements
Add machine learning models for prediction
Build an interactive dashboard (Streamlit/Power BI)
Integrate real-time movie data APIs
Perform sentiment analysis on audience reviews
👩‍💻 Author
Made with ❤️ by Rakhi Yadav

Turning data into blockbuster insights 🎥✨
