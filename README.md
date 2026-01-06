🏏 IPL Win Probability Prediction App

A Machine Learning–powered web application that predicts the win probability of an IPL team in real time based on the current match situation.
Built using Python, scikit-learn, and Streamlit, and deployed on Streamlit Cloud.

🚀 Live Demo

👉 https://iplpredictorproba.streamlit.app

📌 Project Overview

In limited-overs cricket, win probability depends on several dynamic factors like:

Runs left to score

Balls remaining

Wickets in hand

Current and required run rate

Teams and venue

This project uses historical IPL ball-by-ball data to train a classification model that estimates the probability of the batting team winning from any given match situation.

🧠 Machine Learning Pipeline

Data Source: IPL ball-by-ball & match-level data

Feature Engineering:

Runs left

Balls left

Wickets left

Current Run Rate (CRR)

Required Run Rate (RRR)

Batting team, Bowling team, City

Preprocessing:

Categorical encoding using ColumnTransformer

Numerical feature scaling

Model:

Logistic Regression (probability-based output)

Serialization:

Trained pipeline saved as pipe.pkl

🖥️ Web Application (Streamlit)

The Streamlit app allows users to:

Select batting team, bowling team, and venue

Input match situation (score, overs, wickets)

Get real-time win probability for both teams

📂 Project Structure
ipl_prediction/
│
├── app.py              # Streamlit application
├── pipe.pkl            # Trained ML pipeline
├── requirements.txt    # Project dependencies
└── README.md           # Project documentation

⚙️ Installation & Setup (Local)
1️⃣ Clone the repository
git clone https://github.com/<your-username>/ipl_prediction.git
cd ipl_prediction

2️⃣ Create and activate environment (Conda recommended)
conda create -p venv python=3.11 -y
conda activate ./venv

3️⃣ Install dependencies
python -m pip install -r requirements.txt

4️⃣ Run the app
streamlit run app.py

📦 Requirements

Main libraries used:

Python 3.11

streamlit

scikit-learn

pandas

numpy

(Exact versions are listed in requirements.txt)

📊 Example Features Used for Prediction
Feature	Description
runs_left	Runs remaining to win
balls_left	Balls remaining
wickets_left	Wickets in hand
current_run_rate	Current run rate
required_run_rate	Required run rate
batting_team	Batting team
bowling_team	Bowling team
city	Match venue
🎯 Use Cases

Cricket analytics & visualization

Sports data science projects

ML portfolio project

Probability-based decision modeling

🧩 Future Improvements

Over-by-over win probability graph

Support for live match data

More advanced models (XGBoost, Random Forest)

Model retraining with recent IPL seasons

Mobile-friendly UI improvements

👤 Author

Kaustubh Gidh
MS in Data Science | Machine Learning & AI Enthusiast

📫 Feel free to connect on LinkedIn or explore my other ML projects!

⭐ Acknowledgements

IPL Dataset (Kaggle)

Streamlit Documentation

scikit-learn Community
