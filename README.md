🏎️ F1 Predictive Analytics Platform
A data-driven platform for analyzing Formula 1 performance and predicting career outcomes using machine learning.


📌 Table of Contents
About the Project

Key Features

Tech Stack

Installation

Project Structure

Usage

API Endpoints

Dashboard Screenshots

Future Enhancements

Contributors

📖 About the Project
The F1 Predictive Analytics Platform is a comprehensive tool that leverages historical Formula 1 data, machine learning models, and interactive dashboards to:

Analyze career stats of F1 drivers

Compare driver performance across multiple metrics

Predict career points based on inputs

Visualize data using advanced plots

Built with Flask, Streamlit, and Dash, the platform provides a modern, flexible, and intelligent interface for fans, analysts, and researchers.

🚀 Key Features
🎯 Predictive Modeling: Forecast driver points using Random Forest Regressor

📊 Performance Dashboards: Analyze win rates, podium finishes, and more

🌍 Nationality-Based Insights: Evaluate performance by country

🧠 Clustering & Correlation: Group drivers by performance tiers

🔍 Driver-Level Analytics: Deep-dive into individual stats

⚙️ API-Driven Design: Clean REST endpoints for data and prediction

🧰 Tech Stack
Layer	Technologies
Frontend	HTML, CSS, Bootstrap 5, Plotly.js
Dashboards	Flask, Streamlit, Dash
Backend	Python 3.8+, Pandas, Scikit-learn, NumPy
ML Models	Random Forest Regressor (sklearn)
Data Source	dataset.csv – curated F1 driver data

🛠 Installation
Prerequisites
Python 3.8+

pip (Python package manager)

# 1. Clone the repository
git clone https://github.com/<prasadsolankar>/f1-predictive-analytics.git
cd f1-predictive-analytics

# 2. Install dependencies
pip install -r requirements.txt

# 3. Verify the dataset
Ensure `dataset.csv` is in the project root directory.
🧪 Usage
Option 1: Flask Web App (Recommended)
bash
Copy
Edit
python f1_web_app.py
# Open http://localhost:5000
Option 2: Streamlit Dashboard
bash
Copy
Edit
python run_dashboard.py
# Choose Option 1
# Opens at http://localhost:8501
Option 3: Dash Dashboard
bash
Copy
Edit
python run_dashboard.py
# Choose Option 2
# Opens at http://localhost:8050
📁 Project Structure
graphql
Copy
Edit
f1-predictive-analytics/
│
├── f1_web_app.py             # Flask application
├── f1_analytics_platform.py  # Streamlit dashboard
├── dash_f1_dashboard.py      # Dash dashboard
├── run_dashboard.py          # Dashboard launcher
├── launch_web_app.py         # Web app launcher
├── dataset.csv               # F1 driver dataset
├── templates/                # HTML templates for Flask
│   ├── index.html
│   └── dashboard.html
└── requirements.txt          # Python dependencies
📡 API Endpoints (Flask)
Method	Endpoint	Description
GET	/api/overview_stats	Summary statistics of all drivers
GET	/api/top_drivers	Top 10 drivers by career wins
GET	/api/driver_details/<name>	Full stats for a given driver
POST	/api/predict	Predict points using performance input
GET	/api/win_rate_distribution	Histogram plot of win rates
GET	/api/championship_analysis	Top drivers by championships
GET	/api/nationality_analysis	Nationality-based scatter plot
GET	/api/correlation_matrix	Correlation heatmap
GET	/api/performance_clustering	Performance-based cluster plot

🖼️ Dashboard Screenshots
Include screenshots here (upload images to GitHub or use direct links)

🌱 Future Enhancements
📱 Mobile app version (React Native or Flutter)

📈 Real-time race data and telemetry integration

🧠 Deep learning models and time series predictions

💬 Sentiment analysis using NLP

👥 User accounts and personalized dashboards

👥 Contributors
TEAM AI
Team Leader: Ruturaj Nagane
Project Members: [Vikram Thorat,Prasad Solankar,Omkar Solankar]
