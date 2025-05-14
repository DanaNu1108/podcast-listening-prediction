# 🎧 Predict Podcast Listening Time

This repository contains a complete solution and experimentation for the [Kaggle Playground Series - Season 5, Episode 4](https://www.kaggle.com/competitions/playground-series-s5e4/overview).  
The goal of the competition is to predict the listening time of podcast episodes based on metadata, popularity scores, publication details, and more.

---

## 📂 Project Structure

├── Podcast_Prediction_Final.ipynb # Full notebook: EDA, modeling, evaluation
├── Podcast_Project_Slides.pdf # Slide deck summarizing the project
└── README.md # Project documentation

---

## 🗃 Dataset

The dataset is not included in this repository due to file size limits.  
You can download the data directly from Kaggle here:  
🔗 [Kaggle Dataset – Playground Series S5E4](https://www.kaggle.com/competitions/playground-series-s5e4/data)

Once downloaded, place `train.csv` and `test.csv` in the same directory as the notebook to run it locally.

---

## 🧾 Project Overview

This is a supervised regression problem focused on estimating podcast listening time using numerical and categorical features. We performed EDA, handled missing values, engineered new features, and evaluated multiple regression models to optimize prediction performance.

---

## 📌 Key Insights

- `Episode_Length_minutes` had a 92% correlation with the target and was the strongest predictor.
- Genre, sentiment, and publication timing had minimal influence.
- Engineered features like `Ad_Density` and a binary `No_Guest` flag improved model performance.

---

## 🧠 Models Used

- Linear Regression — Baseline model
- Gradient Boosting — Tuned with RandomizedSearchCV
- XGBoost — Stable but not top-performing
- Random Forest — Best overall (R² ≈ 0.7784)

---

## 📒 Notebook Summary

- Exploratory Data Analysis (EDA)
- Missing value and outlier handling
- Feature engineering and encoding
- Model training and evaluation
- Comparison using R² and RMSE

---

## 📑 View Presentation

🗂 [Open Project Slides (PDF)](./Podcast_Project_Slides.pdf)

---

## ✅ Final Notes

This project demonstrates how strong preprocessing and thoughtful feature design can significantly improve model performance.  
By combining technical experimentation and insight, we uncovered valuable patterns in podcast engagement behavior.
