# Movie Dataset Analysis & Prediction

*Note: This project was created as a personal learning exercise to practice data manipulation with Pandas and learn the basics of Machine Learning.*

This project explores a dataset of around 4,800 movies. The goal was to find interesting trends in the film industry and build simple models to predict a movie's financial success based on its budget, release year and genre.

## Dataset
The data used in this project was downloaded from Kaggle: [Movies Dataset (abdallahwagih/movies)](https://www.kaggle.com/datasets/abdallahwagih/movies)

## Project Files

### 1. Data Analysis (`movie_analysis.ipynb`)
In this notebook, I loaded and cleaned the raw data. I used graphs to answer a few basic questions:
* Which genres are the most popular?
* Does a higher budget actually lead to higher revenue?
* How have average movie budgets changed over time?
* Which movies made the highest profit?

### 2. Revenue Prediction (`movie_revenue_prediction.ipynb`)
In this notebook, I built a **Linear Regression** model. The goal was to see if I could predict the exact revenue of a movie based on its budget, year and genre.
* The model did a decent job for average movies but struggled to predict massive outliers.

### 3. Hit or Flop Classification (`movie_profit_classification.ipynb`)
Since predicting an exact dollar amount was difficult, I changed the problem. I built a **Logistic Regression** model to simply predict if a movie would make a profit (1) or a flop (0).
* I balanced the model so it wouldn't just guess "Hit" every time and then visualized the results using a Confusion Matrix.

## Libraries Used
* **Pandas:** Data cleaning, manipulation
* **Matplotlib & Seaborn:** Data visualization (Scatter plots, trend lines and Heatmaps)
* **Scikit-Learn:** Machine Learning (Train/Test splitting, Linear Regression, Logistic Regression, Evaluation metrics)