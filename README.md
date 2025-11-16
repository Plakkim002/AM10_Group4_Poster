# AM10_Group4_Poster
This is the repository for the poster presentation of study group 4 for AM10

# Predicting Premier League Final Standings

## 1. Topic
**Predicting Premier League Final Standings**

---

## 2. Issues or Questions Being Addressed
The objective of this project is to predict the final league standings of the **2025/26 Premier League season** using regression analysis.  
We will be examining historical data from the past few seasons to identify the key performance factors that influence success and use these relationships to forecast how the current season might conclude.

---

## 3. Source of Data
The dataset for this project will be obtained from **[Football-Data.co.uk](https://www.football-data.co.uk/)**, an open-source platform that provides historical records of Premier League matches.  

The data includes:
- Full-time and half-time scores  
- Shots and shots on target  
- Corners, fouls, yellow and red cards  
- Match results  

The site is updated weekly, so current **2025/26 season results** are available as well.  
This makes it feasible to use all past seasons up to **2024/25** for model training and the **2025/26 season’s partial data** for prediction.

The data can be downloaded in CSV format and will require cleaning and aggregation to create season-level summaries, such as:
- Total goals  
- Average shots per match  
- Win ratios for each team  

---

## 4. Statistical Techniques
Our work will begin with **data cleaning and preparation**, building from match-level data to season-level summaries that capture each team’s performance across multiple indicators.  

**Exploratory data analysis (EDA)** will then be used to uncover patterns and relationships — for example, correlations between goals scored, shots, fouls, and total points earned.  
A key part of this analysis will be exploring patterns in the current season that may not yet be reflected in the league standings.

**Feature engineering** will involve constructing new variables such as:
- Goal difference  
- Total wins  
- Average shots per game  

These features help improve the predictive power of the model.

The main modelling approach will be **multiple linear regression**, where the **target variable** is the total number of points a team earns in a season.  
The model will be trained on historical seasons and evaluated on a recent season (most likely **2024/25**) to assess its accuracy.  
Once validated, the model will be applied to the **2025/26 season’s data** to estimate final points and predict the final league standings.

** Instructions to run the code: **
1. git clone the repository
2. Open the Jupyter Notebook file `Sudy_Group_4_Poster_Code.ipynb` in Jupyter Notebook or Jupyter Lab
3. Run requirements.txt to install the necessary libraries:
    ```
    pip install -r requirements.txt
    ```
4. Run all the cells in the notebook to generate the results and visualizations