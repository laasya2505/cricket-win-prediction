# cricket-win-prediction
This project is an IPL Win Predictor application developed using Streamlit. The application predicts the probability of the batting team winning or losing an IPL (Indian Premier League) match based on the match's current state.

Key Features:
User Inputs:

Batting Team & Bowling Team: Select from the list of IPL teams.
Host City: Choose the city where the match is being played.
Match Details: Enter the target score, current score, overs completed, and wickets lost.
Backend Model:

A pre-trained machine learning model (stored in pipe.pkl) is used for predictions. This model was trained to compute the probability of a team winning or losing based on match parameters.
Calculations:

The application calculates critical metrics such as:
Runs Left: Target runs minus the current score.
Balls Left: Remaining balls in the innings.
Wickets Remaining: Total wickets (10) minus the wickets lost.
Current Run Rate (CRR): Runs scored per over so far.
Required Run Rate (RRR): Runs required per over to meet the target.
Prediction Output:

The application displays the winning probability for both the batting and bowling teams in percentage form.
Technologies Used:
Streamlit: For building the user interface and hosting the web application.
Python Libraries:
Pandas for data handling.
Pickle for loading the trained machine learning model.
Machine Learning:
A classification model trained to predict match outcomes based on past IPL data.
