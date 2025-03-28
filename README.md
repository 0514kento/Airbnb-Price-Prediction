# 🏙️ Airbnb Price Prediction: NYC vs. LA

**Team 10B Final Project**  
Kento Morita, TingHsuan (Oceana) Chan, Jiyun Sun, Yumo Jiang, Chuhan Zhang

---

## 📘 Overview

This project investigates Airbnb pricing in **New York City** and **Los Angeles** using machine learning classification models to categorize listings as **“high”** or **“low”** priced.

Using 2023 data from [Kaggle](https://www.kaggle.com/datasets/kritikseth/us-airbnb-open-data), we examine key listing features like `room_type`, `minimum_nights`, `reviews`, and `availability`, and compare model performance across cities.

---

## 🧠 Key Techniques

- **Data Preprocessing**: Outlier removal, one-hot encoding, datetime transformation, feature scaling.
- **Feature Engineering**: `price_category`, `days_from_last_review_23`, SMOTE for class imbalance.
- **Models Used**:
  - Logistic Regression (with GridSearch & SMOTE)
  - Decision Tree (with hyperparameter tuning)
  - Random Forest
  - Neural Networks (fine-tuned with Keras)

---

## 🎯 Results Summary

| Model                          | Los Angeles | New York City |
|-------------------------------|-------------|---------------|
| Logistic Regression (tuned)   | 79.3%       | 78.3%         |
| Decision Tree (tuned)         | 79.4%       | 78.6%         |
| Random Forest (SMOTE)         | 79.4%       | **78.7%**     |
| Neural Network (tuned)        | **79.7%**   | 78.6%         |

- **Random Forest** was the most interpretable and consistent.
- **Neural Networks** achieved the highest accuracy in LA but are more complex to interpret.
- **Room Type** was the most significant predictor in both cities.

---

## 💡 Key Takeaways

- Private rooms offer better value for budget-conscious travelers.
- Listings with flexible minimum night stays are better for short-term visits.
- Seasonal trends impact pricing—book early for holidays.
- While ML models improve accuracy, room details like amenities could further boost predictions.

---

## 🛠️ Technologies

- Python (Pandas, NumPy, scikit-learn, Keras)
- SMOTE for handling class imbalance
- Matplotlib / Seaborn for data visualization
- GridSearchCV for hyperparameter optimization

---

## 📚 References

- [Airbnb Open Data (Kaggle)](https://www.kaggle.com/datasets/kritikseth/us-airbnb-open-data)
- Plots, methods, and results detailed in `report.pdf`.

---

> _“Smarter pricing starts with better prediction.”_
