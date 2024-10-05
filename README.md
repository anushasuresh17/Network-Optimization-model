# Network-Optimization-model

Project Overview
This project aims to analyze and optimize network performance by identifying key factors that impact signal strength. We used Random Forest Regression to determine the most significant variables affecting network performance and provided actionable insights for infrastructure improvements.

Dataset
The dataset consists of the following columns:

Timestamp: Date and time of the network activity.
Signal Strength (dBm): Strength of the signal, measured in dBm.
SNR: Signal-to-Noise Ratio.
Call Duration (s): Duration of the call in seconds.
Environment: Type of environment (e.g., Urban, Suburban).
Attenuation (dB): The loss of signal strength during transmission.
Distance to Tower (km): Distance from the user to the nearest tower.
Tower ID: Identifier for the tower.
Call Type: Type of call (e.g., Voice, Data).
Incoming/Outgoing: Status of the call (incoming or outgoing).
Project Workflow
Data Exploration and Cleaning:

Checked for missing values and outliers.
Converted categorical columns to numerical using one-hot encoding.
Exploratory Data Analysis:

Visualized numerical columns using box plots and pair plots to understand the data distribution.
Determined that there were no significant outliers.

Modeling:

Split the data into training and testing sets.
Tested linear regression, but due to low R-squared values, moved to Random Forest Regression.
Used Random Forest to build a regression model to predict signal strength.

Key Insights:

The most important factors influencing signal strength were:
Attenuation
Call Duration
Distance to Tower
SNR
Environment and Tower ID had moderate influence, while Call Type and Incoming/Outgoing status had minimal effect.


Recommendations for Network Optimization:

Reduce Attenuation by minimizing physical obstructions and improving transmission power.
Optimize Tower Locations to reduce the distance between users and towers.
Improve SNR by reducing signal interference.
Results
Achieved an R-squared score using Random Forest Regression.
Provided key insights for network performance improvement, which can guide future infrastructure optimization efforts.

Requirements
pandas
numpy
matplotlib
seaborn
statsmodels
scikit-learn
