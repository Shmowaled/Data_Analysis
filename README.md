STC TV Data Analysis & Insights
This repository contains a series of Jupyter Notebooks that perform various data analysis tasks on STC TV (Jawwy) user data. The project explores time-series forecasting, builds a content-based recommendation engine, and demonstrates data storytelling techniques.


T2 - Usage Forecasting (stc_TV_T2.ipynb)
Goal: To forecast total daily user watch hours for the next two months.

Process:
Cleans and parses raw, unstructured time-series data using regular expressions.
Conducts an Exploratory Data Analysis (EDA) to identify peak viewing days of the week.
Builds a predictive model using the Prophet library.
Generates and visualizes a 60-day forecast, including trend and weekly seasonality components.
Dataset: Raw text data embedded in the notebook, representing OCR output from an Excel sheet.

T3 - Movie Recommendation Engine (stc_TV_T3.ipynb)
Goal: To recommend movies to users based on their viewing history.

Process:
Uses a collaborative filtering approach based on user-item interactions.
Filters the dataset to focus on a single genre ('Animation') as a proxy for movies.
Constructs a user-movie matrix to represent viewing patterns.
Calculates the correlation between movies to find similarities.
Generates the top 5 movie recommendations for users who watched "Moana", filtering by popularity (number of views).
Dataset: stc TV Data Set_T3.xlsx

T4 - Data Storytelling (stc_TV_Data_Set_T4.ipynb)
Goal: To demonstrate how to effectively communicate data insights through storytelling (analysis written in Arabic).

Process:
Simulates a business scenario: analyzing the impact of a new "Focus Mode" feature designed to reduce user screen time.
Generates mock "before" and "after" data to represent the feature launch.
Presents a clear narrative analyzing the feature's success, showing a significant drop in average daily screen time.
Visualizes the impact with an effective line chart, highlighting the launch date as a key event.
Dataset: Mock data generated within the notebook for demonstration purposes.

Core Libraries:
pandas: For data manipulation and analysis.
matplotlib & seaborn: For data visualization.
numpy: For numerical operations.
prophet: For time-series forecasting (T2).
pyxlsb: For reading .xlsb Excel files (though T3 uses .xlsx).

Author
SHAHAD